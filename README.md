# Proyecto de Limpieza de Datos: **Heart Disease**

Este proyecto tiene como objetivo limpiar y preparar el **Heart Disease dataset** para su análisis y modelado posterior. A través de este proceso, se abordan problemas comunes de calidad de los datos, como valores nulos, errores en la codificación y transformación de variables, para garantizar que los datos estén listos para un análisis más profundo o construcción de modelos de machine learning.

## Descripción del Dataset

El **Heart Disease Dataset** es un conjunto de datos que contiene información sobre pacientes y su diagnóstico de enfermedades cardíacas. Las características incluyen variables como edad, sexo, presión arterial, colesterol, resultados de pruebas médicas y diagnósticos de enfermedades cardíacas. El dataset se encuentra disponible en la [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+disease).

## Objetivos del Proyecto

- **Limpieza de Datos:** Preparar el conjunto de datos eliminando inconsistencias, manejando valores nulos y transformando las variables de manera adecuada.
- **Transformación de Variables:** Convertir variables categóricas a valores descriptivos y transformar variables numéricas cuando sea necesario.
- **Preprocesamiento para Análisis:** Asegurarse de que el conjunto de datos esté listo para análisis exploratorio y modelado.

## Pasos Realizados en la Limpieza de Datos

1. **Exploración Inicial de Datos**
    - Inspección de los tipos de datos y la existencia de valores nulos.
    - Análisis de las variables categóricas y numéricas.
2. **Tratamiento de Valores Nulos**
    - Se identificaron las columnas con valores nulos.
    - Las variables categóricas con pocos valores nulos fueron reemplazadas por la **moda** de la columna.
3. **Conversión de Variables Categóricas**
    - Se transformaron las variables que originalmente eran representadas con números a categorías descriptivas (por ejemplo, "typical angina", "asymptomatic", etc.) para una mayor claridad.
4. **Transformación de la Variable `heart_disease`**
    - La variable `heart_disease` fue convertida en una variable binaria:
        - **0** se convierte en **'absence'** (ausencia de enfermedad).
        - Los valores mayores a 0 se convierten en **'presence'** (presencia de enfermedad).
5. **Revisión de Tipos de Datos**
    - Se realizaron conversiones de tipo de datos para asegurar que todas las columnas tuvieran el tipo correcto (por ejemplo, convertir columnas con números almacenados como `object` a tipo `float64`).

## Resultados Esperados

- **Dataset Limpio:** Después de aplicar estos pasos, el dataset está limpio y listo para ser usado en análisis o modelos predictivos.
- **Transformación de Variables:** Las variables categóricas han sido transformadas a valores descriptivos, y la variable `heart_disease` ha sido simplificada a una variable binaria de presencia/ausencia.

## Requisitos

Para ejecutar el notebook y realizar la limpieza de datos, asegúrate de tener instaladas las siguientes bibliotecas en Python:

- `pandas`
- `numpy`

Puedes instalar estas bibliotecas utilizando pip:

```bash
pip install pandas numpy
```

## Ejecución del Proyecto

1. Clona o descarga este repositorio.
2. Abre **data-cleaning.ipynb** en Jupyter Notebook.
3. Ejecuta las celdas para realizar el proceso de limpieza de datos.
4. Una vez que los datos estén limpios, puedes continuar con el análisis exploratorio o la construcción de modelos de machine learning.

## Conclusiones

Este proyecto tiene como objetivo proporcionar una base sólida para el análisis de datos o modelado de predicción relacionados con las enfermedades cardíacas, garantizando que el dataset esté libre de problemas comunes de calidad de datos.

## Atribución

Si usas los datos de este proyecto o cualquier parte del conjunto de datos, por favor da el crédito correspondiente de acuerdo con la licencia **CC BY 4.0**, como sigue:

> "Heart Disease" por la UC Irvine Machine Learning Repository, disponible en [https://archive.ics.uci.edu/dataset/45/heart+disease](https://archive.ics.uci.edu/dataset/45/heart+disease). Licencia: **CC BY 4.0**.