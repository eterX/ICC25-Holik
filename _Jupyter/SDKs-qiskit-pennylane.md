

# qisKit

- tutoriales de Qiskit
	- [https://qiskit.org/textbook/preface.html](https://qiskit.org/textbook/preface.html)


---
## simulación Aer

https://qiskit.github.io/qiskit-aer/tutorials/1_aersimulator.html#

https://quantum.cloud.ibm.com/docs/en/api/qiskit/qiskit.circuit.QuantumCircuit

```python
# ejemplo de estado guardado y luego tratado algebraicamente
import qiskit as qk
from qiskit_aer import AerSimulator

# Define the state vector
eta = [np.sqrt(2/3), np.sqrt(1/3) * np.exp(1j * np.pi/3)]
estado1 = qk.QuantumCircuit(1, 1)
estado1.initialize(eta, 0)
estado1.save_statevector(label='my_sv')# IMPORTANTE: save_statevector ANTES de medir
estado1.measure_all()
estado1.draw('mpl')

  

# Usar AerSimulator con método statevector

backend = AerSimulator(method='statevector')
```
### inicializar con un estado arbitrario

https://quantum.cloud.ibm.com/docs/en/api/qiskit/qiskit.circuit.library.Initialize

### salvar el estado, antes de una medición

>[!warn] en qk 1.0+ se movió a un  módulo 

https://github.com/Qiskit/qiskit-aer/blob/main/qiskit_aer/library/save_instructions/save_statevector.py

To use `save_statevector`, the circuit must be run on a simulator backend such as `AerSimulator` or `QasmSimulator` with the method set to `'statevector'`

1. **`AerSimulator(method='statevector')`**: Especificar el método para asegurar compatibilidad
2. **`save_statevector(label='nombre') `ANTES de medir**: Guardar el estado antes de que colapse por la medición
3.  **Extraer con `result.data(0)['my_sv']`**: Obtienes el vector de estado guardado
4. **Operar algebraicamente**: el estado es un array de numpy/sympy que se puede usar para calcular matrices de densidad, productos internos, etc.

  

---
## simulación stateVectorSampler

no confundir con 
https://quantum.cloud.ibm.com/docs/en/api/qiskit/qiskit.primitives.StatevectorSampler

- If `save_statevector` is not found, ensure you're using `from qiskit_aer import AerSimulator` (not the old qiskit.Aer)                                    │
- Always use `method='statevector'` when creating the simulator

---
#  pennylane


---

# Python 


## numpy y simpy

- enlaces - numpy
- enlaces - sympy
	- https://live.sympy.org/
	- [matrices](https://docs.sympy.org/latest/tutorials/intro-tutorial/matrices.html)
	- 
```python
# Verificar que es un número real en el rango [0,1]
error_redondeo=1e-10
assert np.abs(Z.imag) < error_redondeo, "La probabilidad debe ser real"
assert error_redondeo <= Z.real <= error_redondeo, "La probabilidad debe estar en el rango [0,1]"
```

>[!tip] `lambda` is a reserved keyword in Python, so to create a Symbol called $\lambda$, use **lamda** (without the b). It will still pretty print as  $\lambda$


## numpy ↔ simpy

$$\left[\begin{matrix}\frac{\sqrt{2}}{2} & 2\\3 & 4 e^{\frac{i \pi}{3} }\end{matrix}\right]$$
```python
numpy_array = np.array([[1/np.sqrt(2), 2], [3, np.sqrt(16) * np.exp(1j * np.pi/3)]])
display(numpy_array) 
sympy_matrix = sp.Matrix(numpy_array)   
display(sympy_matrix) 
numpy_array = np.array(sympy_matrix).astype(np.complex128)
display(numpy_array)
```

$Z^{\otimes2}=\ket{\sigma_z}\otimes\ket{\sigma_z}$
```python
 Z_2qubits = sp.kronecker_product(sigma_z,sigma_z)
 Z_2qubits = np.(sigma_z,sigma_z)
```

Proyector $P_Z=\ket{\sigma_z}\bra{\sigma_z}$
```python
proyector_z = np.outer(ket_zero, np.conj(ket_zero))
```

## Álgebra

## producto exterior

`np.outer(A, B)` calcula el producto externo $A$ ⊗ $B$ donde si $A$ es dim(n,1) y $B$ es dim(m,1), entonces el resultado es una matriz dom(n,m). `np.outer([a, b], [a*, b*])`, genera una matriz donde cada elemento resulta del producto de los componentes originales con sus conjugados: `[[a·a*, a·b*], [b·a*, b·b*]]`

 Para obtener $\rho_{\psi}=\ket{\psi}\bra{\psi}$:
 ```python
 densidad_phi=np.outer(ket_psi, ket_psi.conj().T)
```

>[!warning] intercambiando los argumentos, calcula $\bra{i}\otimes\ket{i}$, NO el producto externo

 ```python
 _=np.outer(ket_psi.conj(), ket_psi) #calcula $\bra{i}\otimes\ket{i}$
```


## autovalores y autovectores - diagonalización

```python
eigenvalues, eigenvectors = np.linalg.eig(np.array(([[1,2],[3,4]])))
eigenvalues =  sp.Matrix([[1,2],[3,4]]).eigenvalues()
eigenvectors =  sp.Matrix([[1,2],[3,4]]).eigenvects()
```

```python
#to diagonalize a matrix, use `diagonalize`. `diagonalize` returns a tuple , where  is diagonal and $M=PDP^1$
P, D = M.diagonalize()
```

## Física

### bases

```python
# base computacional 
ket_zero = np.array([1/np.sqrt(2), 0])
ket_one = np.array([0, 1/np.sqrt(2)])

# base Hadamard
ket_plus = np.array([1/np.sqrt(2), 1/np.sqrt(2)])
ket_minus = np.array([1/np.sqrt(2), -1/np.sqrt(2)])

# base Y
ket_i =      np.array([[1/np.sqrt(2)], [1j/np.sqrt(2)]])  # Estado |i>
ket_minusi =  np.array([[1/np.sqrt(2)], [-1j/np.sqrt(2)]]) # Estado |-i>

proyector_i=np.outer(ket_i,ket_i.conj()) # notar orden y no necesita .T()
proyector_minusi=np.outer(ket_minusi,ket_minusi.conj())

#imprime
display(f"|-i>",sp.Matrix(proyector_minusi))
display(f"|i>",sp.Matrix(proyector_i))
#verificacion
assert np.allclose(proyector_minusi + proyector_i, np.eye(2))
```

### Regla de Born
```python
# medir $\psi$ en base de Hadamard
P_plus = np.abs(np.dot(np.conjugate(ket_plus), psi_vector))**2
P_minus = np.abs(np.dot(np.conjugate(ket_minus), psi_vector))**2

# Probabilidad: p(+) = <eta|M_+|eta>
# Usar @ para producto matricial (equivalente a np.dot() pero más legible)
P_plus = np.conj(psi_vector) @ proyector_plus @ psi_vector
```


## Computación
### compuertas

```python
compuerta_h=qk.circuit.library.HGate().to_matrix()
ket_plus_alternativo = compuerta_h * ket_zero.transpose().conjugate() 
```

