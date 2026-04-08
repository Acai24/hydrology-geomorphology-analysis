# Tesis: Modelación hidrológica e hidráulica de eventos de inundación en la cuenca del río Isa mediante HEC-HMS y HEC-RAS.

## Descripción
Este repositorio contiene los datos, scripts y resultados utilizados para el desarrollo de mi tesis.

## Objetivo de la tesis
Este estudio tiene como objetivo analizar la precipitación en la cuenca del río Isa y su transformación en escorrentía superficial, con el fin de modelar caudales de diseño y simular escenarios de inundación mediante HEC-HMS y HEC-RAS. Además, se busca identificar zonas susceptibles a inundación a partir de la integración de análisis hidrológico y modelación hidráulica.
---

## Estructura del repositorio
data/
   ## Estructura del repositorio

data/
   ├── precipitation/
   ├── hydrology/
   ├── gis/

scripts/
 ├── 01_data_cleaning.R
 ├── 02_hydrology_model.R
 ├── 03_flood_mapping.R

hec_hms/
   ├── basin_model/
   ├── meteorologic_model/
   ├── run_files/

hec_ras/
   ├── geometry/
   ├── flow_data/
   ├── boundary_conditions/   
   ├── ras_outputs/
   

figures/
   ├── precipitation_analysis/
   ├── flood_maps/
   ├── ras_profiles/
   ├── simulation/
   ├── hec_ras_simulation.mp4

# Simulación hidráulica (HEC-RAS)

Simulación del comportamiento del flujo en el río Isa bajo condiciones de crecida:

![HEC-RAS Simulation](figures/simulation/hec_ras_simulation.mp4)

results/
   ├── discharge_results.csv
   ├── flood_depths.tif
   ├── discharge_results.csv

thesis/
   ├── thesis.pdf
   ├── methodology.md
---

## Metodología
El desarrollo del estudio se realizó en las siguientes etapas:
-Recolección de datos de precipitación mensual en la cuenca del río Isa.
-Procesamiento y limpieza de datos en R (manejo de valores faltantes y normalización).
-Análisis exploratorio de precipitación y caracterización de estacionalidad.
-Estimación de escorrentía superficial mediante coeficiente de escorrentía.
-Generación de caudales de entrada para el modelo HEC-HMS.
-Modelación hidrológica de la cuenca en HEC-HMS.
-Modelación hidráulica de inundaciones en HEC-RAS.
-Integración de resultados con SIG (QGIS y R sf).
-Generación de mapas de inundación y zonas de riesgo.

---

 ## Herramientas utilizadas
 R(tidyverse, sf, ggplot2)
🌊 HEC-HMS (modelación hidrológica)
🌊 HEC-RAS (modelación hidráulica)
🗺️ QGIS (análisis espacial)
📊 Excel / CSV (datos de precipitación)
🛰️ Shapefiles de la cuenca del río Isa
☁️ CloudCompare (topografía / nubes de puntos)
💻 GitHub (control de versiones)
---

---
 # Análisis de precipitación

El análisis de precipitación mensual en la cuenca del río Isa permitió identificar una marcada estacionalidad, donde los meses de mayor precipitación corresponden a la temporada húmeda. Estos meses presentan valores superiores al promedio anual, lo que incrementa significativamente el potencial de generación de escorrentía superficial y, por ende, el riesgo de inundación en las zonas aledañas al cauce principal.

A partir de los datos de precipitación, se estimó el caudal superficial mediante un coeficiente de escorrentía, evidenciando una relación directa entre precipitación y caudal generado.

 # Modelación hidrológica (HEC-HMS)

Se desarrolló un modelo hidrológico de la cuenca del río Isa utilizando HEC-HMS para transformar la precipitación en caudal de escorrentía. Este modelo permitió estimar hidrogramas de respuesta para distintos eventos de lluvia.

 # Modelación hidráulica (HEC-RAS)

Se generó una aproximación de la zona de inundación mediante un buffer hidráulico alrededor del cauce principal del río Isa, como representación simplificada de la expansión lateral del flujo en condiciones de crecida. Esta metodología es equivalente a una aproximación preliminar de resultados obtenidos mediante modelos hidráulicos como HEC-RAS. Los caudales obtenidos fueron utilizados en HEC-RAS para simular el comportamiento del flujo en el cauce del río Isa, permitiendo identificar zonas potenciales de desbordamiento e inundación.

# Simulación hidráulica (HEC-RAS)

Se realizó una simulación hidráulica del río Isa utilizando HEC-RAS, donde se modeló el comportamiento del flujo bajo condiciones de crecida.
https://github.com/tu-usuario/tu-repo/blob/main/figures/simulation/hec_ras_simulation.mp4

 # Resultados
 -Modelación hidrológica e hidráulica; The analysis of precipitation allows the caudate to be measured in a simple manner based on the coefficients of escorrentia, which represents an approximate conceptual model in HEC-HMS.The caudales generados fueron utilizados as part of the hydraulic simulation in HEC-RAS, permitiendo to analyze the transport of the flujo in the cauce of the Río Isa. Los results evidencian una expansion lateral del flujo en conditions de high precipitation, lo cual fue representado mediante la generación de zonas de inundación en torno SIG.
-Mapas de precipitación acumulada
-Hidrogramas de caudal
-Mapas de profundidad de inundación
-Zonas de riesgo hidráulico

---

## 👩‍💻 Autor
Romanti Esther Aquino Payano

## 📅 Fecha
2026
