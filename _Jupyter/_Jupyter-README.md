
# Entorno Jupyter

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

- ejecutar `jupyter lab` y abrir un cuaderno
```sh
cd # a la bóveda de Obsidian
conda activate ICC25 # nuevo prompt: (ICC25) ➜  ICC25-Holik git:(main) ✗
jupyter-lab # abre navegador
```

![[README.d/jupyter_lab_pantalla.png]]
1. abre navegador, apuntado a `127.0.0.1:8888`
	1. si no abre, en la `consola`se ve el URL para el navegador: `http://localhost:8889/lab?token=af3e...ba7f` (notar el puerto)
2. abrir carpeta
3. abrir cuaderno
4. editar celdas

## cuaderno Algebra-Lineal.ipynb

[SymPy](https://www.sympy.org/es/): "es una biblioteca de Python para matemáticas simbólicas. Su propósito es llegar a ser un sistema de álgebra por computadora (CAS) completo manteniendo el código tan simple como sea posible para poder ser legible y extensible de manera fácil. SymPy está escrito en Python enteramente."

Un número complejo se define por:

$$ z ∈ ℂ → z = a + bi $$
$$ con\ a,b ∈ ℝ $$
## cuaderno







