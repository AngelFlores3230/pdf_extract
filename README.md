# pdf_extract
# Análisis Comparativo de Librerías Python para Extracción de Texto desde Documentos PDF Digitales

Repositorio experimental desarrollado para comparar el desempeño de diferentes librerías Python orientadas a la extracción automática de texto desde documentos PDF digitales.

El proyecto evalúa las librerías:

* PyMuPDF
* pdfminer.six
* pdfplumber
* pypdf

mediante un conjunto homogéneo de métricas cuantitativas y análisis estadístico reproducible.

---

# Objetivo

Comparar el comportamiento de distintas librerías de extracción de texto desde PDF en términos de:

* velocidad de procesamiento
* cantidad de texto recuperado
* porcentaje de frases válidas
* redundancia textual
* escalabilidad según número de páginas

El estudio busca proporcionar una base experimental útil para proyectos de:

* minería de texto
* procesamiento documental
* construcción de corpus lingüísticos
* NLP
* sistemas RAG
* recuperación de información

---

# Diseño Experimental

Se ejecutaron pruebas utilizando:

| Documento PDF | Número de páginas |
| ------------- | ----------------- |
| Documento 1   | 10 páginas        |
| Documento 2   | 25 páginas        |
| Documento 3   | 50 páginas        |
| Documento 4   | 100 páginas       |

Cada documento fue procesado con las cuatro librerías bajo las mismas condiciones computacionales.

Total de ejecuciones experimentales:

4 librerías × 4 documentos = 16 ejecuciones

---

# Métricas Evaluadas

El experimento registra automáticamente las siguientes métricas:

* tiempo de extracción
* total de caracteres
* total de palabras
* total de frases
* frases válidas
* frases inválidas
* porcentaje de frases válidas
* frases duplicadas
* porcentaje de duplicados
* promedio de palabras por frase
* promedio de caracteres por página
* páginas con error

---

# Estructura del Repositorio

```text
├── notebooks/
│   ├── extraccion_pymupdf.ipynb
│   ├── extraccion_pdfminer.ipynb
│   ├── extraccion_pdfplumber.ipynb
│   ├── extraccion_pypdf.ipynb
│   └── consolidacion_resultados.ipynb
│
├── datasets/
│   ├── pdf_10_paginas.pdf
│   ├── pdf_25_paginas.pdf
│   ├── pdf_50_paginas.pdf
│   └── pdf_100_paginas.pdf
│
├── resultados/
│   ├── metricas_consolidadas.csv
│   ├── frases_consolidadas.csv
│   ├── resumen_por_libreria.csv
│   └── tablas_estadisticas.csv
│
└── README.md
```

---

# Tecnologías Utilizadas

* Python 3
* Google Colab
* pandas
* matplotlib
* scipy
* statsmodels
* PyMuPDF
* pdfminer.six
* pdfplumber
* pypdf

---

# Análisis Estadístico

El estudio incluye:

* ANOVA de un factor
* Kruskal-Wallis
* ANOVA bloqueado por documento
* Tukey HSD

Estas pruebas permitieron determinar si las diferencias observadas entre librerías fueron estadísticamente significativas.

---

# Resultados Generales

Principales hallazgos del experimento:

* PyMuPDF obtuvo el mejor rendimiento temporal.
* pdfminer.six alcanzó el mayor porcentaje de frases válidas.
* pdfplumber presentó el menor porcentaje de duplicados.
* El tamaño del documento influye significativamente en el comportamiento de las librerías.

---

# Reproducibilidad

Todos los notebooks, datasets, métricas y resultados estadísticos se incluyen en este repositorio con el propósito de garantizar:

* transparencia experimental
* validación independiente
* reutilización académica
* comparación con futuras herramientas

---

# Cómo Ejecutar el Proyecto

## 1. Clonar repositorio

```bash
git clone https://github.com/usuario/repositorio.git
```

## 2. Abrir notebooks

Los notebooks pueden ejecutarse directamente en:

* Google Colab
* Jupyter Notebook
* JupyterLab

## 3. Instalar dependencias

```bash
pip install pymupdf
pip install pdfminer.six
pip install pdfplumber
pip install pypdf
pip install pandas
pip install matplotlib
pip install scipy
pip install statsmodels
```

---

# Trabajo Futuro

Como líneas futuras de investigación se propone:

* incorporar PDFs escaneados con OCR
* evaluar documentos multicolumna
* analizar tablas y estructuras complejas
* integrar métricas semánticas
* construir corpus paralelos bilingües
* evaluar calidad lingüística mediante NLP

---

# Contribución del Autor

El autor desarrolló la totalidad del diseño experimental, implementación de algoritmos, procesamiento documental, análisis estadístico y generación de resultados. Todos los recursos permanecen disponibles en este repositorio para fines académicos y de investigación.

---

# Licencia

Este proyecto se distribuye con fines académicos y de investigación.

