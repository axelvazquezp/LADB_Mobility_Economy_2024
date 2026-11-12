# LADB - Urban Traffic and Economic Mobility Analysis 🚗📈

Este repositorio contiene un caso de estudio avanzado de analítica de datos desarrollado para evaluar de forma longitudinal la correlación entre la movilidad urbana y la productividad macroeconómica en las principales metrópolis de Latinoamérica. El proyecto abarca un ciclo completo (End-to-End) de procesamiento, estandarización y modelado de bases de datos masivas.

---

## 🎯 Contexto y Problema de Negocio
El crecimiento acelerado de las zonas urbanas en Latinoamérica genera retos críticos en la infraestructura de transporte, impactando directamente en la competitividad económica de las regiones. La gestión pública y los fondos de inversión privados requieren identificar con precisión los focos de ineficiencia vial para optimizar la asignación de recursos y priorizar el desarrollo de infraestructura vial.

Este análisis estratégico busca resolver tres preguntas de negocio:
1. ¿Existe una relación directa entre los niveles de congestión vehicular y el Producto Interno Bruto (PIB) per cápita de las ciudades latinoamericanas?
2. ¿Cómo impactan los tiempos de retraso por tráfico (`jams_delay`) en la productividad laboral del mercado regional?
3. Basado en el cruce de datos económicos y operativos, ¿en qué ciudades clave se justifica con mayor urgencia la inversión en infraestructura de transporte?

---

## 🛠️ Tecnologías y Herramientas Utilizadas
*   **Python (Pandas, NumPy):** Procesamiento de datos masivos, preparación de variables para el cálculo de poblaciones absolutas y computación estadística.
*   **Seaborn & Matplotlib:** Diseño de visualizaciones analíticas avanzadas para la evaluación de distribuciones y detección de valores atípicos (outliers).
*   **Jupyter Notebook:** Entorno de desarrollo para la construcción del pipeline reproducible.

---

## 📊 Fuentes de Información e Integración de Datos
El núcleo técnico del proyecto radica en la ingesta, limpieza profunda y combinación de dos fuentes de datos de alta relevancia global:
1.  **TomTom Traffic Index:** Datos operativos reales sobre marcas de congestión, velocidades promedio y tiempos de retraso en tráfico.
2.  **OECD Cities (OCDE):** Indicadores macroeconómicos oficiales de productividad, PIB de la ciudad, demografía y empleo.

---

## 📊 Proceso de Análisis y Etapas del Proyecto

### 1. Preparación y Modelado de Datos (Python)
*   **Construcción de Pipeline Reproducible:** Automatización de la limpieza de datos para transformar tipos de datos genéricos (`object`) a variables numéricas y formatos de fecha optimizados.
*   **Estandarización de Estructuras:** Normalización masiva de nombres de columnas bajo la convención técnica `snake_case` para asegurar mantenibilidad.
*   **Tratamiento de Datos Masivos:** Filtrado temporal estricto (ejercicio 2024), agregación por promedios ponderados de tráfico y cálculo analítico de poblaciones absolutas.

### 2. Integración y Análisis Estadístico
*   **Uniones Internas Avanzadas (Inner Joins):** Consolidación de métricas de congestión vial frente a variables de desempeño macroeconómico.
*   **Auditoría de Distribuciones:** Evaluación de sesgos y tratamiento de valores atípicos utilizando métricas clave como el retraso por congestión (`jams_delay`) y el PIB per cápita (`city_gdp_capita`).

---

## 📈 Hallazgos Clave y Conclusiones de Negocio

| Dimensión Analizada | Diagnóstico / Hallazgo | Implicación y Decisión Estratégica |
| :--- | :--- | :--- |
| **Saturación Vial Máxima** | **Mexico City** registró el mayor tiempo promedio de retraso por tráfico en toda la región durante 2024. | Se posiciona como el mercado con mayor pérdida de horas-hombre productivas, marcando la prioridad número uno para proyectos de transporte masivo. |
| **Correlación de Movilidad** | Pérdida de productividad linealmente asociada a la métrica `jams_delay` en ciudades con PIB medio. | La congestión vehicular actúa como un freno directo para la competitividad económica de las metrópolis emergentes. |
| **Focos de Inversión** | Ciudades con alto PIB per cápita pero con infraestructura vial saturada. | El cruce de datos identifica los clústeres urbanos donde la inversión en transporte generará el mayor retorno en productividad para la OCDE. |

---

## 🚀 Recomendaciones Estratégicas
1. **Priorización de Capital en Nodos Críticos:** Dirigir de forma prioritaria los fondos de inversión en infraestructura vial hacia Ciudad de México y metrópolis con perfiles de congestión idénticos, enfocándose en alternativas de transporte multimodal para reducir los tiempos de retraso.
2. **Replicabilidad del Pipeline:** Implementar el flujo de preparación de datos desarrollado en Python para monitorear semestralmente los indicadores de TomTom y la OCDE, permitiendo un modelo predictivo de alerta temprana ante cuellos de botella urbanos.

---

## 🖼️ Interactividad y Acceso al Ecosistema

### 📓 Notebook del Proyecto en Google Colab
Haz clic en la insignia inferior para acceder directamente al entorno interactivo y reproducible en Google Colab para auditar el código, las uniones de datos y las gráficas estadísticas:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1wGsDTDRij0SDuKXaUV9Bx53MHkBruBR4)

O también puedes usar este enlace directo: [Abrir en Google Colab](https://colab.research.google.com/drive/1wGsDTDRij0SDuKXaUV9Bx53MHkBruBR4)

---

## 📂 Estructura del Repositorio
*   `S5 ladb_mobility_economy_project_.ipynb`: Jupyter Notebook principal que aloja el pipeline de limpieza, las consultas de integración avanzada y las visualizaciones analíticas.
