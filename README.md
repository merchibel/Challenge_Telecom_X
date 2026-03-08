📊 Telecom X - Análisis de Evasión de Clientes (Churn)
📌 Descripción del proyecto

Este proyecto forma parte del desafío "Churn de Clientes" de Telecom X, cuyo objetivo es analizar los factores que influyen en la evasión de clientes.

La empresa enfrenta una alta tasa de cancelaciones de servicios, por lo que resulta fundamental comprender el comportamiento de los clientes y detectar patrones asociados al abandono.

Para este análisis se realizó un proceso completo de ETL (Extracción, Transformación y Carga) y Análisis Exploratorio de Datos (EDA) utilizando Python y sus principales bibliotecas de análisis de datos.

Los resultados obtenidos permitirán al equipo de Data Science desarrollar modelos predictivos y estrategias de retención de clientes.

🎯 Objetivos del análisis

Importar datos desde una API en formato JSON.

Transformar los datos en un DataFrame de Pandas.

Realizar limpieza y preparación de datos (ETL).

Identificar inconsistencias y corregirlas.

Crear nuevas variables que aporten al análisis.

Explorar patrones asociados a la evasión de clientes.

Generar insights que apoyen futuras estrategias de retención.

📂 Fuente de datos

Los datos fueron obtenidos desde la API pública del desafío:

🔗
https://github.com/ingridcristh/challenge2-data-science-LATAM

Dataset utilizado:

TelecomX_Data.json

El dataset contiene información sobre:

datos demográficos de clientes

servicios contratados

facturación

tipo de contrato

método de pago

estado de evasión (Churn)

⚙️ Tecnologías utilizadas

Python

Google Colab

Pandas

NumPy

Matplotlib

Seaborn

Requests

🔄 Proceso de análisis
1️⃣ Extracción de datos

Los datos fueron obtenidos directamente desde la API utilizando la librería requests y posteriormente convertidos a un DataFrame de Pandas para facilitar su manipulación.

2️⃣ Exploración inicial de datos

Se realizó una revisión de:

columnas del dataset

tipos de datos

estructura general de la información

Se utilizaron funciones como:

df.info()
df.dtypes
df.describe()
3️⃣ Limpieza de datos

Se verificaron posibles problemas que pudieran afectar el análisis:

valores nulos

registros duplicados

inconsistencias en categorías

formatos incorrectos

Se utilizaron herramientas como:

isnull()
duplicated()
unique()
4️⃣ Transformación de datos

Se aplicaron diversas transformaciones para mejorar la calidad del dataset:

estandarización de texto

conversión de columnas numéricas

eliminación de valores faltantes

limpieza de categorías

5️⃣ Creación de nuevas variables

Se creó la variable:

Cuentas_Diarias

Esta variable estima el gasto diario del cliente a partir de su facturación mensual.

Cuentas_Diarias = MonthlyCharges / 30

Esto permite analizar con mayor precisión el comportamiento de consumo de los clientes.

📊 Análisis exploratorio de datos (EDA)

Durante el análisis se exploraron patrones relacionados con la evasión de clientes, evaluando variables como:

tipo de contrato

método de pago

cargos mensuales

antigüedad del cliente

Las visualizaciones permitieron identificar tendencias importantes en el comportamiento de los clientes.

💡 Insights principales

Algunos hallazgos relevantes incluyen:

Los clientes con contratos mensuales presentan mayor probabilidad de abandono.

Algunos métodos de pago muestran mayor asociación con churn.

Los clientes con menor antigüedad tienden a cancelar con mayor frecuencia.

Los niveles de facturación pueden influir en la decisión de abandono.

Estos insights pueden ser utilizados para diseñar estrategias de retención de clientes.

