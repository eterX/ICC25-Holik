

# qisKit

---
## simulación Aer

https://qiskit.github.io/qiskit-aer/tutorials/1_aersimulator.html#

https://quantum.cloud.ibm.com/docs/en/api/qiskit/qiskit.circuit.QuantumCircuit
```python
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
### salvar el estado, antes de una medición

>[!warn] en qk 1.0+ se movió a la módulo 

https://github.com/Qiskit/qiskit-aer/blob/main/qiskit_aer/library/save_instructions/save_statevector.py

To use `save_statevector`, the circuit must be run on a simulator backend such as `AerSimulator` or `QasmSimulator` with the method set to `'statevector'`

  1. save_statevector() ANTES de medir: Guardas el estado antes de que colapse por la medición
  2. AerSimulator(method='statevector'): Especificas el método para asegurar compatibilidad
  3. Extraes con result.data(0)['my_sv']: Obtienes el vector de estado guardado
  4. Operas algebraicamente: Ahora eta_vector es un array de numpy que puedes usar para calcular matrices de densidad, productos internos, etc.

  Así puedes poner save_statevector(label='nombre') en cualquier punto del circuito y extraer el estado justo en ese momento, sin importar qué operaciones
  vengan después.


---
## simulación stateVectorSampler

https://quantum.cloud.ibm.com/docs/en/api/qiskit/qiskit.primitives.StatevectorSampler


---
#  pennylane
