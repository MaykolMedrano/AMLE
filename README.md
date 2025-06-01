-----

# EAE3709 - Aplicaciones de Machine Learning en Economía

**Instituto de Economía**
**Pontificia Universidad Católica de Chile**
**1er Semestre 2025**

-----

## Integrantes del Equipo

  - **Profesor**

      - Joaquín Pérez Lapillo

  - **Ayudantes**

      - Luis García B.
      - Sebastián Hernández B.
      - Oscar Herrera G.

  - **Estudiantes**

      - Catalina Aránguiz | **Github**: [caranguizc](https://github.com/caranguizc)
      - Maykol Medrano | **Github**: [MaykolMedrano](https://github.com/MaykolMedrano)

-----

## Descripción del Repositorio

Este repositorio contiene las soluciones para las tareas del curso **Aplicaciones de Machine Learning en Economía**. Cada tarea aborda diferentes técnicas y problemas, desde el análisis exploratorio y la integración de datos hasta la construcción de modelos de clasificación y clustering.

-----

## Tarea 1: Análisis Exploratorio de Datos (EDA) de Indicadores Socioeconómicos

Esta tarea se enfoca en el **análisis exploratorio de datos (EDA)**, integrando información económica, demográfica, de desigualdad y medioambiental para obtener una visión completa de las dinámicas globales.

### 🎯 Objetivos

  - **Importar y limpiar** datasets de diversas fuentes, manejando valores faltantes y estandarizando nombres de países.
  - **Analizar la distribución** de variables clave como el PIB per cápita, alfabetización y tasas de natalidad.
  - **Estudiar correlaciones** entre indicadores socioeconómicos y el desarrollo económico.
  - **Integrar datos** del Índice de Gini y emisiones de CO₂ para enriquecer el análisis.
  - **Evaluar el impacto** de crisis globales (Subprime 2008, COVID-19) en indicadores medioambientales.

### 💾 Fuentes de Datos

1.  **Dataset Económico-Demográfico (2007)**: [Repositorio en GitHub](https://raw.githubusercontent.com/lfgarcia-1/EAE3709-1-2025/refs/heads/main/economic_dataset.csv)
2.  **Índice de Gini**: [Repositorio en GitHub](https://raw.githubusercontent.com/datasets/gini-index/refs/heads/main/data/gini-index.csv)
3.  **Emisiones de CO₂ por Nación**: [Repositorio en GitHub](https://raw.githubusercontent.com/datasets/co2-fossil-by-nation/refs/heads/main/data/fossil-fuel-co2-emissions-by-nation.csv)

### 📈 Conclusiones Principales

  - El **PIB per cápita** se correlaciona positivamente con el acceso a tecnología y la alfabetización, y negativamente con la natalidad y mortalidad infantil.
  - Variables como la **Población** y el **Área** son más relevantes para explicar el PIB total que el PIB per cápita.
  - La **desigualdad (Gini)** muestra relaciones complejas; países con alto PIB pueden tener también alta desigualdad.
  - Las **emisiones de CO₂** de países industrializados tienden a aumentar, con caídas visibles durante crisis económicas globales.

### 📁 Archivos

  - `AMLE-TAREA-01.ipynb`: Notebook con el código, análisis detallado y visualizaciones.
  - `README.md`: Este archivo.

-----

## Tarea 2: Modelos de Clasificación y Clustering

Esta tarea se divide en dos partes: la construcción de un modelo de **clasificación** para un problema de marketing bancario y un análisis de **clustering** para agrupar países según su perfil de exportación.

### Parte A: Clasificación - Predicción de Suscripción a Depósitos a Plazo

  - **Problema**: Predecir si un cliente de un banco portugués suscribirá un depósito a plazo como resultado de una campaña de marketing telefónico.
  - **Objetivo**: Desarrollar un modelo de clasificación binaria (`sí/no`) que sea realista y predictivo, prestando especial atención a la ingeniería de características y la evaluación de modelos.
  - **Dataset**: Los datos provienen del [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing) e incluyen atributos del cliente (edad, trabajo, educación) e información de la campaña (tipo de contacto, duración de la llamada).

### Parte B: Clustering con K-Means & PCA - Perfiles de Exportación de Países

  - **Problema**: Ante una guerra comercial, ¿qué países podrían sufrir consecuencias similares? El objetivo es identificar grupos de países con perfiles de exportación parecidos.
  - **Objetivo**: Aplicar **K-Means** para encontrar clusters de países y usar **Análisis de Componentes Principales (PCA)** para identificar las variables de exportación más relevantes que definen estos grupos. Se utilizan datos del año 2023.
  - **Dataset**: Se utiliza una base de datos del Banco Mundial y el Trade Analysis Information System, disponible en [este link](https://www.google.com/search?q=https://raw.githubusercontent.com/olherreragz/EAE3709-2025-1/refs/heads/main/T2_data/Data.csv). Incluye indicadores como crecimiento del PIB, porcentaje de exportaciones de alta tecnología, combustibles, manufacturas, etc.

### 📁 Archivos

  - `AMLE-TAREA-02.ipynb`: Notebook con la implementación de los modelos de clasificación y los algoritmos de K-Means y PCA.
  - `README.md`: Este archivo.
