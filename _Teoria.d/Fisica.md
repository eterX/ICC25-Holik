---
aliases:
  - Física
  - Física Cuántica
  - Física Clásica
---


# Física Clásica

---

# Física Cuántica

## Notación de Dirac

Extracto de [[Algebra#Notación de Dirac]]: ![[Algebra#Notación de Dirac]]



## Postulados de la Mecánica Cuántica

### Postulado 1: Espacio de Estados

**Enunciado (Inglés):**
Associated to any isolated physical system is a complex vector space with inner product (that is, a Hilbert space) known as the _state space_ of the system. The system is completely described by its _state vector_, which is a unit vector in the system's state space.

**Traducción:**
A todo sistema físico aislado se le asocia un espacio vectorial complejo con producto interno (esto es, un espacio de Hilbert) conocido como el _espacio de estados_ del sistema. El sistema está completamente descripto por su _vector de estado_, que es un vector unitario en el espacio de estados del sistema.

**Explicación:**
- El espacio de estados es matemáticamente un [[Algebra#Espacios de Hilbert|espacio de Hilbert]] ℋ sobre ℂ
- Para un qubit: ℋ = ℂ²
- Para n qubits: ℋ = ℂ^(2ⁿ) (producto tensorial de n copias de ℂ²)
- Condición de normalización: ⟨ψ|ψ⟩ = 1

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.2.1 "State space" (págs. 80-81)
- [[Alexei Yu. Kitaev/Classical and Quantum Computation - Alexei Yu. Kitaev|Kitaev et al.]] - Capítulo 2, Sección 2.1 "General definitions"
- Ver también: [[Algebra#Espacios de Hilbert]]


### Postulado 2: Evolución Temporal

**Enunciado (Inglés):**
The evolution of a _closed_ quantum system is described by a _unitary transformation_. That is, the state |_ψ_〉 of the system at time $t_1$ is related to the state |_ψ′_〉 of the system at time $t_2$ by a unitary operator $U$ which depends only on the times $t_1$ and $t_2$,
$$|\psi'\rangle = U|\psi\rangle \tag{NC 2.84}$$

**Traducción:**
La evolución de un sistema cuántico _cerrado_ está descripta por una _transformación unitaria_. Esto es, el estado |_ψ_〉 del sistema en el tiempo $t_1$ está relacionado con el estado |_ψ′_〉 del sistema en el tiempo $t_2$ mediante un operador unitario $U$ que depende únicamente de los tiempos $t_1$ y $t_2$,
$$|\psi'\rangle = U|\psi\rangle \tag{NC 2.84}$$

**Explicación:**
- Operador unitario: $U^\dagger U = U U^\dagger = I$
- Preserva el producto interno: ⟨ψ|φ⟩ = ⟨Uψ|Uφ⟩
- Conserva la normalización: ||ψ|| = ||Uψ||
- La evolución es reversible: $U^{-1} = U^\dagger$

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.2.2 "Evolution" (págs. 81-84)
- [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong|Wong]] - Capítulo sobre operadores unitarios
- Ver también: [[Algebra#Operadores Unitarios]]


#### Postulado 2bis: Ecuación de Schrödinger

**Enunciado (forma dependiente del tiempo):**
$$i\hbar \frac{\partial}{\partial t}|\psi(t)\rangle = \hat{H}|\psi(t)\rangle \tag{NC 2.86}$$

**Traducción y explicación:**
La ecuación de Schrödinger describe la evolución temporal continua de un estado cuántico, donde:
- $\hbar = h/(2\pi) \approx 1.055 \times 10^{-34}$ J·s (constante de Planck reducida)
- $\hat{H}$: operador Hamiltoniano (energía total del sistema)
- $i$: unidad imaginaria

**Solución formal:**
$$|\psi(t)\rangle = \hat{U}(t)|\psi(0)\rangle$$

donde $\hat{U}(t) = e^{-i\hat{H}t/\hbar}$ es el operador de evolución temporal.

**Propiedades de U(t):**
- $U(0) = I$ (identidad en t=0)
- $U^\dagger(t)U(t) = I$ (unitario, preserva norma)
- $U(t_1)U(t_2) = U(t_1+t_2)$ (propiedad de grupo)

**Interpretación física:**
- En ausencia de mediciones, el sistema evoluciona unitariamente
- La evolución es determinista a nivel del vector de estado
- La probabilidad emerge en la medición, no en la evolución
- Las compuertas cuánticas son casos discretos de esta evolución continua

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.2.2 (ecuación 2.86)
- [[Alexei Yu. Kitaev/Classical and Quantum Computation - Alexei Yu. Kitaev|Kitaev et al.]] - Discusión de evolución unitaria


### Postulado 3: Medición Cuántica

**Enunciado (Inglés):**
Quantum measurements are described by a collection $\{M_m\}$ of _measurement operators_. These are operators acting on the state space of the system being measured. The index _m_ refers to the measurement outcomes that may occur in the experiment. If the state of the quantum system is |_ψ_〉 immediately before the measurement then the probability that result _m_ occurs is given by:
$$p(m) = \langle\psi|M_m^\dagger M_m|\psi\rangle \tag{NC 2.87}$$

**Traducción:**
Las mediciones cuánticas están descriptas por una colección $\{M_m\}$ de _operadores de medición_. Estos son operadores que actúan sobre el espacio de estados del sistema que se está midiendo. El índice _m_ se refiere a los resultados de medición que pueden ocurrir en el experimento. Si el estado del sistema cuántico es |_ψ_〉 inmediatamente antes de la medición, entonces la probabilidad de que ocurra el resultado _m_ está dada por:
$$p(m) = \langle\psi|M_m^\dagger M_m|\psi\rangle \tag{NC 2.87}$$

**Estado después de la medición:**
$$|\psi'\rangle = \frac{M_m|\psi\rangle}{\sqrt{\langle\psi|M_m^\dagger M_m|\psi\rangle}} \tag{NC 2.88}$$

**Condición de completitud:**
$$\sum_m M_m^\dagger M_m = I$$

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.2.3 "Quantum measurement" (págs. 84-92)
- [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong|Wong]] - Capítulo 6 "Quantum Measurement"


#### Medición Proyectiva (caso especial)

**Definición:**
Una medición proyectiva está caracterizada por un observable (operador hermitiano) $M$ con descomposición espectral:
$$M = \sum_m m P_m$$

donde:
- $m$ son los autovalores (resultados posibles de medición)
- $P_m$ son proyectores ortogonales ($P_m = P_m^\dagger = P_m^2$)
- $P_m P_{m'} = \delta_{mm'} P_m$

**Regla de Born:**
La probabilidad de obtener el resultado $m$ al medir el observable $M$ en el estado $|\psi\rangle$ es:
$$p(m) = \langle\psi|P_m|\psi\rangle = ||P_m|\psi\rangle||^2$$

**Estado después de la medición proyectiva:**
$$|\psi'\rangle = \frac{P_m|\psi\rangle}{\sqrt{\langle\psi|P_m|\psi\rangle}}$$

**Ejemplo - Medición en la base computacional:**
Para un qubit, medir en la base $\{|0\rangle, |1\rangle\}$:
- $P_0 = |0\rangle\langle 0|$
- $P_1 = |1\rangle\langle 1|$
- Si $|\psi\rangle = \alpha|0\rangle + \beta|1\rangle$:
  - $p(0) = |\alpha|^2$
  - $p(1) = |\beta|^2$

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.2.5 "Projective measurements"
- Ver también: [[Algebra#Proyectores]]


### Postulado 4: Sistemas Compuestos

**Enunciado (Inglés):**
The state space of a composite physical system is the tensor product of the state spaces of the component physical systems. Moreover, if we have systems numbered 1 through n, and system number i is prepared in the state |ψ_i〉, then the joint state of the total system is |ψ_1〉 ⊗ |ψ_2〉 ⊗ ⋯ ⊗ |ψ_n〉.

**Traducción:**
El espacio de estados de un sistema físico compuesto es el producto tensorial de los espacios de estados de los sistemas físicos componentes. Además, si tenemos sistemas numerados del 1 al n, y el sistema número i está preparado en el estado |ψ_i〉, entonces el estado conjunto del sistema total es |ψ_1〉 ⊗ |ψ_2〉 ⊗ ⋯ ⊗ |ψ_n〉.

**Explicación matemática:**
- Si el sistema A tiene espacio de estados ℋ_A y el sistema B tiene ℋ_B
- El sistema compuesto A+B tiene espacio de estados ℋ_A ⊗ ℋ_B
- Dimensión: dim(ℋ_A ⊗ ℋ_B) = dim(ℋ_A) × dim(ℋ_B)

**Ejemplo - Dos qubits:**
- Sistema 1: ℋ₁ = ℂ² (base {|0⟩, |1⟩})
- Sistema 2: ℋ₂ = ℂ² (base {|0⟩, |1⟩})
- Sistema compuesto: ℋ₁⊗ℋ₂ = ℂ⁴ (base {|00⟩, |01⟩, |10⟩, |11⟩})

**Estados producto vs estados entrelazados:**
- Estado producto: $|\psi\rangle = |\psi_A\rangle \otimes |\psi_B\rangle$ (separable)
- Estado entrelazado: no puede escribirse como producto (ejemplo: Bell state $\frac{1}{\sqrt{2}}(|00\rangle + |11\rangle)$)

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.1.7 "Tensor products" y Sección 2.2.4
- [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong|Wong]] - Capítulo 5 "Tensor Products"
- [[Jeffery Bub/Entrelazamiento cuantico e informacion - Jeffery Bub|Bub]] - Artículo sobre entrelazamiento cuántico
- Ver también: [[Algebra#Producto Tensorial]]


---

## Observables y Medición

### Operadores Hermíticos (Observables)

**Definición:**
Un operador $A$ es hermítico (o autoadjunto) si:
$$A = A^\dagger$$

**Propiedades fundamentales:**
1. Los autovalores son reales
2. Autovectores correspondientes a autovalores distintos son ortogonales
3. Admite descomposición espectral: $A = \sum_a a|a\rangle\langle a|$

**Interpretación física:**
- Los observables físicos (posición, momento, energía, spin) se representan como operadores hermíticos
- Los autovalores representan los posibles resultados de medición
- Los autovectores son los estados en los cuales el observable tiene valor definido

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.1.5 "Hermitian operators"
- Ver también: [[Algebra#Operadores Hermíticos]]

---

## Principios Adicionales

### Principio de Superposición

Si $|\psi_1\rangle$ y $|\psi_2\rangle$ son estados posibles del sistema, entonces cualquier combinación lineal normalizada
$$|\psi\rangle = \alpha|\psi_1\rangle + \beta|\psi_2\rangle, \quad |\alpha|^2 + |\beta|^2 = 1$$
también es un estado posible del sistema.

**Interpretación:**
- Este principio distingue fundamentalmente la mecánica cuántica de la física clásica
- Un qubit puede estar en superposición de |0⟩ y |1⟩ simultáneamente
- La medición "fuerza" al sistema a colapsar a uno de los estados base

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Discusión conceptual en Capítulo 1
- [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong|Wong]] - Introducción al principio de superposición
- Ver también: [[Algebra#Combinaciones Lineales]]


### Colapso del Estado (interpretación de Copenhague)

Después de una medición que arroja resultado $m$, el estado del sistema "colapsa" al autoestado correspondiente a ese resultado.

**Nota:** Esta es solo una de varias interpretaciones de la mecánica cuántica. Otras interpretaciones (muchos mundos, variables ocultas, etc.) dan descripciones diferentes del proceso de medición.

**Referencias:**
- [[Federico Holik/Teoria de la informacion de Claude E. Shannon (4)/Teoria de la informacion de Claude E. Shan - Federico Holik|Holik]] - Discusiones sobre interpretaciones de la mecánica cuántica


---


## Estados Puros y Estados Mixtos

### Estados Puros

**Definición:**
Un estado cuántico es _puro_ cuando el sistema está completamente descripto por un único vector de estado $|\psi\rangle$ en el espacio de Hilbert. El sistema posee conocimiento completo (máximo posible) sobre su preparación.

**Caracterización matemática:**
$$|\psi\rangle \in \mathcal{H}, \quad \langle\psi|\psi\rangle = 1$$

**Ejemplos:**
- Qubit en estado $|0\rangle$
- Qubit en superposición $\frac{1}{\sqrt{2}}(|0\rangle + |1\rangle)$
- Estado de Bell $\frac{1}{\sqrt{2}}(|00\rangle + |11\rangle)$ para dos qubits

**Propiedades:**
- Representan el máximo conocimiento cuántico posible sobre el sistema
- La incertidumbre proviene únicamente de la naturaleza probabilística de la mecánica cuántica
- No hay ignorancia clásica adicional sobre qué estado puro describe el sistema

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.4 "Density operator" (págs. 98-105)
- [[Alexei Yu. Kitaev/Classical and Quantum Computation - Alexei Yu. Kitaev|Kitaev et al.]] - Capítulo 2


### Estados Mixtos

**Definición:**
Un estado cuántico es _mixto_ cuando existe ignorancia clásica sobre cuál vector de estado puro describe el sistema. El sistema se describe mediante un _ensamble estadístico_ de estados puros $\{(p_i, |\psi_i\rangle)\}$ donde $p_i$ es la probabilidad clásica de que el sistema esté en el estado $|\psi_i\rangle$.

**Caracterización mediante ensamble:**
$$\text{Ensamble: } \{(p_1, |\psi_1\rangle), (p_2, |\psi_2\rangle), \ldots, (p_n, |\psi_n\rangle)\}$$

con:
- $p_i \geq 0$ (probabilidades no negativas)
- $\sum_i p_i = 1$ (normalización)
- $|\psi_i\rangle$ estados puros (no necesariamente ortogonales)

**Origen de estados mixtos:**

1. **Ignorancia sobre la preparación:** No sabemos con certeza en qué estado puro fue preparado el sistema
   - Ejemplo: una fuente cuántica produce $|0\rangle$ con probabilidad 0.7 y $|1\rangle$ con probabilidad 0.3

2. **Subsistemas de estados entrelazados:** Al considerar un subsistema de un sistema compuesto entrelazado, el subsistema se describe por un estado mixto
   - Ejemplo: si dos qubits están en el estado de Bell $\frac{1}{\sqrt{2}}(|00\rangle + |11\rangle)$, cada qubit individualmente está en un estado mixto

3. **Decoherencia:** Interacción con el entorno transforma estados puros en mixtos

**Diferencia crucial con superposiciones:**
- **Superposición (estado puro):** $|\psi\rangle = \frac{1}{\sqrt{2}}(|0\rangle + |1\rangle)$ exhibe efectos de interferencia
- **Mezcla estadística (estado mixto):** probabilidad 0.5 de $|0\rangle$ y 0.5 de $|1\rangle$ NO exhibe interferencia

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.4.1-2.4.2 (págs. 98-102)
- [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong|Wong]] - Discusión de estados mixtos
- [[Jeffery Bub/Entrelazamiento cuantico e informacion - Jeffery Bub|Bub]] - Secciones sobre reducción a subsistemas


---

## Matriz Densidad (Operador Densidad)

### Definición

La **matriz densidad** (u operador densidad) $\rho$ es una descripción matemática unificada de estados cuánticos que engloba tanto estados puros como mixtos.

**Para un estado puro** $|\psi\rangle$:
$$\rho = |\psi\rangle\langle\psi| \tag{estado puro}$$

**Para un estado mixto** descrito por el ensamble $\{(p_i, |\psi_i\rangle)\}$:
$$\rho = \sum_i p_i |\psi_i\rangle\langle\psi_i| \tag{estado mixto}$$

**Notación alternativa:**
En algunos textos se denota como $\hat{\rho}$ o simplemente como el "operador de estado".


### Propiedades Fundamentales de $\rho$

La matriz densidad satisface las siguientes propiedades características:

#### 1. Hermiticidad
$$\rho = \rho^\dagger$$

**Consecuencia:** Todos los autovalores de $\rho$ son reales.

#### 2. Positividad (Semidefinida positiva)
$$\langle\phi|\rho|\phi\rangle \geq 0 \quad \forall |\phi\rangle \in \mathcal{H}$$

**Equivalentemente:** Todos los autovalores de $\rho$ son no negativos: $\lambda_i \geq 0$.

**Interpretación:** Los autovalores pueden interpretarse como probabilidades.

#### 3. Traza Unitaria
$$\text{Tr}(\rho) = 1$$

**Justificación:** La suma de todas las probabilidades debe ser 1.

**Cálculo explícito:**
$$\text{Tr}(\rho) = \text{Tr}\left(\sum_i p_i |\psi_i\rangle\langle\psi_i|\right) = \sum_i p_i \text{Tr}(|\psi_i\rangle\langle\psi_i|) = \sum_i p_i \cdot 1 = 1$$

#### 4. Criterio de Pureza: $\text{Tr}(\rho^2)$

**Para estados puros:**
$$\text{Tr}(\rho^2) = 1 \quad \Leftrightarrow \quad \rho^2 = \rho$$

**Para estados mixtos:**
$$\text{Tr}(\rho^2) < 1$$

**Demostración (estado puro):**
Si $\rho = |\psi\rangle\langle\psi|$, entonces:
$$\rho^2 = (|\psi\rangle\langle\psi|)(|\psi\rangle\langle\psi|) = |\psi\rangle\langle\psi|\psi\rangle\langle\psi| = |\psi\rangle\langle\psi| = \rho$$

Por lo tanto:
$$\text{Tr}(\rho^2) = \text{Tr}(\rho) = 1$$

**Pureza generalizada:**
$$\gamma(\rho) = \text{Tr}(\rho^2)$$

- $\gamma = 1$: estado puro
- $\gamma < 1$: estado mixto
- $\gamma = 1/d$ (donde $d = \dim \mathcal{H}$): estado maximalmente mixto

#### 5. Descomposición Espectral

Como $\rho$ es hermitiano, admite descomposición espectral:
$$\rho = \sum_i \lambda_i |i\rangle\langle i|$$

donde:
- $\lambda_i \geq 0$ (autovalores no negativos)
- $\sum_i \lambda_i = 1$ (traza unitaria)
- $|i\rangle$ son autovectores ortonormales

**Interpretación:** Los autovalores $\lambda_i$ pueden verse como probabilidades de encontrar el sistema en el autoestado $|i\rangle$.


### Cálculo de Probabilidades y Valores Esperados

#### Probabilidades de Medición

Para una medición proyectiva con proyectores $\{P_m\}$, la probabilidad de obtener el resultado $m$ es:
$$p(m) = \text{Tr}(P_m \rho) \tag{NC 2.117}$$

**Verificación para estado puro:**
Si $\rho = |\psi\rangle\langle\psi|$:
$$p(m) = \text{Tr}(P_m |\psi\rangle\langle\psi|) = \langle\psi|P_m|\psi\rangle$$

que coincide con la regla de Born del Postulado 3.

#### Valor Esperado de un Observable

Para un observable $M$ (operador hermitiano):
$$\langle M \rangle = \text{Tr}(M \rho) \tag{NC 2.118}$$

**Demostración:**
$$\langle M \rangle = \sum_i p_i \langle\psi_i|M|\psi_i\rangle = \sum_i p_i \text{Tr}(M |\psi_i\rangle\langle\psi_i|) = \text{Tr}\left(M \sum_i p_i |\psi_i\rangle\langle\psi_i|\right) = \text{Tr}(M\rho)$$


### Estado Post-Medición

Después de una medición con operadores $\{M_m\}$ que arroja resultado $m$, el estado se actualiza según:
$$\rho' = \frac{M_m \rho M_m^\dagger}{\text{Tr}(M_m \rho M_m^\dagger)} \tag{NC 2.119}$$

**Caso especial (medición proyectiva):**
$$\rho' = \frac{P_m \rho P_m}{\text{Tr}(P_m \rho)}$$


### Ejemplos Específicos

#### Ejemplo 1: Qubit en estado puro $|0\rangle$

$$\rho = |0\rangle\langle 0| = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$$

**Verificación de propiedades:**
- Hermitiana: $\rho = \rho^\dagger$ ✓
- Traza: $\text{Tr}(\rho) = 1 + 0 = 1$ ✓
- Pureza: $\rho^2 = \rho$, entonces $\text{Tr}(\rho^2) = 1$ ✓ (estado puro)

#### Ejemplo 2: Estado mixto equiprobable

Sistema preparado con igual probabilidad en $|0\rangle$ o $|1\rangle$:
$$\rho = \frac{1}{2}|0\rangle\langle 0| + \frac{1}{2}|1\rangle\langle 1| = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} + \frac{1}{2}\begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = \frac{I}{2}$$

**Verificación:**
- $\text{Tr}(\rho) = \frac{1}{2}(1+1) = 1$ ✓
- $\rho^2 = \frac{I}{4}$, entonces $\text{Tr}(\rho^2) = \frac{1}{2} < 1$ ✓ (estado mixto)
- Este es el **estado maximalmente mixto** para un qubit

#### Ejemplo 3: Comparación superposición vs mezcla

**Estado puro (superposición):**
$$|\psi\rangle = \frac{1}{\sqrt{2}}(|0\rangle + |1\rangle)$$
$$\rho_{\text{puro}} = |\psi\rangle\langle\psi| = \frac{1}{2}\begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix}$$

**Estado mixto:**
$$\rho_{\text{mixto}} = \frac{1}{2}|0\rangle\langle 0| + \frac{1}{2}|1\rangle\langle 1| = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$$

**Diferencia clave:** Los elementos fuera de la diagonal (coherencias) son no nulos en el estado puro pero cero en el mixto. Estas coherencias son responsables de los efectos de interferencia cuántica.


### Evolución Temporal de $\rho$

Para un sistema cerrado con evolución unitaria $U$:
$$\rho(t) = U\rho(0)U^\dagger \tag{NC 2.120}$$

**Demostración:**
Si $\rho(0) = \sum_i p_i |\psi_i(0)\rangle\langle\psi_i(0)|$ y cada $|\psi_i(t)\rangle = U|\psi_i(0)\rangle$:
$$\rho(t) = \sum_i p_i |\psi_i(t)\rangle\langle\psi_i(t)| = \sum_i p_i U|\psi_i(0)\rangle\langle\psi_i(0)|U^\dagger = U\rho(0)U^\dagger$$

**Ecuación de von Neumann:**
Forma diferencial análoga a la ecuación de Schrödinger:
$$i\hbar \frac{d\rho}{dt} = [H, \rho] = H\rho - \rho H \tag{NC 2.121}$$

donde $[H, \rho]$ es el conmutador de $H$ y $\rho$.


### Traza Parcial: Reducción a Subsistemas

Para un sistema compuesto AB con matriz densidad $\rho_{AB}$, la matriz densidad del subsistema A se obtiene mediante la **traza parcial** sobre B:
$$\rho_A = \text{Tr}_B(\rho_{AB}) \tag{NC 2.122}$$

**Definición explícita:**
Si $\{|i_B\rangle\}$ es una base ortonormal del espacio de Hilbert de B:
$$\rho_A = \sum_i (I_A \otimes \langle i_B|) \rho_{AB} (I_A \otimes |i_B\rangle)$$

**Ejemplo: Estado de Bell**
Para el estado entrelazado $|\Psi\rangle = \frac{1}{\sqrt{2}}(|00\rangle + |11\rangle)$:
$$\rho_{AB} = |\Psi\rangle\langle\Psi| = \frac{1}{2}(|00\rangle\langle 00| + |00\rangle\langle 11| + |11\rangle\langle 00| + |11\rangle\langle 11|)$$

La traza parcial sobre B da:
$$\rho_A = \text{Tr}_B(\rho_{AB}) = \frac{1}{2}(|0\rangle\langle 0| + |1\rangle\langle 1|) = \frac{I}{2}$$

**Conclusión:** Aunque el estado conjunto es puro, cada subsistema está en un estado mixto maximalmente mezclado. Este es el origen cuántico de estados mixtos por entrelazamiento.

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.4.3 "Reduced density operator" (págs. 103-105)
- Ver también: [[Algebra#Traza Parcial]]


### Tabla Resumen: Propiedades de $\rho$

| Propiedad | Expresión Matemática | Significado |
|-----------|---------------------|-------------|
| **Hermiticidad** | $\rho = \rho^\dagger$ | Autovalores reales |
| **Positividad** | $\langle\phi\|\rho\|\phi\rangle \geq 0$ | Autovalores no negativos |
| **Traza unitaria** | $\text{Tr}(\rho) = 1$ | Normalización probabilística |
| **Pureza** | $\text{Tr}(\rho^2) = 1$ (puro) | Criterio de distinción |
| | $\text{Tr}(\rho^2) < 1$ (mixto) | entre puros y mixtos |
| **Descomposición espectral** | $\rho = \sum_i \lambda_i \|i\rangle\langle i\|$ | $\lambda_i \geq 0$, $\sum_i \lambda_i = 1$ |
| **Probabilidad medición** | $p(m) = \text{Tr}(P_m \rho)$ | Regla generalizada de Born |
| **Valor esperado** | $\langle M \rangle = \text{Tr}(M\rho)$ | Cálculo de observables |
| **Evolución unitaria** | $\rho(t) = U\rho(0)U^\dagger$ | Dinámica cerrada |
| **Ecuación de von Neumann** | $i\hbar \frac{d\rho}{dt} = [H, \rho]$ | Forma diferencial |


### Ventajas del Formalismo de Matriz Densidad

1. **Descripción unificada:** Trata estados puros y mixtos en un mismo marco matemático
2. **Subsistemas:** Permite describir subsistemas de sistemas entrelazados vía traza parcial
3. **Sistemas abiertos:** Fundamental para tratar decoherencia e interacción con el entorno
4. **Información cuántica:** Base para definir entropía de von Neumann y otras medidas de información
5. **Cálculos simplificados:** La fórmula $\text{Tr}(M\rho)$ para valores esperados es a menudo más simple que trabajar con vectores de estado

**Referencias:**
- [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|Nielsen & Chuang]] - Sección 2.4 completa (págs. 98-112)
- [[Alexei Yu. Kitaev/Classical and Quantum Computation - Alexei Yu. Kitaev|Kitaev et al.]] - Capítulo 2
- [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong|Wong]] - Capítulo sobre matriz densidad
- Ver también: [[Algebra#Operadores de Densidad]]


---
