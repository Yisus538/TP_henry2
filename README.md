# Proyecto de Análisis de Datos de Telecomunicaciones

## Descripción General

Este proyecto involucra un análisis exhaustivo del sector de telecomunicaciones en Argentina, con un enfoque particular en el acceso a internet en diferentes provincias. El objetivo principal es ayudar a una empresa proveedora de servicios de telecomunicaciones a comprender el panorama actual, identificar oportunidades de crecimiento y mejorar la calidad del servicio. El proyecto incluye un Análisis Exploratorio de Datos (EDA), el desarrollo de un dashboard funcional e interactivo, y el cálculo y la visualización de Indicadores Clave de Rendimiento (KPIs).

## Estructura del Proyecto

- **data/**
  - **processed/**: Contiene los conjuntos de datos procesados utilizados en el análisis.
    - `accesos_por_tecnologia.csv`: Datos de accesos categorizados por tecnología.
    - `penetracion-hogar.csv`: Datos sobre las tasas de penetración en los hogares.
    - `Penetracion-total.csv`: Datos de penetración total.
  - **raw/**: Contiene los conjuntos de datos originales, tal como fueron recibidos, antes de cualquier procesamiento.
  
- **notebooks/**
  - **EDA.ipynb**: Notebook de Jupyter que contiene el Análisis Exploratorio de Datos (EDA). Este notebook documenta todo el proceso de EDA, incluyendo la limpieza de datos, el análisis de valores faltantes, outliers y visualizaciones. Cada paso está acompañado de celdas Markdown que explican los hallazgos y conclusiones.
  
- **Scripts/**
  - `data_processing.py`: Script en Python para procesar los datos originales en un formato utilizable para el análisis.

- **venv/**: Entorno virtual que contiene las dependencias necesarias para el proyecto.

- **.gitattributes**: Archivo de configuración de Git para manejar diferentes tipos de archivos.
  
- **README.md**: Archivo de documentación del proyecto que proporciona una visión general del proyecto, su estructura y las principales conclusiones.

## Tecnologías y Herramientas

- **Python**: Lenguaje de programación principal utilizado para el procesamiento y análisis de datos.
- **Pandas**: Utilizado para la manipulación y análisis de datos.
- **Matplotlib/Seaborn**: Utilizados para la creación de visualizaciones.
- **Jupyter Notebook**: Para documentar el proceso de EDA.
- **Dash/Plotly**: Utilizado para crear el dashboard interactivo.
- **Git**: Sistema de control de versiones utilizado para rastrear los cambios del proyecto.

## Metodología

### 1. Análisis Exploratorio de Datos (EDA)
Se realizó un EDA para obtener una comprensión inicial de los datos, identificar patrones y reconocer problemas de calidad de los datos. Se tomaron los siguientes pasos:

- **Análisis de Valores Faltantes**: Identificación y tratamiento de datos faltantes en el conjunto de datos.
- **Detección de Outliers**: Examinación de los datos para detectar valores extremos que podrían sesgar el análisis.
- **Visualización de Datos**: Se utilizaron diversos gráficos y diagramas para visualizar tendencias y distribuciones dentro de los datos.

### 2. Desarrollo del Dashboard
Se creó un dashboard interactivo que permite la exploración detallada de los datos. El dashboard incluye filtros por provincia, período de tiempo y tipo de acceso, facilitando el análisis de aspectos específicos de los datos.

### 3. Análisis de KPIs

Se calcularon los siguientes KPIs:

- **Promedio de accesos por cada 100 hogares por provincia**:
  - Este KPI se calculó agrupando los datos por provincia y obteniendo el promedio de accesos por cada 100 hogares.
  - **Promedio nacional**: También se calculó el promedio de accesos por cada 100 hogares a nivel nacional.

- **Promedio de accesos por cada 100 habitantes por provincia**:
  - Similar al KPI anterior, este mide el promedio de accesos por cada 100 habitantes por provincia.
  - **Promedio nacional**: Se calculó el promedio de accesos por cada 100 habitantes a nivel nacional.

- **Proporción de accesos por tecnología**:
  - Se sumaron los accesos por cada tipo de tecnología y se calculó la proporción que representa cada tecnología sobre el total de accesos.

Estos KPIs fueron calculados y visualizados en el dashboard para proporcionar insights accionables para los tomadores de decisiones.

## Análisis y Conclusiones

El análisis reveló varios insights clave:

- **Tendencias en el Acceso a Internet**: Hay un incremento constante en el acceso a internet en la mayoría de las provincias, siendo las áreas urbanas las que muestran las tasas de crecimiento más altas.
- **Penetración de Tecnologías**: La tecnología de fibra óptica está ganando terreno rápidamente, superando a las conexiones ADSL tradicionales.
- **Oportunidades de Crecimiento**: Las provincias con menores tasas de penetración presentan oportunidades significativas para la expansión.

Estos hallazgos sugieren que la empresa de telecomunicaciones debería enfocarse en expandir la infraestructura de fibra óptica en áreas rurales, mientras continúa mejorando la calidad del servicio en los centros urbanos.

