# Executive Report

## Ecommerce Sales Data Analysis

### Project Objective

The objective of this project was to analyze an e-commerce sales dataset containing 100,000 transactions in order to identify revenue drivers, customer behavior patterns and business insights that can support data-driven decision making.

The analysis included data quality assessment, feature engineering, exploratory data analysis (EDA), statistical evaluation and data visualization techniques.

---

## Dataset Overview

The dataset contains:

- 100,000 transactions
- 14 original variables
- Customer information
- Product information
- Payment methods
- Transaction dates
- Revenue-related variables

Data quality assessment revealed:

- No missing values
- No major data consistency issues
- Appropriate data types after transformation
- A dataset suitable for business analysis without extensive cleaning requirements

---

## Feature Engineering

To enhance the analysis, several new variables were created:

### Revenue

Revenue was calculated as:

Revenue = Quantity × Price × (1 - Discount)

This variable became the primary business metric used throughout the analysis.

### AgeGroup

Customers were segmented into age ranges:

- 18–25
- 26–35
- 36–50
- 50+

This segmentation enabled demographic analysis.

### HighValueCustomer

Transactions above the 75th percentile of revenue were classified as:

- High Value
- Regular

This feature supports customer segmentation and business-oriented analysis.

---

# Key Findings

## 1. Revenue Distribution

Revenue follows a positively skewed distribution.

Most transactions generate moderate revenue values, while a smaller number of higher-value transactions contribute disproportionately to total sales.

This pattern is common in e-commerce environments.

---

## 2. Product Categories Show Balanced Performance

Revenue is distributed relatively evenly across all product categories.

No single category dominates total revenue generation.

This suggests a diversified product portfolio and reduced dependency on individual product segments.

---

## 3. Customer Loyalty Is Not a Strong Revenue Predictor

The analysis found no strong relationship between Customer Loyalty Score and total revenue.

Customers with both high and low loyalty scores generated similar revenue patterns.

This indicates that loyalty alone is insufficient to explain spending behavior.

---

## 4. Customer Income Group Has Limited Impact

Revenue generation remains remarkably similar across low, medium and high income groups.

Customer income does not appear to be a major differentiating factor in purchasing behavior within this dataset.

---

## 5. Revenue Remains Relatively Stable Throughout the Year

Monthly revenue analysis identified moderate fluctuations across the year.

Higher-performing months include:

- May
- August
- December

Lower-performing months include:

- February
- September

However, the overall revenue pattern remains relatively stable.

---

## 6. Age Influences Total Revenue Contribution but Not Spending Behavior

Older customer segments generated higher total revenue.

However, average transaction revenue remained very similar across all age groups.

This suggests that differences in total revenue are driven by transaction volume rather than individual spending patterns.

---

## 7. Revenue Is Primarily Driven by Price and Quantity

Correlation analysis identified the strongest relationships with revenue:

| Variable | Correlation with Revenue |
|-----------|-----------|
| Price | 0.73 |
| Quantity | 0.57 |
| Discount | -0.13 |

Price and quantity are the primary revenue drivers.

Discounts show a small negative relationship with revenue generation.

---

## 8. Customer Revenue Is Highly Diversified

The Top 10 customers generate only:

**0.27% of total revenue**

This indicates an extremely diversified customer base and low dependency on individual customers.

Such diversification contributes to business resilience and stability.

---

# Business Recommendations

Based on the analysis, the following recommendations are proposed:

### Product Strategy

Continue maintaining a diversified product portfolio, as revenue is balanced across categories.

### Pricing Strategy

Prioritize pricing optimization and sales volume initiatives, as these variables demonstrate the strongest impact on revenue generation.

### Discount Management

Monitor discount strategies carefully to avoid unnecessary reductions in revenue.

### Customer Analytics

Explore additional customer behavior variables, since age, income and loyalty score alone do not explain purchasing patterns.

### Strategic Planning

