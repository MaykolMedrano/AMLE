
# Tarea 1: EAE3709 - Aplicaciones de Machine Learning en Economía
**Instituto de Economía**
**Pontificia Universidad Católica de Chile**
**1er Semestre 2025**

---

## Presentación

- **Profesor**
  - Joaquín Pérez Lapillo

- **Ayudantes**
  - Luis García B.
  - Sebastián Hernández B.
  - Oscar Herrera G.

- **Estudiantes**
  - Catalina Aránguiz | **Github**:  [caranguizc](https://github.com/caranguizc)
  - Maykol Medrano    | **Github**:  [MaykolMedrano](https://github.com/MaykolMedrano)

---

## 1. Introducción

Esta **Tarea 1** se centra en el **análisis exploratorio de datos (EDA)**, trabajando con información económica, demográfica y de desarrollo humano de múltiples fuentes. A lo largo del proceso, se integran también datos de desigualdad (Índice de Gini) y de emisiones de CO₂ por país, buscando una visión más amplia sobre la relación entre crecimiento económico, desigualdad y factores medioambientales.

---

## 2. Objetivos de la Tarea

- **Importar y limpiar** diversos datasets, formateando adecuadamente las columnas y resolviendo inconsistencias en los nombres de países.
- **Analizar** la distribución de variables clave (ej. PIB per cápita, tasa de natalidad, tasa de mortalidad infantil, etc.) y detectar valores atípicos (outliers).
- **Estudiar correlaciones** entre variables socioeconómicas y la variable objetivo (PIB per cápita o PIB agregado).
- **Integrar** información de múltiples fuentes (Índice de Gini y emisiones de CO₂) mediante uniones (merges) basadas en “año” y “nombre de país”.
- **Comparar** cómo distintos indicadores (p.ej., tasa de crecimiento de emisiones de CO₂) reaccionan a eventos globales como la crisis subprime y la crisis del COVID-19.

---

## 3. Estructura de la Tarea

1. **Carga y Limpieza de Datos**
   - Importar los datasets desde repositorios de GitHub.
   - Formatear columnas (tipos de datos, fechas, etc.).
   - Eliminar o imputar valores faltantes (NaN) con criterios justificados (p.ej., media o mediana por región).

2. **EDA Inicial (Dataset Económico-Demográfico)**
   - Cálculo de estadísticas descriptivas (media, mediana, desviación estándar) para variables como `Population`, `GDP ($ per capita)`, `Literacy (%)`, etc.
   - Visualización de distribuciones (KDE plots, histogramas, boxplots) y detección de outliers.
   - Análisis de correlaciones (absolute correlation ranking) para entender qué factores inciden más en el PIB per cápita y en el PIB total.

3. **Integración del Índice de Gini**
   - Limpieza de nombres de países y conversión de las columnas de año.
   - Mapeo de nombres inconsistentes para poder hacer un **INNER JOIN**.
   - Análisis de correlaciones entre el Índice de Gini y variables socioeconómicas claves, discutiendo hallazgos y sorpresas.

4. **Integración de Emisiones de CO₂**
   - Uso de un tercer dataset que detalla emisiones totales y por tipo de combustible (solid, liquid, gas, cement, etc.).
   - Creación y visualización de **series de tiempo** para varios países destacados (EE.UU., China, Alemania...).
   - Cálculo de tasas de crecimiento (pct change) y desviaciones respecto al promedio para estudiar el comportamiento en periodos de crisis (2007-2010 y 2017-2020).

5. **Merge Final y Heatmap**
   - Unión de los datos anteriores en un único dataframe “final” (para 2007).
   - Generación de un **heatmap** de correlaciones con un énfasis en la variable de emisiones totales de CO₂ (`Total`).
   - Interpretación sobre qué variables económicas, demográficas y de desarrollo humano están más relacionadas con la contaminación.

---

## 4. Fuentes de Datos

1. **Dataset Económico-Demográfico (2007)**
   - Repositorio en [GitHub](https://raw.githubusercontent.com/lfgarcia-1/EAE3709-1-2025/refs/heads/main/economic_dataset.csv).

2. **Índice de Gini**
   - Datos anuales sobre la desigualdad de ingresos a nivel de cada país.
   - Repositorio en [GitHub](https://raw.githubusercontent.com/datasets/gini-index/refs/heads/main/data/gini-index.csv).

3. **Emisiones de CO₂**
   - Datos de emisiones totales y por combustible fósil, además de variables como `Per Capita`, `Bunker fuels`, etc.
   - Repositorio en [GitHub](https://raw.githubusercontent.com/datasets/co2-fossil-by-nation/refs/heads/main/data/fossil-fuel-co2-emissions-by-nation.csv).

---

## 5. Conclusiones Generales

- **PIB per cápita** suele asociarse de manera positiva con el **acceso a tecnología** (teléfonos per cápita) y la **alfabetización**, mientras que presenta correlaciones negativas con tasas de natalidad y mortalidad infantil.
- Al analizar **PIB ($)**, otras variables como la **Población**, **Teléfonos per cápita** o el **Area** muestran más relevancia que en el PIB per cápita.
- La **desigualdad económica** (Índice de Gini) guarda relaciones diversas con las variables económicas; ciertos países con alto PIB pueden mostrar altos niveles de desigualdad.
- En emisiones de CO₂, países industrializados (EE.UU., China, Alemania, etc.) presentan tendencias de **aumento** a lo largo del tiempo, con disrupciones en años de crisis, exceptuando a Alemania.
- La **fusión de datos** de múltiples fuentes permite comprender de manera más integral la relación entre desarrollo económico, desigualdad y sostenibilidad medioambiental.

---

## 6. Estructura de Archivos y Uso

- `Tarea_1.ipynb`: Archivo principal que contiene la resolución paso a paso, con sus explicaciones y visualizaciones.
- `README.md`: Explica el contexto de la tarea, su objetivo y conclusiones centrales.

---

¡Gracias por leer este README!
Para más detalles, revisa el **notebook**, donde se profundiza en cada paso descrito.

