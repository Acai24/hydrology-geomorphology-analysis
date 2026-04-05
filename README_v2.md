# Tesis: Modelación hidrológica e hidráulica de eventos de inundación en la cuenca del río Isa mediante HEC-HMS y HEC-RAS.

## Descripción
Este repositorio contiene los datos, scripts y resultados utilizados para el desarrollo de mi tesis.

## Objetivo de la tesis
El objetivo de este proyecto es analizar la precipitación en la cuenca del río Isa y estimar su impacto hidrológico mediante la generación de caudales superficiales y la identificación de posibles zonas de inundación. El estudio busca caracterizar la variabilidad temporal de la precipitación y su relación con el riesgo hidrológico en la cuenca.

---

## Estructura del repositorio
- data/ → Datos utilizados para el análisis hidrológico e hidráulico
- scripts/ → Scripts utilizados para procesamiento y análisis de datos
- figures/ → Gráficos y visualizaciones generadas con CloudCompare y QGIS
- results/ → Resultados obtenidos de la simulación hidrológica e hidráulica (HEC-HMS / HEC-RAS)
- thesis.pdf → Documento final de la tesis

---

## Herramientas utilizadas
- HEC-HMS (modelación hidrológica)
- HEC-RAS (modelación hidráulica e inundación)
- CloudCompare (procesamiento de nubes de puntos)
- R (tidyverse, ggplot2, sf)
- QGIS (visualización espacial)
- Datos CSV de precipitación
- Shapefiles de la cuenca del río Isa
- GitHub para control de versiones y documentación del proyecto
---

---



## 📈 Metodología
- Recolección y organización de datos hidrológicos y topográficos  
- Análisis exploratorio de los datos
- # Metodología
1. Recolección de datos de precipitación mensual en la cuenca del río Isa.
2. Limpieza y procesamiento de datos en R (manejo de valores faltantes y conversión numérica).
3. Análisis exploratorio de datos (EDA) para identificar patrones estacionales.
4. Cálculo de promedios mensuales de precipitación.
5. Estimación de caudal superficial mediante un coeficiente de escorrentía.
6. Visualización de resultados mediante gráficos en R.
7. Integración de datos espaciales con shapefiles del río Isa.
- # Análisis de precipitación
El análisis de precipitación mensual en la cuenca del río Isa permitió identificar una marcada estacionalidad, donde los meses de mayor precipitación corresponden a la temporada húmeda. Estos meses presentan valores superiores al promedio anual, lo que incrementa significativamente el potencial de generación de escorrentía superficial y, por ende, el riesgo de inundación en las zonas aledañas al cauce principal.
A partir de los datos de precipitación, se estimó el caudal superficial mediante la aplicación de un coeficiente de escorrentía. Los resultados evidencian una relación directa entre los meses de mayor precipitación y los incrementos en el caudal, lo cual confirma el comportamiento hidrológico esperado en la cuenca del río Isa.

- Modelación hidrológica con HEC-HMS  
- Modelación hidráulica de inundaciones con HEC-RAS  
- Procesamiento y análisis geoespacial en QGIS  
- Visualización y evaluación de resultados  
- Validación de escenarios de inundación  

---
 
---



## 🧠 Nota del estudio
Este proyecto se enfoca en la evaluación de la vulnerabilidad por inundación en zonas cercanas a cuerpos de agua mediante modelación numérica y análisis geoespacial.

## 👩‍💻 Autor
Romanti Esther Aquino Payano

## 📅 Fecha
2026