Leverage the stable revenue structure and diversified customer base to support long-term growth initiatives.

---

# Conclusion

This exploratory data analysis successfully transformed raw transactional data into actionable business insights.

The analysis identified pricing and purchase volume as the main drivers of revenue generation, while demographic and loyalty-related variables showed limited predictive value.

The business represented by this dataset demonstrates:

- A diversified customer base
- Balanced category performance
- Stable revenue patterns
- Low customer concentration risk

These findings provide a solid foundation for future analytical initiatives, customer segmentation strategies and data-driven business decision making.

## Dataset Considerations

During the exploratory analysis, several variables exhibited highly balanced distributions across categories, income groups and customer segments.

These characteristics suggest that the dataset may have been synthetically generated or intentionally balanced for educational and analytical purposes.

As a result, the objective of this project is not to validate real-world e-commerce behavior, but rather to demonstrate the application of data analysis techniques, feature engineering, visualization methods and business-oriented interpretation of results.

The conclusions presented in this report should therefore be interpreted within the context of an educational dataset designed for exploratory analysis.

---

# Appendix – Executive Summary in Spanish

## Objetivo del Proyecto

El objetivo de este proyecto fue aplicar técnicas de Análisis Exploratorio de Datos (EDA) sobre un conjunto de datos de comercio electrónico con 100.000 transacciones, con el fin de identificar patrones de comportamiento, factores que influyen en los ingresos y oportunidades de análisis orientadas a la toma de decisiones.

## Consideraciones sobre el Dataset

Durante el análisis se observó que múltiples variables presentan distribuciones extremadamente equilibradas entre categorías, grupos de ingresos y segmentos de clientes.

Estas características sugieren que el dataset ha sido generado sintéticamente o diseñado con fines formativos, por lo que las conclusiones obtenidas deben interpretarse como un ejercicio de aplicación de técnicas analíticas y no como una representación exacta del comportamiento de un negocio real.

## Principales Hallazgos

### 1. Distribución de los ingresos

Los ingresos presentan una distribución asimétrica positiva. La mayoría de las transacciones generan ingresos moderados, mientras que un número reducido de operaciones de mayor valor incrementa significativamente la facturación total.

### 2. Categorías de producto equilibradas

Las diferentes categorías analizadas presentan niveles de ingresos muy similares, sin que exista una categoría claramente dominante.

### 3. La fidelización no explica el gasto

No se encontró una relación significativa entre el Customer Loyalty Score y los ingresos generados por los clientes.

### 4. El nivel de ingresos del cliente no es determinante

Los grupos de renta baja, media y alta muestran contribuciones muy similares a la facturación total.

### 5. Variaciones moderadas a lo largo del año

Se identificaron fluctuaciones mensuales en los ingresos, aunque sin una estacionalidad especialmente marcada.

### 6. La edad influye en el volumen, pero no en el gasto medio

Los grupos de mayor edad generan más ingresos totales, pero el gasto medio por transacción es prácticamente igual en todos los segmentos analizados.

### 7. Los principales impulsores del ingreso son el precio y la cantidad

El análisis de correlación identificó que las variables con mayor relación con los ingresos son:

- Precio del producto (0.73)
- Cantidad comprada (0.57)

### 8. Base de clientes altamente diversificada

Los 10 clientes con mayor facturación generan únicamente el **0,27%** de los ingresos totales, lo que indica una baja dependencia de clientes individuales.

## Conclusión

El proyecto permitió aplicar de forma práctica técnicas de limpieza de datos, análisis exploratorio, ingeniería de características, visualización y análisis estadístico.

Los resultados muestran que los ingresos están principalmente influenciados por el precio y el volumen de compra, mientras que variables demográficas y de fidelización presentan una capacidad explicativa limitada dentro de este conjunto de datos.

Más allá de los hallazgos concretos, el valor principal del proyecto reside en la metodología aplicada para transformar datos brutos en información útil para la toma de decisiones.