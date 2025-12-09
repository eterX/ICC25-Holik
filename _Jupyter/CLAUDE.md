# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a quantum computing course repository for "Introducción a la Computación Cuántica y Tecnologías Cuánticas" (Introduction to Quantum Computing and Quantum Technologies) taught by Dr. Federico Hernán Holik at UNaHur. The repository is structured as an Obsidian vault and contains Jupyter notebooks for quantum computing exercises and experiments using Qiskit and related libraries.

## Environment Setup

### Creating the Conda Environment

The project uses a Conda environment named `ICC25` with Python 3.12:

```bash
cd /Users/lbatlle/ICC25-Holik/_Jupyter
conda env create --solver libmamba --file ICC25.yml --name ICC25
conda init
conda activate ICC25
```

If environment creation fails, try using `--solver classic` instead of `--solver libmamba`.

### Updating the Environment

```bash
conda activate ICC25
conda env update --file ICC25.yml
```

Or to update all packages:

```bash
conda activate ICC25
conda update --all
```

### Running Jupyter Lab

```bash
cd /Users/lbatlle/ICC25-Holik
conda activate ICC25
jupyter lab
```

This will open a browser pointing to `http://localhost:8888` (or another port if 8888 is in use).

## Key Dependencies

The environment includes:
- **Python**: >=3.12, <3.13
- **Quantum Computing**: qiskit, qiskit_aer, qiskit-ibm-runtime, qiskit[visualization]
- **Scientific Computing**: numpy, sympy (via anaconda distribution)
- **Jupyter**: jupyter, jupyterlab, ipykernel, ipywidgets, jupyterlab-git
- **Utilities**: pylatexenc (for LaTeX rendering in Qiskit visualizations)

## Repository Structure

This is the `_Jupyter` subdirectory of the main ICC25-Holik repository:

- **Notebooks**:
  - `Algebra-Lineal.ipynb`: Linear algebra exercises with SymPy (complex numbers, vectors, matrices, tensor products)
  - `Parcial_UNAHUR.ipynb`: Exam notebook with quantum state calculations, Hamiltonian eigenvalues, and circuit implementations
  - `Parcial_UNAHUR-vacío.ipynb`: Empty template for the exam
  - `Qiskit_Ejemplos.ipynb`: Qiskit examples and demonstrations
  - `Mach-Zehnder.ipynb`: Mach-Zehnder interferometer simulations
  - `Singlet_State_Braket.ipynb`: Singlet state examples using Amazon Braket

- **Documentation**:
  - `Jupyter-README.md`: Setup instructions for Jupyter environment
  - `SDKs-qiskit-pennylane.md`: Important reference for Qiskit/PennyLane patterns and gotchas
  - `entornosPython.md`: Python environment comparison (CPython vs Anaconda)
  - `ICC25.yml`: Conda environment specification

- **Parent directories** (accessible via `..`):
  - `../_Teoria.d/`: Theory notes (Algebra.md, Fisica.md)
  - `../_Clases.d/`: Class materials and PDFs
  - `../_Bibliografia.d/`: Bibliography

## Working with Qiskit

### Critical Patterns from SDKs-qiskit-pennylane.md

**Important**: Always consult `SDKs-qiskit-pennylane.md` for Qiskit best practices. Key patterns:

#### 1. Saving State Vectors Before Measurement

```python
from qiskit_aer import AerSimulator

circuit = qk.QuantumCircuit(1, 1)
circuit.initialize(state_vector, 0)

# CRITICAL: save_statevector BEFORE measuring
circuit.save_statevector(label='my_sv')

# Now measure (this collapses the state)
circuit.measure_all()

# Use statevector simulator
backend = AerSimulator(method='statevector')
job = backend.run(circuit, shots=1000)
result = job.result()

# Extract saved state for algebraic operations
saved_state = result.data(0)['my_sv']
```

#### 2. Initializing Arbitrary States

