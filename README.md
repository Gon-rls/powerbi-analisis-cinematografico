#  Dashboard de Análisis Cinematográfico — Power BI

Dashboard interactivo desarrollado en Power BI que analiza el rendimiento económico y de crítica de un conjunto de películas: recaudación, presupuesto, puntuación media, género, país y evolución temporal.

**Realizado por:** Gonzalo Rodrigáñez Lorente-Sorolla



##  Objetivo del proyecto

Construir un dashboard de una sola página que permita explorar de forma dinámica el mercado cinematográfico, respondiendo a preguntas como:

- ¿Qué películas y géneros generan más recaudación?
- ¿Existe relación entre presupuesto invertido y recaudación obtenida?
- ¿Qué géneros reciben mejor puntuación media?
- ¿Cómo ha evolucionado la recaudación del sector entre 1980 y 2020?

##  Datos

Tabla única `movies` con los siguientes campos:

| Campo | Descripción |
|---|---|
| `name` | Título de la película |
| `genre` | Género cinematográfico |
| `country` | País de producción |
| `year` | Año de estreno |
| `budget` | Presupuesto de producción |
| `gross` | Recaudación obtenida |
| `score` | Puntuación / valoración |
| `rating` | Clasificación por edades |

Se creó además una medida DAX personalizada para el **ROI** (`SUM(gross) / SUM(budget)`).

##  KPIs principales

| Indicador | Valor |
|---|---|
| Total de películas | 7.668 |
| Recaudación total | 6 bill. |
| Nota media | 63,90 |
| Presupuesto medio | 355,90 mill. |
| ROI | 3 |

##  Visualizaciones

- **Top 10 Películas más Taquilleras** — ranking por recaudación
- **Recaudación por Género** — comparativa por género
- **Presupuesto vs Recaudación** — diagrama de dispersión (correlación)
- **Puntuación Media por Género** — valoración de crítica por género
- **Recaudación por Año** — evolución temporal (1980–2020)

##  Filtros interactivos

- Clasificación (rating)
- País de producción
- Género
- Rango de años (slider 1980–2020)

##  Conclusiones

- El género **Action** concentra la mayor parte de la recaudación, muy por encima del resto.
- Existe correlación positiva entre presupuesto y recaudación, con dispersión en los tramos altos.
- La crítica no siempre coincide con la taquilla: géneros como *History* o *Musical* puntúan mejor de media.
- La recaudación global crece de forma sostenida hasta un pico marcado en torno a 2008.

##  Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `Power_Bi_Trabajo_Cinematografico.pbix` | Archivo original de Power BI (requiere Power BI para abrirse) |
| `Documentacion_Proyecto_PowerBI_Cine.docx` | Documentación completa del proyecto |


##  Herramientas utilizadas

Power BI · Power Query · DAX 
