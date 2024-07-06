# Proyecto Final de Ciencia de Datos: Clasificación de Niveles de Obesidad

## Descripción del Proyecto

Este proyecto se centra en la creación de un modelo de clasificación multiclase para predecir el nivel de obesidad de un individuo basado en sus hábitos de vida y características personales. Utilizando datos del dataset "ObesityDataSet", se desarrollan y comparan varios modelos de clasificación para identificar el más efectivo.

## Contenido del Repositorio

- `ObesityDataSet.csv`: El conjunto de datos utilizado para entrenar y evaluar los modelos.
- `ProyectoDS_Barra.ipynb`: La primera parte del proyecto que incluye la limpieza de datos y el análisis exploratorio de datos (EDA).
- `ProyectoDS_ParteI_Barra.ipynb`: La segunda parte del proyecto que incluye la selección de características y la implementación de los modelos de clasificación.
- `README.md`: Este archivo, que proporciona una visión general del proyecto.

## Objetivo del Proyecto

El objetivo principal de este proyecto es desarrollar un modelo de clasificación multiclase que pueda predecir el nivel de obesidad de un individuo. Las hipótesis específicas exploradas incluyen:

1. Existe una correlación significativa entre la falta de actividad física y los niveles más altos de obesidad.
2. Los individuos más jóvenes tienden a tener mayores problemas de obesidad.

## Contexto Comercial

Este análisis es crucial desde una perspectiva comercial y de salud pública debido a:

- **Salud Pública**: Ayuda a las autoridades sanitarias a diseñar programas más efectivos para combatir la obesidad.
- **Intervenciones Preventivas**: Ofrece recomendaciones personalizadas para reducir el riesgo de desarrollar obesidad.
- **Beneficios Económicos**: Disminuye los costos de atención médica asociados con la obesidad.
- **Desarrollo de Productos**: Orienta el desarrollo de productos y servicios en el sector de la alimentación y el fitness.

## Descripción de Variables

- `Gender`: Género del individuo.
- `Age`: Edad del individuo en años.
- `Height`: Altura del individuo en metros.
- `Weight`: Peso del individuo en kilogramos.
- `Family_history_with_overweight`: Antecedentes familiares de sobrepeso u obesidad.
- `FAVC`: Consumo frecuente de alimentos altamente calóricos.
- `FCVC`: Frecuencia de consumo de vegetales.
- `NCP`: Número de comidas principales al día.
- `CAEC`: Consumo de alimentos entre comidas.
- `SMOKE`: Si el individuo fuma o no.
- `CH2O`: Cantidad de agua consumida diariamente.
- `SCC`: Monitoreo del consumo de calorías.
- `FAF`: Frecuencia de actividad física semanal.
- `TUE`: Tiempo usando dispositivos tecnológicos cada día.
- `CALC`: Frecuencia de consumo de alcohol.
- `MTRANS`: Tipo de transporte más utilizado.
- `NObeyesdad`: Nivel de obesidad del individuo.

## Modelo de Clasificación Multiclase

### Paso 1: Preparar los Datos

- Codificación de variables categóricas.
- División del dataset en entrenamiento (60%), validación (20%) y prueba (20%).
- Escalado de características.

### Paso 2: Selección de Características

Utilizamos RFE con Random Forest para identificar las características más influyentes:
- `Height`
- `Weight`
- `FCVC`
- `BMI`
- `Gender_Male`

### Paso 3: Entrenamiento y Evaluación del Modelo

#### Modelo de Regresión Logística

- **Precisión General**: 92% en validación, 94% en prueba.
- **Desempeño por Categoría**: Desafíos específicos en las categorías "Normal Weight" y "Overweight_Level_I".
- **Matriz de Confusión**: Errores significativos en las categorías mencionadas.

#### Modelo Random Forest

- **Precisión General**: 98% en validación, 97.4% en prueba.
- **Desempeño por Categoría**: Alta precisión y recall en casi todas las categorías.
- **Consistencia**: Buen rendimiento en validación y prueba, sugiriendo buena generalización.

## Conclusión General

Este análisis exhaustivo demuestra que los modelos aplicados, especialmente Random Forest, son robustos y efectivos para la clasificación de tipos de obesidad y peso. Sin embargo, aún hay espacio para optimizaciones que podrían aumentar la fiabilidad y la aplicabilidad de estos modelos en contextos prácticos, mejorando su utilidad como herramientas en la prevención y manejo de la obesidad en entornos clínicos o de salud pública.

## Cómo Ejecutar el Proyecto

1. Clonar el repositorio.
2. Instalar dependencias necesarias.
3. Ejecutar los notebooks.

## Autor
- Rindolfo Barra Roa

## Agradecimientos
Agradecimientos a [CoderHouse](https://www.coderhouse.com/) por el curso de Data Science I, que proporcionó la base y estructura para este proyecto.