```python
# Initialize with custom state vector
state = [np.sqrt(2/3), np.sqrt(1/3) * np.exp(1j * np.pi/3)]
circuit.initialize(state, 0)
```

#### 3. Common Quantum Operations

```python
# Base states (computational basis)
ket_zero = np.array([1, 0])
ket_one = np.array([0, 1])

# Hadamard basis
ket_plus = np.array([1/np.sqrt(2), 1/np.sqrt(2)])
ket_minus = np.array([1/np.sqrt(2), -1/np.sqrt(2)])

# Born rule for measurement probability
P_plus = np.abs(np.dot(np.conjugate(ket_plus), psi_vector))**2

# Projector
proyector_z = np.outer(ket_zero, np.conj(ket_zero))

# Kronecker product for multi-qubit operators
Z_2qubits = np.kron(sigma_z, sigma_z)
# Or with sympy:
Z_2qubits = sp.kronecker_product(sigma_z, sigma_z)

# Gate matrices
compuerta_h = qk.circuit.library.HGate().to_matrix()
```

### NumPy ↔ SymPy Conversions

```python
# NumPy to SymPy
numpy_array = np.array([[1/np.sqrt(2), 2], [3, np.sqrt(16) * np.exp(1j * np.pi/3)]])
sympy_matrix = sp.Matrix(numpy_array)

# SymPy to NumPy
numpy_array = np.array(sympy_matrix).astype(np.complex128)
```

### Validating Results

```python
# Verify real probabilities in [0,1]
error_redondeo = 1e-10
assert np.abs(probability.imag) < error_redondeo, "Probability must be real"
assert 0 <= probability.real <= 1, "Probability must be in [0,1]"
```

## Notebook Architecture

All notebooks follow this pattern:

1. **Import standard libraries**:
   ```python
   import sympy as sp
   import numpy as np
   import qiskit as qk
   from qiskit_aer import AerSimulator
   from IPython.display import display, Math
   ```

2. **Define quantum states symbolically** (when appropriate)
3. **Create and run circuits** with proper state saving
4. **Validate results** algebraically
5. **Visualize** with matplotlib/qiskit visualization tools

## Git Conventions

From `.gitignore`, the repository uses a special convention:
- **Only directories starting with `_*`** are tracked by git (e.g., `_Jupyter`, `_Teoria.d`, `_Clases.d`)
- Exceptions: `README.md`, `README.d/`, `.stignore`
- Personal/local work directories (without `_` prefix) are not tracked
- This allows each student to maintain personal notes alongside the official course materials

Ignored files include:
- `.ipynb_checkpoints/` and `.virtual_documents/` (Jupyter artifacts)
- `.obsidian/`, `.DS_Store` (editor/OS artifacts)
- `*.sync-conflict-*` (Syncthing conflicts)

## Course Context

This is an educational repository for a 10-week quantum computing course at UNaHur:
- **Schedule**: Tuesdays, 10:00-13:00 (Argentina time zone)
- **Evaluation**: Exams on specific dates in December (see `Parcial_UNAHUR.ipynb`)
- **Topics**: Pure quantum states, density matrices, Hamiltonians, quantum circuits, measurement, entanglement

## Common Tasks

### Running Tests/Verification
There is no formal test suite. Verification is done by:
1. Running notebook cells sequentially
2. Checking numerical results against analytical calculations
3. Validating assertions (e.g., `assert P_plus + P_minus == 1`)

### Creating a New Notebook
1. Activate the conda environment: `conda activate ICC25`
2. Launch Jupyter Lab: `jupyter lab`
3. Import standard libraries (numpy, sympy, qiskit, qiskit_aer)
4. Follow patterns from existing notebooks (especially state saving before measurement)

### Debugging Qiskit Issues
- If `save_statevector` is not found, ensure you're using `from qiskit_aer import AerSimulator` (not the old qiskit.Aer)
- Always use `method='statevector'` when creating the simulator
- Save state before measurement, not after
- Check `SDKs-qiskit-pennylane.md` for troubleshooting patterns
