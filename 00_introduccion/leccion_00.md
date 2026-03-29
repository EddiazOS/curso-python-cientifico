# Lección 00 — Introducción e Instalación del Entorno de Trabajo

Bienvenido al curso de **Python Científico**. Esta lección te guiará paso a paso para instalar y configurar todo el entorno de trabajo necesario antes de comenzar con los módulos de análisis de datos, visualización y bioinformática.

---

## ¿Qué es Python Científico?

Python se ha convertido en el lenguaje estándar para la computación científica gracias a un ecosistema de librerías especializadas. A lo largo de este curso trabajaremos con las siguientes:

| Librería | Función principal |
|---|---|
| **NumPy** | Cómputo numérico y manejo de arreglos multidimensionales |
| **Pandas** | Manipulación y análisis de datos tabulares |
| **Matplotlib / Seaborn** | Visualización de datos |
| **SciPy** | Estadística, optimización y cómputo científico |
| **Biopython** | Bioinformática y biología computacional |

Todo el trabajo lo haremos dentro de **Jupyter Notebooks**, un entorno interactivo que permite combinar código, texto, ecuaciones y gráficas en un mismo documento.

---

## 1. Instalación de Miniconda

Usaremos **Miniconda** como gestor de entornos y paquetes. Es una versión ligera de Anaconda que incluye solo `conda` y Python.

### Windows

1. Descarga el instalador desde: https://docs.conda.io/en/latest/miniconda.html  
   → Elige la versión **Miniconda3 Windows 64-bit**.

2. Ejecuta el instalador `.exe` y sigue el asistente. En la pantalla de opciones avanzadas:
   - ✅ Marca **"Add Miniconda3 to my PATH environment variable"** (opcional pero recomendado).
   - ✅ Marca **"Register Miniconda3 as my default Python"**.

3. Abre el **Anaconda Prompt** (buscándolo en el menú de inicio) y verifica la instalación:

```bash
conda --version
```

### macOS

1. Descarga el instalador desde: https://docs.conda.io/en/latest/miniconda.html  
   → Elige **Miniconda3 macOS Apple Silicon (arm64)** si tienes un Mac con chip M1/M2/M3, o **macOS Intel (x86_64)** si tu Mac es anterior a 2020.

2. Abre la **Terminal** y navega a la carpeta de descargas:

```bash
cd ~/Downloads
bash Miniconda3-latest-MacOSX-arm64.sh   # cambia el nombre según el archivo descargado
```

3. Sigue las instrucciones del instalador. Acepta la licencia y confirma la ubicación de instalación. Al finalizar, escribe `yes` cuando pregunte si deseas inicializar conda.

4. Cierra y vuelve a abrir la Terminal, luego verifica:

```bash
conda --version
```

### Linux

1. Descarga el instalador desde la terminal:

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

2. Dale permisos de ejecución e instala:

```bash
chmod +x Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

3. Sigue las instrucciones. Al finalizar, ejecuta:

```bash
source ~/.bashrc
conda --version
```

---

## 2. Creación del Entorno Virtual

Un **entorno virtual** permite aislar las dependencias del curso sin afectar tu instalación de Python global. Este repositorio incluye el archivo `environment.yml` con todas las librerías necesarias.

### Clonar el repositorio

Si aún no tienes el repositorio en tu máquina, clónalo con:

```bash
git clone https://github.com/EddiazOS/curso-python-cientifico.git
cd curso-python-cientifico
```

### Crear el entorno desde `environment.yml`

```bash
conda env create -f environment.yml
```

Este comando leerá el archivo `environment.yml` e instalará automáticamente todas las librerías del curso (NumPy, Pandas, Matplotlib, SciPy, etc.).

### Activar el entorno

```bash
conda activate python-cientifico
```

> 💡 **Recuerda**: cada vez que abras una terminal nueva debes activar el entorno antes de trabajar.

### Desactivar el entorno

```bash
conda deactivate
```

---

## 3. Lanzar JupyterLab

Con el entorno activo, inicia JupyterLab desde la carpeta del repositorio:

```bash
jupyter lab
```

Esto abrirá automáticamente una ventana en tu navegador con la interfaz de JupyterLab. Desde allí puedes navegar entre los módulos del curso y abrir los notebooks (archivos `.ipynb`).

> Si prefieres la interfaz clásica de Jupyter Notebook, usa: `jupyter notebook`

---

## 4. Verificación del Entorno

Una vez dentro de JupyterLab, abre el archivo `00_introduccion/00_intro_python.ipynb` y ejecuta la siguiente celda para verificar que todas las librerías están correctamente instaladas:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import scipy
import sys

print(f"Python:     {sys.version}")
print(f"NumPy:      {np.__version__}")
print(f"Pandas:     {pd.__version__}")
print(f"SciPy:      {scipy.__version__}")
print("✅ ¡Entorno configurado correctamente!")
```

Si ves el mensaje `✅ ¡Entorno configurado correctamente!` sin errores, estás listo para comenzar el curso.

---

## 5. Estructura del Curso

```
curso-python-cientifico/
│
├── 00_introduccion/          ← Estás aquí
├── 01_numpy/
├── 02_pandas/
├── 03_matplotlib_seaborn/
├── 04_scipy/
├── 05_aplicaciones/          ← Bioinformática y biología computacional
├── datos/                    ← Datasets usados en el curso
├── environment.yml           ← Dependencias del entorno
└── README.md
```

---

## 6. Solución de Problemas Comunes

**`conda: command not found`**  
→ Cierra y vuelve a abrir la terminal. Si persiste, agrega manualmente conda al PATH o reinstala Miniconda.

**`PackagesNotFoundError` al crear el entorno**  
→ Ejecuta `conda update conda` y vuelve a intentar `conda env create -f environment.yml`.

**JupyterLab no abre en el navegador**  
→ Copia la URL que aparece en la terminal (con el token) y pégala manualmente en tu navegador.

**Kernel no disponible en el notebook**  
→ Asegúrate de tener el entorno activo antes de lanzar JupyterLab, o instala el kernel manualmente:
```bash
python -m ipykernel install --user --name python-cientifico --display-name "Python Científico"
```

---

*Módulo 00 — Curso de Python Científico | EddiazOS*
