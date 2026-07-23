# Urban Traffic and Economic Mobility Analysis – Sprint 5

Este repositorio contiene el análisis realizado durante el Sprint 5 para evaluar cómo la movilidad urbana se relaciona con la productividad económica en las principales ciudades latinoamericanas[cite: 1].

El proyecto trabaja con datos reales de **TomTom Traffic Index** y **OECD Cities**, los cuales se limpian, combinan y analizan para identificar en qué ciudades conviene invertir en infraestructura de transporte[cite: 1].

## Contenido del repositorio

- `notebooks/S5_ladb_mobility_economy_project_.ipynb`: Notebook principal que incluye la carga, limpieza, estandarización de columnas, conversión de tipos de datos, filtrado por año (2024), agrupación por promedios de tráfico, cruce con indicadores económicos y visualizaciones analíticas.

## Cómo abrir el notebook en Google Colab

Puedes abrir y ejecutar este archivo directamente en tu navegador usando Google Colab mediante el siguiente enlace:

- [Abrir en Google Colab](https://colab.research.google.com/drive/1wGsDTDRij0SDuKXaUV9Bx53MHkBruBR4?usp=sharing)

## Objetivo del análisis

- **Evaluar cómo la movilidad urbana se relaciona con la productividad económica** en las principales ciudades latinoamericanas[cite: 1].
- **Construir un pipeline de limpieza reproducible** para transformar datos en formato *object* a numéricos/fechas, estandarizar nombres en *snake_case* y calcular poblaciones absolutas.
- **Analizar comportamientos, distribuciones y valores atípicos** mediante métricas como retrasos por congestión (`jams_delay`) y PIB per cápita (`city_gdp_capita`).
- **Generar insights estratégicos** para la toma de decisiones en inversiones de infraestructura vial (destacando a **Mexico City** con el mayor tiempo promedio de tráfico en 2024).
