# 🧠 Impacto de las Redes Sociales en la Salud Mental Adolescente
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mera-15/impacto_redes_salud_mental/blob/main/analisis_redes_salud_mental.ipynb)

## 📊 Contexto del Proyecto
Este proyecto es un Análisis Exploratorio de Datos (EDA) diseñado para investigar y cuantificar la relación empírica entre los hábitos de consumo de redes sociales y los indicadores de salud mental en adolescentes. 

## 🛠️ Herramientas y Tecnologías
* **Lenguaje:** Python
* **Manipulación y Limpieza de Datos:** Pandas
* **Visualización de Datos:** Plotly Express
* **Exploración Inicial:** ydata-profiling

## 🔍 Hipótesis y Hallazgos Clave

**1. Relación entre Tiempo de Uso y Depresión**
* *Hipótesis:* A mayor cantidad de horas diarias invertidas en redes sociales, mayor es la tasa de depresión reportada.
* *Hallazgo:* El análisis de los datos revela que no existe una aparición de depresión en consumos menores a 5 horas diarias. Sin embargo, a partir de ese umbral, la proporción de casos comienza a escalar, alcanzando su pico máximo (10% de la muestra) en el grupo de usuarios con 8 horas de consumo diario. Esto sugiere que el riesgo aumenta significativamente en rangos de exposición extrema.

<img width="1743" height="465" alt="Sin título1" src="https://github.com/user-attachments/assets/dc2c85f8-a587-48f1-85ab-d3a2b7ce53e3" />

**2. Impacto del Género en la Depresión**
* *Hipótesis:* Ante niveles similares de uso, el género influye en la propensión a reportar síntomas.
* *Hallazgo:* Al desglosar la tasa de depresión por género en los grupos de alto consumo (5 horas o más), se observa una clara tendencia de vulnerabilidad diferenciada:
  * En los segmentos de **5, 6 y 7 horas diarias**, el porcentaje de mujeres con depresión supera consistentemente al de los hombres. (Por ejemplo, a las 5 horas de uso, la tasa en mujeres es del 6.1% frente al 3.1% en hombres). Curiosamente, en el pico máximo de uso registrado (8 horas diarias), la tendencia se invierte levemente, presentando los hombres una tasa de depresión mayor (10.7%) en comparación con las mujeres (9.1%).
En conclusión, la hipótesis se sostiene para la gran mayoría de los casos analizados. Existe una brecha de género donde las mujeres muestran mayor susceptibilidad a la depresión ante el mismo nivel de exposición a las redes, aunque en niveles de consumo extremo (8 horas), el impacto resulta severo para ambos géneros.

<img width="1745" height="473" alt="Sin título2" src="https://github.com/user-attachments/assets/81fd99bc-caf1-4e37-a161-001b004b2519" />

### 3. Ejercicio Físico vs. Tiempo en Redes (En proceso ⏳)
**Hipótesis:** *Existe una relación inversamente proporcional entre la frecuencia de ejercicio físico y el tiempo de uso de redes sociales.*

**Estado:** [Actualmente realizando el Análisis Exploratorio de Datos (EDA) para evaluar esta métrica y diseñar la visualización correspondiente.]

## 📂 Estructura del Repositorio
* `analisis_redes_salud_mental.ipynb`: Cuaderno de Google Colab con el código fuente, limpieza y visualizaciones interactivas.
* `reporte_salud_mental_adolescentes.html`: Reporte de diagnóstico general del dataset.

## 🚀 Cómo visualizar el proyecto
Para interactuar con los gráficos de Plotly, se recomienda descargar el cuaderno `.ipynb` y ejecutarlo en Google Colab o Jupyter Notebook, ya que GitHub renderiza los gráficos interactivos como imágenes estáticas.
