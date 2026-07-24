# Smart Supply Chain Analytics

## Descripción general

Smart Supply Chain Analytics es un proyecto integral de análisis de datos y aprendizaje automático desarrollado sobre el dataset público Olist (Brazilian E-Commerce Dataset). El objetivo es construir un ecosistema analítico capaz de apoyar la toma de decisiones relacionadas con la gestión de inventarios, la predicción de demanda y la optimización de la cadena de suministro mediante técnicas de ingeniería de datos, inteligencia de negocios y machine learning.

La solución integra procesos ETL, modelado dimensional, análisis exploratorio, modelos predictivos, segmentación de vendedores, pronósticos de demanda, dashboards de inteligencia de negocios y una aplicación interactiva para la consulta de resultados.

---

## Objetivo del proyecto

Diseñar e implementar una plataforma analítica que permita:

* Anticipar posibles quiebres de inventario mediante modelos de pronóstico.
* Identificar patrones operativos mediante segmentación de vendedores.
* Predecir retrasos en entregas utilizando modelos supervisados.
* Integrar información transaccional y fuentes externas para enriquecer los análisis.
* Facilitar la toma de decisiones mediante dashboards e interfaces interactivas.

---

## Problema de negocio

Las empresas de comercio electrónico enfrentan desafíos relacionados con la variabilidad de la demanda, la gestión eficiente del inventario y el cumplimiento de tiempos de entrega.

Una planificación inadecuada puede generar:

* Rupturas de stock.
* Sobreinventario.
* Incremento de costos logísticos.
* Pérdida de ventas.
* Deterioro de la experiencia del cliente.

Este proyecto busca abordar estos problemas mediante el análisis de datos históricos y la construcción de modelos predictivos orientados a la operación de una cadena de suministro.

---

## Arquitectura de la solución

La solución fue diseñada bajo una arquitectura orientada al procesamiento analítico de datos.

### Flujo general

1. Extracción e integración de datos transaccionales.
2. Limpieza y estandarización de información.
3. Construcción del Data Warehouse.
4. Generación de variables analíticas.
5. Entrenamiento de modelos de Machine Learning.
6. Visualización mediante dashboards.
7. Consulta de resultados mediante aplicación interactiva.

### Diagrama de arquitectura

![Diagrama OLTP](img/Diagrama_OLTP.png)

---

## Dataset

### Fuente principal

* Olist Brazilian E-Commerce Dataset

Información utilizada:

* Pedidos
* Clientes
* Productos
* Vendedores
* Pagos
* Reseñas
* Geolocalización

### Fuente exógena

Se incorporó información de eventos comerciales y días festivos relevantes en Brasil para enriquecer los modelos predictivos.

Ejemplos:

* Black Friday
* Cyber Monday
* Días festivos nacionales

---

## Tecnologías utilizadas

### Lenguajes

* Python
* SQL

### Herramientas

* Google BigQuery
* Looker Studio
* Streamlit

### Librerías

* Pandas
* NumPy
* Scikit-learn
* Statsmodels
* Plotly

---

## Componentes del proyecto

### ETL e Ingeniería de Datos

Se desarrollaron procesos de extracción, transformación y carga para integrar múltiples fuentes de información y preparar los datos para análisis y modelado.

Actividades realizadas:

* Limpieza de datos.
* Estandarización de registros.
* Tratamiento de valores faltantes.
* Manejo de valores atípicos.
* Integración de fuentes externas.
* Generación de tablas analíticas.

### Modelado Dimensional

Se diseñó un Data Warehouse basado en esquema estrella para optimizar las consultas analíticas y la generación de indicadores.

![Diagrama Data Warehouse](img/Diagrama_estrella.png)

---

### Segmentación de vendedores

Se aplicaron algoritmos de clustering para identificar grupos de vendedores con comportamientos similares y generar estrategias diferenciadas de operación.

Técnica utilizada:

* K-Means

Objetivo:

