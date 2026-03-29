# 🐍 Curso de Python Científico para Ciencias Exactas

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Duración](https://img.shields.io/badge/Duración-10%20semanas-orange)]()
[![Nivel](https://img.shields.io/badge/Nivel-Principiante-brightgreen)]()

Curso estructurado de **Python Científico** dirigido a estudiantes de pregrado de la Facultad de Ciencias Exactas (Química y Biología) **sin experiencia previa en programación**. El curso se desarrolla en dos fases: primero se construye una base sólida en programación y computación científica con Python, y luego se aplica ese conocimiento en problemas reales de química y biología.

---

## 🎯 Objetivos Generales

- Desarrollar competencias básicas en programación con Python desde cero.
- Dominar las herramientas del ecosistema científico de Python (NumPy, Pandas, Matplotlib, SciPy).
- Resolver problemas matemáticos y científicos mediante simulación, álgebra lineal, estadística y ecuaciones diferenciales.
- Aplicar Python como herramienta de análisis en contextos reales de Química y Biología Molecular.

---

## 👥 Público Objetivo

Estudiantes de pregrado de la Facultad de Ciencias Exactas (Química, Biología o áreas afines) que deseen incorporar Python como herramienta científica en su formación académica e investigativa. **No se requieren conocimientos previos de programación.**

---

## 🗓️ Estructura del Curso

El curso tiene una duración de **10 semanas con 2 sesiones por semana (20 sesiones en total)**, organizado en dos grandes fases.

---

### 🔵 FASE 1 — Fundamentos de Python Científico (Semanas 1–6)

Esta fase construye las bases de programación y computación científica necesarias para abordar problemas en ciencias exactas.

| Semana | Sesión | Tema | Módulo |
|--------|--------|------|--------|
| 1 | 1 | Introducción a la programación y entorno de trabajo (Jupyter, Conda) | `00_introduccion` |
| 1 | 2 | Variables, tipos de datos, operadores y estructuras de control | `00_introduccion` |
| 2 | 3 | Funciones, módulos y buenas prácticas en Python | `00_introduccion` |
| 2 | 4 | Arreglos numéricos con NumPy: creación, indexación y operaciones | `01_numpy` |
| 3 | 5 | Álgebra lineal con NumPy: matrices, sistemas de ecuaciones, eigenvalores | `01_numpy` |
| 3 | 6 | Manipulación de datos tabulares con Pandas | `02_pandas` |
| 4 | 7 | Limpieza, filtrado y agrupación de datos con Pandas | `02_pandas` |
| 4 | 8 | Visualización de datos con Matplotlib y Seaborn | `03_matplotlib_seaborn` |
| 5 | 9 | Visualización avanzada: gráficos científicos, subplots y anotaciones | `03_matplotlib_seaborn` |
| 5 | 10 | Estadística descriptiva e inferencial con SciPy | `04_scipy` |
| 6 | 11 | Optimización numérica: ajuste de curvas y minimización | `04_scipy` |
| 6 | 12 | Simulación numérica: Monte Carlo y ecuaciones diferenciales ordinarias (ODEs) | `04_scipy` |

---

### 🟢 FASE 2 — Aplicaciones en Ciencias Exactas (Semanas 7–10)

Esta fase aplica los conocimientos adquiridos en la Fase 1 a problemas concretos de Química y Biología, con énfasis en biología molecular.

| Semana | Sesión | Tema | Módulo |
|--------|--------|------|--------|
| 7 | 13 | Química: estequiometría y equilibrio químico con Python | `05_quimica` |
| 7 | 14 | Química: cinética química y modelado de reacciones (ODEs aplicadas) | `05_quimica` |
| 8 | 15 | Química: termodinámica computacional y análisis espectroscópico | `05_quimica` |
| 8 | 16 | Biología: introducción a la bioinformática y manejo de secuencias (Biopython) | `06_biologia` |
| 9 | 17 | Biología molecular: análisis de secuencias de ADN/ARN y proteínas | `06_biologia` |
| 9 | 18 | Biología molecular: alineamiento de secuencias y análisis filogenético básico | `06_biologia` |
| 10 | 19 | Biología: análisis microbiológico y modelado de crecimiento poblacional | `06_biologia` |
| 10 | 20 | Proyecto integrador: resolución de un problema real en Química o Biología | `07_proyecto` |

---

## 📁 Estructura del Repositorio

```
curso-python-cientifico/
├── 00_introduccion/          # Python desde cero: sintaxis, funciones, entorno
├── 01_numpy/                 # Arreglos numéricos y álgebra lineal
├── 02_pandas/                # Manipulación y análisis de datos tabulares
├── 03_matplotlib_seaborn/    # Visualización científica de datos
├── 04_scipy/                 # Estadística, optimización y simulación
├── 05_quimica/               # Aplicaciones en Química (cinética, equilibrio, termodinámica)
├── 06_biologia/              # Aplicaciones en Biología Molecular y Bioinformática
├── 07_proyecto/              # Proyecto integrador final
├── datos/                    # Datasets de ejemplo para los módulos
├── environment.yml           # Entorno de dependencias (Conda)
└── README.md
```

---

## ⚙️ Instalación y Configuración

### Con Conda (recomendado)

```bash
conda env create -f environment.yml
conda activate python-cientifico
jupyter lab
```

### Con pip

```bash
pip install numpy pandas matplotlib seaborn scipy biopython jupyterlab
```

---

## 📚 Herramientas del Curso

| Herramienta | Uso principal |
|-------------|---------------|
| `NumPy` | Arreglos numéricos, álgebra lineal |
| `Pandas` | Manipulación de datos tabulares |
| `Matplotlib / Seaborn` | Visualización científica |
| `SciPy` | Estadística, optimización, ODEs, simulación |
| `Biopython` | Bioinformática y biología molecular |
| `Jupyter Lab` | Entorno interactivo de desarrollo |

---

## 👤 Autor

**Edgar Luis Díaz** — [@EddiazOS](https://github.com/EddiazOS)  
Investigador y educador en bioinformática y biología computacional, Colombia.  
Facultad de Ciencias Exactas — Universidad de Cartagena.

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.
