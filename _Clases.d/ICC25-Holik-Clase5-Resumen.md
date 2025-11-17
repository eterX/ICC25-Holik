Educación:** Crear materiales didácticos, cursos online, tutoriales

**Próximos pasos sugeridos:**
1. Instalar ambos frameworks (Qiskit + Braket)
2. Reproducir todos los ejemplos de la clase
3. Modificar parámetros, explorar variaciones
4. Comenzar a implementar algoritmos sencillos (próxima clase)
5. Considerar contribuir a proyectos open-source (issues de principiantes en GitHub de Qiskit)

---

## Referencias Cruzadas a Clases Anteriores

### Integración con Clase 1

**Conceptos realizados:**

1. **[[ICC25-Holik-Clase1-Resumen#Computadoras Cuánticas Reales|Hardware Cuántico]]**
   - **Clase 1:** Mención abstracta de plataformas (IBM, IonQ, Rigetti)
   - **Clase 5:** Acceso práctico vía Qiskit/Braket, fake providers que emulan hardware real

2. **[[ICC25-Holik-Clase1-Resumen#Era NISQ|Ruido en Era NISQ]]**
   - **Clase 1:** Descripción cualitativa de errores
   - **Clase 5:** Modelado cuantitativo (p=2-5%), simulación realista

3. **[[ICC25-Holik-Clase1-Resumen#Ventaja Cuántica|Verificación Experimental]]**
   - **Clase 1:** Concepto de supremacía cuántica
   - **Clase 5:** Herramientas para medir fidelidad, comparar clásico vs. cuántico

### Integración con Clase 2

**Aplicación de estructuras algebraicas:**

1. **[[ICC25-Holik-Clase2-Resumen#Números Complejos|Amplitudes de Probabilidad]]**
   - **Clase 2:** Definición matemática de α, β ∈ ℂ
   - **Clase 5:** Verificación numérica: |α|² + |β|² ≈ 1.0 en simulaciones

2. **[[ICC25-Holik-Clase2-Resumen#Espacios Vectoriales|Vectores de Estado]]**
   - **Clase 2:** Teoría abstracta de ℂⁿ
   - **Clase 5:** Representación concreta en Python: `np.array([alpha, beta])`

3. **[[ICC25-Holik-Clase2-Resumen#Probabilidad Frecuentista|Interpretación de Probabilidad]]**
   - **Clase 2:** Definición P = lim(N→∞) freq
   - **Clase 5:** Demostración empírica con gráficos de convergencia

### Integración con Clase 3

**Compuertas en acción:**

1. **[[ICC25-Holik-Clase3-Resumen#Compuerta Hadamard|Hadamard Práctica]]**
   - **Clase 3:** Matemática H = (1/√2)[[1,1],[1,-1]]
   - **Clase 5:** Código `circuit.h(0)` y verificación de superposición

2. **[[ICC25-Holik-Clase3-Resumen#Compuertas Pauli|X Gate]]**
   - **Clase 3:** Definición teórica X|0⟩ = |1⟩
   - **Clase 5:** Implementación `circuit.x(0)` en circuito singlete

3. **[[ICC25-Holik-Clase3-Resumen#Circuitos Cuánticos|Notación de Circuitos]]**
   - **Clase 3:** Diagramas abstractos
   - **Clase 5:** Generación automática con `circuit.draw()`

### Integración con Clase 4

**Sistemas compuestos:**

1. **[[ICC25-Holik-Clase4-Resumen#Producto Tensorial|Dos Qubits]]**
   - **Clase 4:** Definición ℂ² ⊗ ℂ² = ℂ⁴
   - **Clase 5:** Implementación `QuantumCircuit(2, 2)` en Qiskit

2. **[[ICC25-Holik-Clase4-Resumen#Compuerta CNOT|CNOT Entrelazante]]**
   - **Clase 4:** Tabla de verdad y matriz 4×4
   - **Clase 5:** Uso práctico `circuit.cx(0,1)` para crear entrelazamiento

3. **[[ICC25-Holik-Clase4-Resumen#Entrelazamiento Cuántico|Estados de Bell]]**
   - **Clase 4:** Derivación matemática de singlete
   - **Clase 5:** Construcción y verificación experimental con 10000 shots

### Progresión Completa (Clases 1-5)

```
Clase 1          Clase 2         Clase 3          Clase 4           Clase 5
(Conceptos)  →   (Matemática) →  (Compuertas)  →  (Multi-Qubit)  →  (Implementación)
─────────────────────────────────────────────────────────────────────────────────────
QC existe        ℂⁿ espacios     H, X, Z          CNOT              Qiskit/Braket
Ruido NISQ       Combinaciones   Circuitos        Entrelazamiento   NoiseModel
Algoritmos       lineales        Unitariedad      Producto ⊗        Transpilación
Aplicaciones     Probabilidad    Reversibilidad   Bell states       Convergencia N→∞
```

---

## Anexo: Guía de Instalación Completa

### Para Windows

**Paso 1: Instalar Anaconda**
1. Descargar desde https://www.anaconda.com/download
2. Ejecutar instalador (Anaconda3-2024.x-Windows-x86_64.exe)
3. Durante instalación:
   - ✓ "Add Anaconda to PATH" (opcional pero recomendado)
   - ✓ "Register Anaconda as default Python"
4. Verificar: Abrir "Anaconda Prompt", escribir `conda --version`

**Paso 2: Crear Entorno Virtual**
```bash
conda create -n qiskit_env python=3.11
conda activate qiskit_env
```

**Paso 3: Instalar Librerías**
```bash
pip install qiskit
pip install qiskit-aer
pip install amazon-braket-sdk
pip install matplotlib
pip install jupyter
```

**Paso 4: Verificar Instalación**
```bash
python -c "import qiskit; print(qiskit.__version__)"
python -c "import braket; print(braket.__version__)"
```

**Paso 5: Lanzar Jupyter**
```bash
jupyter notebook
```

### Para macOS

**Paso 1: Instalar Anaconda**
1. Descargar desde https://www.anaconda.com/download
2. Abrir archivo .pkg descargado
3. Seguir asistente de instalación
4. Abrir Terminal, verificar: `conda --version`

**Paso 2-5:** Igual que Windows (los comandos son idénticos)

**Alternativa (Homebrew):**
```bash
brew install --cask anaconda
echo 'export PATH="/usr/local/anaconda3/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

### Para Linux (Ubuntu/Debian)

**Paso 1: Descargar Anaconda**
```bash
wget https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Linux-x86_64.sh
bash Anaconda3-2024.06-1-Linux-x86_64.sh
```

**Durante instalación:**
- Leer licencia (presionar Enter repetidamente)
- Escribir "yes" para aceptar
- Confirmar ubicación (default: ~/anaconda3)
- **Importante:** Escribir "yes" cuando pregunte "initialize Anaconda3"

**Activar cambios:**
```bash
source ~/.bashrc
```

**Verificar:**
```bash
conda --version
which python  # Debería mostrar ~/anaconda3/bin/python
```

**Paso 2-5:** Igual que Windows

### Troubleshooting Común

**Problema: "conda: command not found"**
- **Solución:** Anaconda no está en PATH
- Windows: Reiniciar computadora, usar "Anaconda Prompt"
- Linux/Mac: Agregar a `.bashrc` o `.zshrc`:
  ```bash
  export PATH="$HOME/anaconda3/bin:$PATH"
  ```

**Problema: "ModuleNotFoundError: No module named 'qiskit'"**
- **Solución:** Entorno no activado o librería no instalada
  ```bash
  conda activate qiskit_env
  pip install qiskit
  ```

**Problema: "ImportError: DLL load failed" (Windows)**
- **Solución:** Instalar Microsoft Visual C++ Redistributable
- Descargar de: https://aka.ms/vs/17/release/vc_redist.x64.exe

**Problema: Jupyter no abre (puerto ocupado)**
- **Solución:** Especificar puerto diferente
  ```bash
  jupyter notebook --port=8889
  ```

**Problema: Qiskit corre lento en Windows**
- **Solución:** Puede ser por antivirus escaneando archivos Python
- Agregar carpeta Anaconda a excepciones del antivirus

---

## Anexo: Código Completo de Ejemplos

### Ejemplo 1: Estado Singlete Completo (Qiskit)

```python
"""
Generación y verificación del estado singlete usando Qiskit
Autor: Dr. Federico Holik - Clase 5
"""

# Importaciones
from qiskit import QuantumCircuit, transpile
from qiskit_aer import AerSimulator
from qiskit.visualization import plot_histogram
import matplotlib.pyplot as plt
import numpy as np

# ============================================
# 1. DEFINIR CIRCUITO
# ============================================
def create_singlet_circuit():
    """Crea circuito para estado singlete |Φ⁻⟩"""
    circuit = QuantumCircuit(2, 2)  # 2 qubits, 2 bits clásicos
    
    # Secuencia de compuertas
    circuit.x(0)      # X en qubit 0
    circuit.x(1)      # X en qubit 1
    circuit.h(0)      # Hadamard en qubit 0
    circuit.cx(0, 1)  # CNOT: control=0, target=1
    
    # Mediciones (obligatorias en Qiskit!)
    circuit.measure([0, 1], [0, 1])
    
    return circuit

# ============================================
# 2. SIMULADOR IDEAL (SIN RUIDO)
# ============================================
def run_ideal_simulation(circuit, shots=10000):
    """Ejecuta simulación sin ruido"""
    backend = AerSimulator()
    job = backend.run(circuit, shots=shots)
    result = job.result()
    counts = result.get_counts(circuit)
    return counts

# ============================================
# 3. SIMULADOR RUIDOSO
# ============================================
def run_noisy_simulation(circuit, shots=10000, p_error=0.02):
    """Ejecuta simulación con ruido depolarizing"""
    from qiskit_aer.noise import NoiseModel, depolarizing_error
    
    # Crear modelo de ruido
    noise_model = NoiseModel()
    
    # Agregar errores a compuertas
    error_h = depolarizing_error(p_error, 1)
    error_cx = depolarizing_error(p_error*2, 2)  # CNOT más ruidoso
    
    noise_model.add_all_qubit_quantum_error(error_h, ['h'])
    noise_model.add_all_qubit_quantum_error(error_cx, ['cx'])
    
    # Backend con ruido
    backend_noisy = AerSimulator(noise_model=noise_model)
    
    # Ejecutar
    job = backend_noisy.run(circuit, shots=shots)
    result = job.result()
    counts = result.get_counts(circuit)
    
    return counts

# ============================================
# 4. ANÁLISIS DE CONVERGENCIA
# ============================================
def convergence_analysis(circuit):
    """Analiza convergencia con diferentes números de shots"""
    shot_values = [10, 50, 100, 500, 1000, 5000, 10000]
    results = {}
    
    backend = AerSimulator()
    
    for shots in shot_values:
        job = backend.run(circuit, shots=shots)
        counts = job.result().get_counts(circuit)
        
        # Calcular probabilidades
        total = sum(counts.values())
        prob_01 = counts.get('01', 0) / total
        prob_10 = counts.get('10', 0) / total
        
        results[shots] = {'01': prob_01, '10': prob_10}
    
    return results

# ============================================
# 5. VISUALIZACIÓN
# ============================================
def plot_results(counts_ideal, counts_noisy):
    """Grafica comparación ideal vs. ruidoso"""
    fig, axes = plt.subplots(1, 2, figsize=(14, 5))
    
    # Subplot 1: Ideal
    axes[0].bar(counts_ideal.keys(), counts_ideal.values(), color='skyblue')
    axes[0].set_title('Simulador Ideal')
    axes[0].set_xlabel('Estado Medido')
    axes[0].set_ylabel('Frecuencia')
    axes[0].axhline(y=5000, color='r', linestyle='--', label='Teórico (50%)')
    axes[0].legend()
    
    # Subplot 2: Ruidoso
    axes[1].bar(counts_noisy.keys(), counts_noisy.values(), color='salmon')
    axes[1].set_title('Simulador Ruidoso')
    axes[1].set_xlabel('Estado Medido')
    axes[1].set_ylabel('Frecuencia')
    axes[1].axhline(y=5000, color='r', linestyle='--', label='Teórico (50%)')
    axes[1].legend()
    
    plt.tight_layout()
    plt.show()

def plot_convergence(results):
    """Grafica convergencia estadística"""
    shots = list(results.keys())
    probs_01 = [results[n]['01'] for n in shots]
    errors = [abs(results[n]['01'] - 0.5) for n in shots]
    
    fig, axes = plt.subplots(1, 2, figsize=(14, 5))
    
    # Subplot 1: Probabilidad vs. N
    axes[0].plot(shots, probs_01, 'o-', markersize=8)
    axes[0].axhline(y=0.5, color='r', linestyle='--', label='Teórico (0.5)')
    axes[0].set_xscale('log')
    axes[0].set_xlabel('Número de Shots (N)')
    axes[0].set_ylabel('P(|01⟩) observado')
    axes[0].set_title('Convergencia a Valor Teórico')
    axes[0].legend()
    axes[0].grid(True, alpha=0.3)
    
    # Subplot 2: Error vs. N (log-log)
    axes[1].plot(shots, errors, 'o-', color='orange', markersize=8)
    axes[1].plot(shots, [0.5/np.sqrt(n) for n in shots], '--', 
                 color='gray', label='~1/√N')
    axes[1].set_xscale('log')
    axes[1].set_yscale('log')
    axes[1].set_xlabel('Número de Shots (N)')
    axes[1].set_ylabel('|P_obs - 0.5|')
    axes[1].set_title('Error Absoluto')
    axes[1].legend()
    axes[1].grid(True, alpha=0.3)
    
    plt.tight_layout()
    plt.show()

# ============================================
# 6. PROGRAMA PRINCIPAL
# ============================================
def main():
    """Función principal - ejecuta todos los análisis"""
    
    print("=" * 60)
    print("GENERACIÓN Y ANÁLISIS DEL ESTADO SINGLETE")
    print("=" * 60)
    
    # Crear circuito
    circuit = create_singlet_circuit()
    print("\n1. Circuito Cuántico:")
    print(circuit.draw(output='text'))
    
    # Simulación ideal
    print("\n2. Ejecutando simulación ideal (10000 shots)...")
    counts_ideal = run_ideal_simulation(circuit, shots=10000)
    print(f"   Resultados: {counts_ideal}")
    
    # Calcular probabilidades
    total = sum(counts_ideal.values())
    prob_01_ideal = counts_ideal.get('01', 0) / total
    prob_10_ideal = counts_ideal.get('10', 0) / total
    print(f"   P(01) = {prob_01_ideal:.4f}")
    print(f"   P(10) = {prob_10_ideal:.4f}")
    print(f"   P(01) + P(10) = {prob_01_ideal + prob_10_ideal:.4f}")
    
    # Simulación ruidosa
    print("\n3. Ejecutando simulación ruidosa (p=0.02, 10000 shots)...")
    counts_noisy = run_noisy_simulation(circuit, shots=10000, p_error=0.02)
    print(f"   Resultados: {counts_noisy}")
    
    # Calcular error
    states_forbidden = counts_noisy.get('00', 0) + counts_noisy.get('11', 0)
    error_rate = states_forbidden / 10000
    print(f"   Estados prohibidos: {states_forbidden} ({error_rate:.2%})")
    
    # Análisis de convergencia
    print("\n4. Análisis de convergencia estadística...")
    results = convergence_analysis(circuit)
    for shots, probs in results.items():
        error = abs(probs['01'] - 0.5)
        print(f"   N={shots:5d}: P(01)={probs['01']:.4f}, Error={error:.4f}")
    
    # Visualización
    print("\n5. Generando gráficos...")
    plot_results(counts_ideal, counts_noisy)
    plot_convergence(results)
    
    print("\n" + "=" * 60)
    print("ANÁLISIS COMPLETADO")
    print("=" * 60)

if __name__ == "__main__":
    main()
```

### Ejemplo 2: Comparación Multi-Backend (Qiskit)

```python
"""
Comparación de resultados entre diferentes backends de Qiskit
"""

from qiskit import QuantumCircuit, transpile
from qiskit_aer import AerSimulator
from qiskit_ibm_runtime.fake_provider import (
    FakeMontreal, FakeSingapore, FakeToronto, FakeManila
)
import matplotlib.pyplot as plt

def compare_backends():
    """Compara mismo circuito en múltiples backends"""
    
    # Crear circuito singlete
    circuit = QuantumCircuit(2, 2)
    circuit.x(0)
    circuit.x(1)
    circuit.h(0)
    circuit.cx(0, 1)
    circuit.measure([0, 1], [0, 1])
    
    # Lista de backends
    backends = {
        'Ideal': AerSimulator(),
        'Montreal': FakeMontreal(),
        'Singapore': FakeSingapore(),
        'Toronto': FakeToronto(),
        'Manila': FakeManila()
    }
    
    # Ejecutar en todos
    results = {}
    for name, backend in backends.items():
        print(f"Ejecutando en {name}...")
        
        # Transpilar (importante!)
        transpiled = transpile(circuit, backend, optimization_level=2)
        
        # Ejecutar
        job = backend.run(transpiled, shots=10000)
        counts = job.result().get_counts()
        
        # Guardar resultados
        results[name] = counts
    
    # Graficar
    fig, axes = plt.subplots(2, 3, figsize=(18, 10))
    axes = axes.flatten()
    
    for idx, (name, counts) in enumerate(results.items()):
        if idx >= len(axes):
            break
            
        # Calcular probabilidades
        total = sum(counts.values())
        states = ['00', '01', '10', '11']
        probs = [counts.get(state, 0)/total for state in states]
        
        # Colorear: azul=permitido, rojo=prohibido
        colors = ['red', 'blue', 'blue', 'red']
        
        # Graficar
        axes[idx].bar(states, probs, color=colors, alpha=0.7)
        axes[idx].set_title(f'{name}', fontsize=14, fontweight='bold')
        axes[idx].set_ylabel('Probabilidad')
        axes[idx].set_ylim(0, 0.6)
        axes[idx].axhline(y=0.5, color='green', linestyle='--', alpha=0.5)
        
        # Agregar texto con error
        error = counts.get('00', 0) + counts.get('11', 0)
        error_rate = error / total
        axes[idx].text(0.5, 0.55, f'Error: {error_rate:.2%}', 
                      ha='center', fontsize=12, color='red')
    
    # Ocultar subplot extra si hay
    if len(results) < len(axes):
        axes[-1].axis('off')
    
    plt.tight_layout()
    plt.savefig('backend_comparison.png', dpi=300)
    plt.show()
    
    # Tabla de resultados
    print("\n" + "=" * 70)
    print(f"{'Backend':<15} {'P(01)':<10} {'P(10)':<10} {'Error':<10} {'Qubits Usados'}")
    print("=" * 70)
    
    for name, counts in results.items():
        total = sum(counts.values())
        p_01 = counts.get('01', 0) / total
        p_10 = counts.get('10', 0) / total
        error = (counts.get('00', 0) + counts.get('11', 0)) / total
        
        # Obtener qubits usados (si está transpilado)
        backend = backends[name]
        transpiled = transpile(circuit, backend)
        qubits = transpiled.qubits if hasattr(transpiled, 'qubits') else "N/A"
        
        print(f"{name:<15} {p_01:<10.4f} {p_10:<10.4f} {error:<10.2%} {str(qubits)}")
    
    print("=" * 70)

if __name__ == "__main__":
    compare_backends()
```

### Ejemplo 3: Estado Singlete en Amazon Braket

```python
"""
Generación del estado singlete usando Amazon Braket
"""

from braket.circuits import Circuit
from braket.devices import LocalSimulator
import matplotlib.pyplot as plt
import numpy as np

def create_singlet_braket():
    """Crea circuito singlete en Braket"""
    circuit = Circuit()
    
    # Compuertas (sintaxis Braket)
    circuit.x(0)
    circuit.x(1)
    circuit.h(0)
    circuit.cnot(0, 1)
    
    return circuit

def run_and_analyze():
    """Ejecuta y analiza resultados"""
    
    # Crear circuito
    circuit = create_singlet_braket()
    print("Circuito creado:")
    print(circuit)
    
    # Definir dispositivo
    device = LocalSimulator()
    
    # Ejecutar con diferentes valores de shots
    shot_values = [100, 1000, 10000]
    
    for shots in shot_values:
        print(f"\n--- Ejecutando con {shots} shots ---")
        
        # Ejecutar
        task = device.run(circuit, shots=shots)
        result = task.result()
        counts = result.measurement_counts
        
        # Calcular probabilidades
        total = sum(counts.values())
        print(f"Resultados: {counts}")
        
        for state, count in counts.items():
            prob = count / total
            print(f"  P({state}) = {prob:.4f}")
    
    # Gráfico de barras
    task = device.run(circuit, shots=10000)
    counts = task.result().measurement_counts
    
    states = list(counts.keys())
    frequencies = list(counts.values())
    
    plt.figure(figsize=(10, 6))
    plt.bar(states, frequencies, color=['red' if s in ['00', '11'] else 'blue' 
                                         for s in states])
    plt.xlabel('Estado Medido', fontsize=12)
    plt.ylabel('Frecuencia', fontsize=12)
    plt.title('Estado Singlete - Amazon Braket (10000 shots)', fontsize=14)
    plt.axhline(y=5000, color='green', linestyle='--', 
                label='Esperado (50%)', linewidth=2)
    plt.legend()
    plt.grid(axis='y', alpha=0.3)
    plt.tight_layout()
    plt.show()

if __name__ == "__main__":
    run_and_analyze()
```

---

## Glosario de Términos Técnicos

**Backend:** Dispositivo (simulador o hardware) donde se ejecutan los circuitos cuánticos.

**Braket:** SDK de Amazon Web Services para computación cuántica.

**Counts:** Diccionario con frecuencias de cada resultado de medición.

**Depolarizing error:** Tipo de ruido donde el qubit pierde información cuántica completamente.

**Fake provider:** Simuladores de Qiskit que emulan hardware real de IBM con modelos de ruido.

**Job:** Objeto que representa una ejecución de circuito en cola o en progreso.

**LocalSimulator:** Simulador que corre en tu computadora local (no en la nube).

**NoiseModel:** Conjunto de errores cuánticos asociados a compuertas y mediciones.

**Qiskit:** SDK de código abierto de IBM para computación cuántica.

**Shots:** Número de veces que se ejecuta un circuito para obtener estadísticas.

**Task:** En Braket, equivalente a "Job" de Qiskit.

**Transpilación:** Traducción de circuito lógico a compuertas nativas del hardware.

**Unitaria:** Matriz que preserva norma; representa evolución cuántica reversible.

---

## Para la Próxima Clase

### Checklist de Preparación

- [ ] Anaconda instalado y funcionando
- [ ] Entorno virtual creado (qiskit_env o similar)
- [ ] Qiskit instalado (versión ≥1.0)
- [ ] Amazon Braket instalado (opcional pero recomendado)
- [ ] Jupyter Notebook funcionando
- [ ] Ejemplos de Clase 5 reproducidos exitosamente
- [ ] Cuenta de IBM Quantum creada (opcional, para hardware real)
- [ ] Lectura de Nielsen & Chuang Cap. 5.1-5.2 (Deutsch-Jozsa, Grover)

### Ejercicios Obligatorios

1. Implementar los 4 estados de Bell en Qiskit y Braket
2. Crear modelo de ruido personalizado y medir impacto
3. Comparar 3 backends diferentes (AerSimulator + 2 fake providers)
4. Graficar convergencia estadística para N = [10, 100, 1000, 10000]

### Conceptos a Refrescar

- Interferencia cuántica (constructiva/destructiva)
- Compuertas controladas (CNOT, Toffoli, general)
- Superposición uniforme (aplicar H a todos los qubits)
- Oráculo cuántico (función implementada como compuerta)

---

**Resumen preparado por:** Asistente IA Especializado en Computación Cuántica  
**Supervisión académica:** Dr. Federico Holik (IFLP-CONICET)  
**Curso:** Introducción a la Computación Cuántica 2025 - UNaHur  
**Última actualización:** 12 de noviembre de 2024  
**Versión:** 1.0 (completa con código ejecutable)

**Palabras clave:** Qiskit, Braket, estado singlete, transpilación, modelos de ruido, convergencia estadística, simuladores, backends, entrelazamiento, programación cuántica

**Tags:** #computación-cuántica #qiskit #braket #implementación #práctica #estado-singlete #ruido #transpilación #simuladores #clase5

---

## Agradecimientos

**Al Dr. Federico Holik** por su paciencia durante los problemas técnicos de la clase y por demostrar que el debugging es parte natural del proceso de desarrollo.

**A la comunidad de Qiskit y Braket** por mantener documentación excelente y ejemplos accesibles.

**A los estudiantes del curso** por sus preguntas que enriquecieron la clase y motivaron aclaraciones en este resumen.

---

**FIN DEL RESUMEN - CLASE 5**