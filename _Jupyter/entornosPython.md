---
theme: entornosPython
_class: lead
paginate: true
backgroundColor:
backgroundImage: url('./entornosPython.svg')
---

# Entorno Python para ICC25

- QC: **simulación** vs compu física
- entorno: **local** vs ⛈️
- entorno local: sistema vs **venv**
- distribución: Python.org vs **propietaria**


| <sub>(C) Federico Hernán Holik  y contribuyentes</sub> |
| ------------------------------------------------------ |
<sub>Licencias: [cc-by-sa-4.0](https://choosealicense.com/licenses/cc-by-sa-4.0/), </sub><sub>[GPLv3](https://choosealicense.com/licenses/gpl-3.0/)</sub>
<sub>Fuente: https://github.com/eterX/ICC25-Holik/blob/main/_Jupyter/entornosPython.md</sub>

---

## entorno: **local** vs ⛈️

| entorno | pro                    | con                                 |
| ------- | ---------------------- | ----------------------------------- |
| local   | - control de versiones | - recursos limitados<br>- localidad |
| ⛈️      | - sin instalación      | - costo directo<br>-                |

empate: colaboración


---

##  entorno local: sistema vs **venv**

sin dudas: entorno virtual por:
 - Distribución de SO  ⚠️
- Lenguaje interpretado ( 🔋 incluídas)
- Portable y a medida 👍
- en gColab se regenera en cada servidor  👎 

---
### simulación: cuadernos  Jupyter

https://jupyter.org/try-jupyter/lab/

- celdas Markdown y ejecutables
- kernel: Py, Cpp, R, SQLite, Octave
- archivos JSON
	- Markdown
	- ejecutables
	- **resultados**

---
### simulación: arquitectura Jupyter

![[blocks.png]]

- muchos cuadernos -> un kernel
- kernels variados
- Python: introspección, debugging

---

##  distribución: Python.org vs **propietaria** (1)

| Característica              | CPython (Oficial)          | Anaconda                               |
| --------------------------- | -------------------------- | -------------------------------------- |
| **Mantenedor**              | Python Software Foundation | Anaconda Inc. (comercial)              |
| **Licencia**                | Licencia PSF (FLOSS)       | BSD (nivel gratuito) + Comercial       |
| **Tamaño**                  | ~25-50 MB                  | ~3-5 GB (instalación completa)         |
| **Gestor de Paquetes**      | pip                        | conda (+ pip)                          |
| **Repositorio de Paquetes** | PyPI (~500 mil paquetes)   | Repositorio Anaconda (~8 mil paquetes) |
| **Público Objetivo**        | Propósito general          | CD/ML, científico, dominios            |




---

##  distribución: Python.org vs **propietaria** (2)

| Característica                 | CPython (Oficial)          | Anaconda                     |
| ------------------------------ | -------------------------- | ---------------------------- |
| **Bibliotecas Preinstaladas**  | Bibliotecas estándar       | NumPy, pandas, Jupyter, +250 |
| **Manejo de Binarios**         | Fuente + wheels            | Binarios precompilados       |
| **Entornos Virtuales**         | venv (stdlib 🔋)           | entornos conda               |
| **Multi-paradigma**            | Solo Python                | Python, R, Julia, etc.       |
| **Integración con el Sistema** | Instalación a nivel del SO | Autocontenido                |



---

##  distribución: Python.org vs **propietaria** (3)

| Característica                 | CPython (Oficial) | Anaconda                                |
| ------------------------------ | ----------------- | --------------------------------------- |
| **Resolución de Dependencias** | Básica (pip)      | Avanzada ($\neq$ solvers)               |
| **Velocidad (instalación)**    | Rápida (pip)      | Más lenta (conda)<br>Más rápida (mamba) |
| **Espacio en Disco**           | Mínimo            | Pesado                                  |
| **Filosofía FLOSS**            | FLOSS puro        | Mixta (paquetes comerciales)            |

---

## Anaconda: instalación M$ Windows

https://www.datacamp.com/es/tutorial/installing-anaconda-windows

---

## Anaconda: instalación Linux/MacO$

➡️ "siga, siga" ➡️

## instalacion

- instalar Conda  (distribución privativa de Python)
- crear entorno ICC25:

```sh
cd _Jupyter # desde la bóveda de Obsidian
conda env create --solver libmamba --file ICC25.yml --name ICC25
conda init
conda activate ICC25
```

>[!warn] posible solución de problemas
  --solver {classic,libmamba} 


---

## Anaconda: instalación Linux/MacO$

- ejecutar `jupyter lab` y abrir un cuaderno
```sh
cd # a la bóveda de Obsidian
conda activate ICC25 # nuevo prompt: (ICC25) ➜  ICC25-Holik git:(main) ✗
jupyter-lab # abre navegador
```


---

# Conclusiones


| entorno             | pro                                                | con                                   |
| ------------------- | -------------------------------------------------- | ------------------------------------- |
| local<br>python.org | - control de versiones                             | - recursos limitados<br>- localidad   |
| local<br>Anaconda   | - control de versiones<br>- entorno mas replicable | - recursos limitados<br>              |
| ⛈️                  | - sin instalación                                  | - costo directo<br>- colaboración(😣) |

**Preguntas? Gracias!**
