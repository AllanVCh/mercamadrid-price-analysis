# Análisis de Precios en Mercamadrid: Volatilidad, Estacionalidad y Riesgos en la Planificación de Compras.
Este proyecto analiza la evolución histórica de los precios de productos comercializados en Mercamadrid, con el objetivo de apoyar la toma de decisiones de compra en empresas de distribución alimentaria o restauración.

A partir de datos públicos correspondientes al periodo 2021–2025, se estudian patrones de volatilidad y estacionalidad de precios a nivel de variedad de producto, identificando meses críticos, productos con mayor riesgo presupuestario y oportunidades de optimización en la planificación de compras.

El análisis se plantea desde la perspectiva de un Analista de Datos Junior, priorizando un enfoque descriptivo, explicable y orientado a negocio.

# Objetivos del análisis

- Clasificar los productos listados en Mercamadrid por su volatilidad en Volátiles, Estables e Intermedios.
- Detectar patrones estacionales relevantes en los precios de los productos más representados en el dataset.
- Determinar meses críticos en los que los precios de los productos más representados sufren variaciones importantes.
- Evaluar el riesgo presupuestario asociado a la variabilidad de precios.
- Generar insights accionables que permitan diseñar estrategias de compras anticipadas.

# Contexto de negocio

- Rol: Analista de Datos Junior
- Sector: Distribución alimentaria / restauración
- Caso de uso: Apoyo a decisiones de compra recurrentes en Mercamadrid

El análisis pretende simular un escenario real en el que una empresa necesita comprender el comportamiento histórico de precios para mejorar la planificación de compras y reducir la exposición a variaciones extremas
de precio.

# Dataset

- Fuente: Datos públicos de Mercamadrid
- Archivos: volpre2021 a volpre2025
- Frecuencia: Registros temporales por variedad de producto

# Variables principales

- FechaDesde
- DescripciónVariedad (nombre del producto)
- PrecioMásFrecuente
- PrecioMáximo
- PrecioMínimo

# Limpieza y preparación de datos

Durante la preparación del dataset se abordaron los siguientes aspectos:

- Conversión y validación de fechas
- Limpieza de columnas de precios (formato numérico)
- Normalización de nombres de productos
- Identificación y análisis de valores extremos (outliers)
- Filtrado de productos con baja frecuencia temporal

# Creación de variables derivadas

- Mes y año
- Variación mensual de precios
- Coeficiente de variación (volatilidad)

Para el análisis principal se utilizó el PrecioMásFrecuente como PrecioBase, al representar el comportamiento típico del mercado y reducir la influencia de valores extremos puntuales.

# Metodología

El proyecto se basa en un análisis exploratorio de datos (EDA) con enfoque en negocio:

- Cálculo de métricas de volatilidad (coeficiente de variación)
- Análisis temporal de precios por producto
- Estudio de estacionalidad mediante agregaciones mensuales
- Identificación de meses críticos con precios significativamente superiores al promedio
- Uso de visualizaciones claras y explicables para comunicar resultados

El análisis es descriptivo, no predictivo.

# Principales insights

Algunos de los hallazgos del análisis incluyen:

- Existen variedades con precios estructuralmente estables y otras con alta volatilidad, lo que implica distintos niveles de riesgo presupuestario.
- Determinados productos presentan picos de precio recurrentes en meses concretos (especialmente en diciembre y enero).
- La estacionalidad detectada permite identificar meses óptimos de compra y periodos a evitar.
- Algunos productos combinan alta volatilidad con estacionalidad marcada, lo que requiere una monitorización más activa.

# Recomendaciones de negocio

- Priorizar compras anticipadas o acuerdos en productos altamente volátiles.
- Ajustar la planificación de compras según patrones estacionales detectados.
- Monitorizar de forma continua productos con alta dispersión de precios.
- Utilizar métricas de volatilidad como apoyo en la gestión del riesgo presupuestario.

# Limitaciones

- No se consideran factores externos como clima, inflación o eventos logísticos.
- No se analizan productos sustitutos.
- Los datos son agregados y no reflejan negociaciones individuales.
- El análisis es descriptivo y no incluye modelos predictivos.

# Herramientas utilizadas

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

# Autor

Allan Villarreal C. / Analista de Datos Junior /
Proyecto independiente basado en datos públicos disponibles en: https://datos.madrid.es/portal/site/egob/menuitem.c05c1f754a33a9fbe4b2e4b284f1a5a0
