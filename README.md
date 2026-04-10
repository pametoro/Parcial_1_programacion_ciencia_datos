# Parcial_1_programación_ciencia_datos

Introducción


En el ámbito de la ciencia de datos, la capacidad de transformar registros crudos en estructuras de información optimizadas es fundamental para garantizar modelos predictivos precisos. El presente estudio técnico se enfoca en el análisis, limpieza y transformación del conjunto de datos Food_Preference.csv, el cual documenta las tendencias de consumo alimentario de una población diversa, integrando dimensiones demográficas y preferencias de dieta.


"Tras una exploración inicial del dataset, se identificaron anomalías críticas como valores de edad fuera de rango lógico (-47 y 263 años) y una presencia significativa de valores nulos en variables demográficas clave. El presente análisis abordará estas inconsistencias mediante vectorización para la limpieza de datos y pivoteo para la síntesis de información, garantizando un procesamiento eficiente de los 290 registros iniciales."


El desarrollo de este trabajo no solo se limita a la exploración estadística, sino que implementa una arquitectura de procesamiento basada en las siguientes técnicas de optimización:

Vectorización y Eficiencia Computacional: 

Se reemplazan estructuras iterativas por operaciones vectorizadas (vía NumPy y Pandas) para el tratamiento de valores atípicos (outliers) y la imputación de datos faltantes detectados en variables críticas como Age y Gender.

Pipeline de Transformación: 

Se utiliza ColumnTransformer para aplicar técnicas de One-Hot Encoding y Escalamiento, garantizando que la memoria se gestione de forma eficiente al procesar variables categóricas y numéricas simultáneamente.

Estrategia de Chunking: 

Se establece como protocolo de escalabilidad para permitir que el análisis sea replicable en entornos de Big Data, evitando cuellos de botella en la memoria RAM.


Detección de Outliers: 

Al análizarlos uno de los mas evidentes es el valor mínimo de edad es -47 y el máximo 263.


