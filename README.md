# 🚦 Movilidad Urbana y Productividad Económica | Python

Proyecto de análisis de datos desarrollado en Python para estudiar la relación entre la movilidad urbana, la congestión vehicular y la productividad económica de distintas ciudades.

El análisis integra información de TomTom Traffic Index y OECD Cities, combinando indicadores de tráfico con variables económicas para identificar patrones y posibles oportunidades de inversión en infraestructura de transporte.

---

## 🎯 Objetivo del proyecto

Analizar la relación entre la congestión urbana y distintos indicadores económicos durante 2024, con el propósito de identificar ciudades donde los problemas de movilidad podrían estar relacionados con limitaciones en productividad y competitividad urbana.

El proyecto busca responder preguntas como:

- ¿Qué ciudades presentan mayores niveles de congestión?
- ¿Existe relación entre el PIB per cápita y los niveles de tráfico?
- ¿Qué ciudades presentan altos niveles de congestión en comparación con sus indicadores económicos?
- ¿Qué territorios podrían requerir mayor atención en materia de infraestructura de transporte?

---

## 🗂️ Fuentes de datos

Para el análisis se utilizaron dos conjuntos de datos:

- **TomTom Traffic Index:** información relacionada con congestión, retrasos, tráfico y tiempos de traslado.
- **OECD Cities:** información económica y urbana como PIB per cápita, desempleo, población y contaminación ambiental.

Los datos fueron filtrados para trabajar con información correspondiente al año 2024.

---

## 🛠️ Herramientas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🧹 Preparación y limpieza de datos

Antes de realizar el análisis se exploró la estructura de los datasets para identificar tipos de datos, formatos inconsistentes y posibles valores ausentes.

Entre las principales transformaciones realizadas se encuentran:

- Estandarización de nombres de columnas.
- Conversión de variables de fecha a formato datetime.
- Conversión de variables económicas almacenadas como texto a valores numéricos.
- Corrección de separadores decimales y de miles.
- Creación de la variable de población total.
- Extracción del año a partir de las fechas.
- Filtrado de los registros correspondientes a 2024.

Estas transformaciones permitieron obtener información consistente y preparada para el análisis.

---

## 🔗 Integración de datos

Los registros de tráfico fueron agrupados por ciudad, país y año para calcular indicadores promedio de movilidad.

Posteriormente, la información de tráfico y economía fue integrada utilizando las variables `city` y `year` como claves de unión.

Se utilizó una unión `INNER`, conservando únicamente las ciudades presentes en ambos conjuntos de datos.

Esto permitió construir un dataset unificado con indicadores como:

- Retrasos por congestión.
- Índice de tráfico.
- Longitud y cantidad de congestionamientos.
- Tiempos de traslado.
- PIB per cápita.
- Desempleo.
- Población.
- Contaminación ambiental.

---

## 📊 Análisis de movilidad urbana

El análisis permitió comparar los niveles promedio de congestión entre diferentes ciudades durante 2024.

Uno de los principales hallazgos fue que **Ciudad de México presentó el mayor promedio de `jams_delay` dentro del conjunto analizado**, seguida por ciudades como Tokio, Nueva York y Londres.

Este resultado permite identificar ciudades donde la presión sobre la infraestructura de movilidad es especialmente elevada.

---

## 📈 Movilidad y productividad económica

Para explorar la relación entre movilidad y economía se analizaron conjuntamente los indicadores de congestión y PIB per cápita.

Los resultados muestran que no existe una relación completamente lineal entre ambas variables.

Algunas ciudades con altos niveles de PIB per cápita también presentan congestión considerable, mientras que otras ciudades con indicadores económicos menores presentan problemas importantes de movilidad.

Esto sugiere que factores adicionales como infraestructura vial, densidad poblacional, transporte público y planeación urbana pueden influir en los niveles de congestión.

---

## 🔎 Hallazgos principales

- La congestión urbana presenta diferencias importantes entre ciudades.
- Ciudad de México destacó por sus elevados niveles promedio de retraso por congestión.
- Un mayor PIB per cápita no necesariamente implica mejores condiciones de movilidad.
- Algunas ciudades presentan niveles de congestión elevados en comparación con sus indicadores económicos.
- La movilidad urbana debe analizarse junto con factores económicos, demográficos y de infraestructura.

---

## 💡 Recomendaciones

Los resultados sugieren priorizar análisis más profundos en ciudades donde coinciden altos niveles de congestión con indicadores económicos moderados o bajos.

Ciudades como Bogotá, Lima y Buenos Aires pueden representar casos relevantes para futuras investigaciones relacionadas con infraestructura de transporte y movilidad urbana.

También sería recomendable incorporar variables adicionales como cobertura de transporte público, parque vehicular, crecimiento urbano y distribución territorial del empleo.

---

## 📸 Evidencias del proyecto

### 🧹 Evidencia 1 — Preparación y limpieza de datos

<img width="1345" height="661" alt="image" src="https://github.com/user-attachments/assets/45c307e0-cff8-461e-a82a-e46f38578d4a" />
<img width="820" height="362" alt="image" src="https://github.com/user-attachments/assets/b4659fc3-7f88-4a45-af62-155269ebf09b" />

La preparación de los datos incluyó la conversión de fechas, corrección de formatos numéricos y transformación de variables económicas para garantizar su correcta utilización durante el análisis.

### 🔗 Evidencia 2 — Integración de movilidad y economía

<img width="1355" height="651" alt="image" src="https://github.com/user-attachments/assets/ff444a95-0556-461f-bf2a-6084414d3383" />
<img width="1372" height="241" alt="image" src="https://github.com/user-attachments/assets/5a5a9aa0-9141-4124-9387-6036edbf0279" />

Los datasets de movilidad y economía fueron integrados mediante una unión INNER utilizando ciudad y año como claves, generando una base consolidada para el análisis.

### 📊 Evidencia 3 — Análisis de movilidad urbana

<img width="1367" height="475" alt="image" src="https://github.com/user-attachments/assets/8c67f3a6-f544-450b-96d1-46c7db8937d7" />

El análisis comparativo permitió identificar las ciudades con mayores niveles promedio de congestión durante 2024, destacando Ciudad de México entre los valores más elevados.

### 📈 Evidencia 4 — Relación entre tráfico y economía

<img width="1377" height="587" alt="image" src="https://github.com/user-attachments/assets/a95423d6-880c-4d38-9c39-b4f1e284d853" />

La visualización conjunta de los indicadores permitió explorar la relación entre congestión vehicular y PIB per cápita, mostrando que no existe una relación lineal directa entre ambas variables.

---

## 💡 Aprendizajes

Este proyecto me permitió fortalecer el proceso completo de preparación y análisis de datos con Python, desde la exploración inicial y limpieza hasta la integración de diferentes fuentes y generación de visualizaciones.

También reforcé el uso de Pandas para transformar, agrupar y combinar información, así como Matplotlib y Seaborn para comunicar patrones y hallazgos mediante visualizaciones.

El proyecto permitió comprender la importancia de conectar los resultados técnicos con preguntas de negocio y utilizar los datos como apoyo para la toma de decisiones.

---

## 👤 Autor

**José Alberto Contreras Ramos**

Data Analyst | Business Intelligence