* Identificar patrones de desempeño.
* Apoyar decisiones de abastecimiento y logística.

---

### Pronóstico de demanda

Se implementaron modelos de series de tiempo para estimar la demanda futura de productos y anticipar posibles quiebres de inventario.

Técnicas utilizadas:

* SARIMA

Objetivos:

* Pronosticar demanda por categoría.
* Generar alertas tempranas.
* Apoyar estrategias de reabastecimiento.

**[INSERTAR AQUÍ GRÁFICAS DE PRONÓSTICO Y RESULTADOS DEL MODELO]**

---

### Predicción de retrasos

Se desarrollaron modelos supervisados para identificar pedidos con alta probabilidad de retraso en la entrega.

Objetivos:

* Reducir riesgos operativos.
* Mejorar la experiencia del cliente.
* Facilitar acciones preventivas.

**[INSERTAR AQUÍ MATRICES DE CONFUSIÓN O MÉTRICAS DEL MODELO]**

---

## Dashboard de Inteligencia de Negocios

Se desarrollaron dashboards interactivos en Looker Studio para monitorear indicadores clave relacionados con ventas, logística, inventario y desempeño de vendedores.

Indicadores destacados:

* Ventas totales.
* Número de pedidos.
* Tiempo promedio de entrega.
* Desempeño por categoría.
* Comportamiento de vendedores.

### Capturas del dashboard

**[INSERTAR AQUÍ CAPTURA GENERAL DEL DASHBOARD]**

**[INSERTAR AQUÍ CAPTURA DE KPIs PRINCIPALES]**

**[INSERTAR AQUÍ CAPTURA DE VISUALIZACIONES RELEVANTES]**

---

## Aplicación Interactiva

El proyecto incorpora una aplicación desarrollada en Streamlit que permite consultar resultados y explorar información analítica de forma interactiva.

### Capturas de la aplicación

**[INSERTAR AQUÍ CAPTURA DE LA PANTALLA PRINCIPAL]**

**[INSERTAR AQUÍ CAPTURA DE CONSULTAS O RESPUESTAS DEL AGENTE]**

---

## Resultados principales

* Construcción de un ecosistema analítico de extremo a extremo.
* Integración de múltiples fuentes de información.
* Implementación de modelos de Machine Learning para soporte a decisiones.
* Generación de dashboards ejecutivos para monitoreo operativo.
* Desarrollo de una aplicación interactiva para consulta de información.

---

## Mi contribución

Mis principales responsabilidades dentro del proyecto fueron:

* Limpieza y estandarización de datos utilizando Python, Pandas y NumPy.
* Validación y normalización de variables categóricas.
* Desarrollo de visualizaciones e indicadores clave de desempeño (KPIs).
* Diseño y construcción de dashboards en Looker Studio.

---

## Equipo del proyecto

Proyecto desarrollado de manera colaborativa como parte de un curso de Minería de Datos.

### Integrantes

* BERNAL MARTÍNEZ LUIS EDUARDO 
* DÍAZ LÓPEZ ALAN FERNANDO
* HERNÁNDEZ CASTILLO FERNANDA BERENICE
* MARTÍNEZ HERNÁNDEZ IRVIN
* MUÑOZ MARQUEZ ORTIZ ARTURO RAFAEL
* MERA MONTIEL GONZALO SEBASTIÁN
* ROSAS GONZÁLEZ MIGUEL ÁNGEL
* VAN STEENBERGHE LUJÁN KRISTOFFER
* VILCHIS LOPEZ VICTOR MANUEL

---

## Estructura del repositorio

```text
smart-supply-chain-analytics/
│
├── data/
├── notebooks/
├── models/
├── dashboard/
├── app/
├── docs/
├── images/
└── README.md
```

---

## Autoría y créditos

Este proyecto fue desarrollado de forma colaborativa por los integrantes del equipo. La sección "Mi contribución" describe específicamente las actividades realizadas por Alan Díaz dentro del proyecto.
