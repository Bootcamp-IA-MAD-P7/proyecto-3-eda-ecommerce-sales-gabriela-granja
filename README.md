# 🛒 Ecommerce Sales Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4C72B0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626)
![EDA](https://img.shields.io/badge/EDA-Exploratory%20Data%20Analysis-success)
![Bootcamp](https://img.shields.io/badge/Bootcamp-Data%20Analytics%20%26%20AI-green)

## 📖 Descripción del Proyecto

Este proyecto aplica técnicas de **Análisis Exploratorio de Datos (EDA)** sobre un conjunto de datos de comercio electrónico compuesto por **100.000 transacciones**.

El objetivo es identificar los factores que impulsan los ingresos, analizar el comportamiento de los clientes y extraer conclusiones de negocio mediante procesos de:

- Limpieza de datos
- Ingeniería de características
- Análisis estadístico
- Visualización de datos
- Interpretación de resultados

Este trabajo forma parte del **Bootcamp de Data Analytics & Artificial Intelligence** y busca transformar datos transaccionales en información útil para la toma de decisiones.

---

## 🎯 Objetivo de Negocio

La pregunta principal que guía este análisis es:

> ¿Qué factores impulsan la generación de ingresos en un negocio de comercio electrónico?

Para responderla se analizan patrones de compra, comportamiento de clientes, rendimiento de categorías de producto y variables relacionadas con los ingresos.

---

## 📊 Dataset

**Nombre:** Ecommerce Sales Dataset

**Fuente:**  
https://www.kaggle.com/datasets/shakirul09/ecommerce-sales-dataset

### Características del Dataset

- 100.000 transacciones
- Información de clientes
- Información de productos
- Métodos de pago
- Descuentos
- Variables demográficas
- Indicadores de fidelización
- Fechas de transacción

### ⚠️ Consideraciones sobre el Dataset

Durante el análisis se observó que múltiples variables presentan distribuciones extremadamente equilibradas entre categorías, grupos de ingresos y segmentos de clientes.

Estas características sugieren que el dataset ha sido generado sintéticamente o diseñado con fines educativos.

Por este motivo, el objetivo principal del proyecto no es validar comportamientos reales de mercado, sino demostrar la aplicación práctica de:

- Exploratory Data Analysis (EDA)
- Data Cleaning
- Feature Engineering
- Data Visualization
- Statistical Analysis
- Business Storytelling

---

## 📂 Estructura del Repositorio

```text
proyecto-3-eda-ecommerce-sales-gabriela-granja/

├── data/
│   ├── raw/
│   │   └── dataset_instructions.md
│   │
│   └── processed/
│
├── notebooks/
│   └── ecommerce_eda.ipynb
│
├── reports/
│   └── executive_report.md
│
├── images/
│   └── charts/
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🚀 Cómo Reproducir el Proyecto

### 1. Clonar el repositorio

```bash
git clone <repository-url>
```

### 2. Crear un entorno virtual

```bash
python -m venv venv
```

### 3. Activar el entorno virtual

Windows (Git Bash)

```bash
source venv/Scripts/activate
```

### 4. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 5. Descargar el Dataset

Descargar desde Kaggle:

https://www.kaggle.com/datasets/shakirul09/ecommerce-sales-dataset

Guardar el archivo CSV en:

```text
data/raw/ecommerce_sales_data.csv
```

### 6. Ejecutar el Notebook

Abrir:

```text
notebooks/ecommerce_eda.ipynb
```

y ejecutar todas las celdas.

---

## 🧠 Metodología

El proyecto sigue un flujo clásico de análisis exploratorio de datos.

### 1️⃣ Data Loading

- Importación del dataset
- Exploración inicial
- Validación estructural

### 2️⃣ Data Quality Assessment

- Análisis de valores nulos
- Detección de duplicados
- Revisión de tipos de datos

### 3️⃣ Feature Engineering

Se crearon nuevas variables orientadas al análisis de negocio.

#### Revenue

```text
Revenue = Quantity × Price × (1 - Discount)
```

#### AgeGroup

Segmentación de clientes por edad:

- 18–25
- 26–35
- 36–50
- 50+

#### HighValueCustomer

Clasificación de transacciones:

- High Value
- Regular

utilizando el percentil 75 como umbral.

### 4️⃣ Exploratory Data Analysis (EDA)

Análisis realizados:

- Distribución de ingresos
- Rendimiento por categoría
- Fidelización de clientes
- Grupos de ingresos
- Tendencias temporales
- Segmentación por edad
- Correlaciones
- Concentración de clientes

### 5️⃣ Interpretación de Negocio

Cada visualización incorpora:

- Contexto
- Objetivo
- Análisis
- Interpretación
- Implicaciones de negocio

---

## 🔍 Principales Hallazgos

### 📈 Distribución de Ingresos

Los ingresos presentan una distribución asimétrica positiva.

La mayoría de las transacciones generan ingresos moderados, mientras que un número reducido de compras de alto valor incrementa significativamente la facturación total.

### 🛍️ Categorías de Producto

Los ingresos se distribuyen de forma bastante equilibrada entre todas las categorías analizadas.

No existe una categoría claramente dominante.

### 🤝 Fidelización

No se identificó una relación significativa entre el índice de fidelización y los ingresos generados.

### 💰 Grupos de Ingresos

Los distintos grupos económicos presentan comportamientos muy similares respecto a la generación de ingresos.

### 📅 Tendencias Temporales

Los ingresos muestran variaciones moderadas a lo largo del año.

Los meses con mejor rendimiento fueron:

- Mayo
- Agosto
- Diciembre

### 📊 Principales Drivers de Revenue

| Variable | Correlación |
|-----------|------------|
| Price | 0.73 |
| Quantity | 0.57 |
| Discount | -0.13 |

El precio y la cantidad comprada son los principales impulsores de los ingresos.

### 👥 Diversificación de Clientes

Los 10 clientes con mayor facturación generan únicamente:

**0,27% de los ingresos totales**

Esto indica una base de clientes altamente diversificada y una baja dependencia de clientes individuales.

---

## 💡 Recomendaciones de Negocio

### Estrategia de Precio

Priorizar iniciativas relacionadas con optimización de precios.

### Incremento de Volumen

Fomentar estrategias orientadas al aumento del volumen de compra.

### Gestión de Descuentos

Monitorizar cuidadosamente el impacto de las promociones sobre los ingresos.

### Analítica de Clientes

Profundizar en variables de comportamiento más allá de la edad, ingresos o fidelización.

### Planificación Estratégica

Aprovechar la estabilidad y diversificación observadas para impulsar iniciativas de crecimiento sostenible.

---

## 🛠️ Tecnologías Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git
- GitHub

---

## 📑 Entregables

### Notebook Principal

```text
notebooks/ecommerce_eda.ipynb
```

Incluye:

- Limpieza de datos
- Ingeniería de características
- Visualizaciones
- Interpretación de resultados
- Conclusiones

### Informe Ejecutivo

```text
reports/executive_report.md
```

Incluye:

- Hallazgos principales
- Insights de negocio
- Recomendaciones
- Conclusiones ejecutivas

---

## 🎓 Competencias Desarrolladas

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Statistical Thinking
- Data Visualization
- Business Storytelling
- Insight Generation
- Git & GitHub Workflow

---

## 👩‍💻 Autora

**Gabriela Granja**

**Business, Marketing & AI**

🔗 GitHub: https://github.com/gabrielagranja

Proyecto desarrollado como parte del portfolio del **Bootcamp de Data Analytics & Artificial Intelligence**.