# 🧠 Impacto de las Redes Sociales en la Salud Mental Adolescente
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mera-15/impacto_redes_salud_mental/blob/main/analisis_redes_salud_mental.ipynb)

## 📊 Contexto del Proyecto
Este proyecto es un Análisis Exploratorio de Datos (EDA) diseñado para investigar y cuantificar la relación empírica entre los hábitos de consumo de redes sociales y los indicadores de salud mental en adolescentes. 

### 📂 Fuente de Datos

El conjunto de datos utilizado para este análisis es de dominio público y fue obtenido a través de **Kaggle**. Puedes acceder al archivo original detallando las métricas en el siguiente enlace:
* [Impact of Social Media on Teen's Mental Health](https://www.kaggle.com/datasets/itszubi/impact-of-social-media-on-teens-mental-health)

## 🛠️ Herramientas y Tecnologías
* **Lenguaje:** Python
* **Manipulación y Limpieza de Datos:** Pandas
* **Visualización de Datos:** Plotly Express
* **Exploración Inicial:** ydata-profiling

## 📕 Diccionario de Datos

| Columna | Descripción |
| :--- | :--- |
| **age** | Edad del adolescente en años. |
| **gender** | Género del individuo. |
| **daily_social_media_hours** | Promedio de horas diarias invertidas en redes sociales. |
| **platform_usage** | Principal plataforma de red social utilizada. |
| **sleep_hours** | Promedio de horas de sueño por día. |
| **screen_time_before_sleep** | Horas de uso de pantallas antes de dormir. |
| **academic_performance** | Puntaje de rendimiento académico (GPA). |
| **physical_activity** | Nivel de actividad física diaria medida en horas. |
| **social_interaction_level** | Nivel de interacción social en el mundo real (bajo, medio, alto). |
| **stress_level** | Puntaje medido del nivel de estrés. |
| **anxiety_level** | Puntaje medido del nivel de ansiedad. |
| **addiction_level** | Puntaje de intensidad de adicción a las redes sociales. |
| **depression_label** | Variable binaria que indica la presencia de depresión (0 = No, 1 = Sí). |

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

### 3. Ejercicio Físico vs. Tiempo en Redes
* *Hipótesis:* *Existe una relación inversamente proporcional entre la frecuencia de ejercicio físico y el tiempo de uso de redes sociales.*
* *Hallazgo:* Al analizar el promedio de horas de actividad física frente a las horas diarias de uso de redes, no se observa ninguna correlación. Independientemente de si los adolescentes pasan 1 u 8 horas frente a las pantallas, el promedio de actividad física se mantiene constante y estable, rondando en todos los grupos aproximadamente 1 hora diaria (valores entre 0.94 y 1.11).
  * En la muestra analizada, el tiempo invertido en redes sociales no actúa como un factor de desplazamiento para el ejercicio físico. El nivel de sedentarismo o actividad se mantiene independiente del consumo digital.

<img width="1745" height="470" alt="Sin título3" src="https://github.com/user-attachments/assets/fe47a1d5-f29f-4c04-9d04-bbb89799d210" />

## 📂 Estructura del Repositorio
* `analisis_redes_salud_mental.ipynb`: Cuaderno de Google Colab con el código fuente, limpieza y visualizaciones interactivas.
* `reporte_salud_mental_adolescentes.html`: Reporte de diagnóstico general del dataset.

## 🚀 Cómo visualizar el proyecto
Para interactuar con los gráficos de Plotly, se recomienda descargar el cuaderno `.ipynb` y ejecutarlo en Google Colab o Jupyter Notebook, ya que GitHub renderiza los gráficos interactivos como imágenes estáticas.
