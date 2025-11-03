🧹 Proyecto de Limpieza de Datos con Python y Pandas
📘 Descripción

Este proyecto tiene como objetivo practicar las principales fases del análisis y limpieza de datos utilizando Python 🐍 y la librería Pandas 🐼.
El propósito es transformar datos crudos en un conjunto limpio, estructurado y listo para el análisis.

🔧 Tecnologías utilizadas

Python 3.x 🐍

Pandas 📊

NumPy 🔢

Jupyter Notebook 📓

🚀 Fases del Proceso de Limpieza de Datos
1️⃣ Importación y carga de datos

Importar librerías esenciales (pandas, numpy).

Cargar los archivos en un DataFrame (pd.read_csv, pd.read_excel, etc.).

Revisar la estructura con head(), info() y describe().

import pandas as pd
import numpy as np

datos = pd.read_csv('archivo.csv')
datos.head()

2️⃣ Exploración inicial 👀

Identificar tipos de datos.

Detectar valores nulos, duplicados o inconsistencias.

Revisar estadísticas generales y outliers.

datos.info()
datos.describe()
datos.isnull().sum()

3️⃣ Limpieza de datos 🧼

Eliminar o imputar valores faltantes (dropna(), fillna()).

Corregir tipos de datos (astype()).

Quitar duplicados (drop_duplicates()).

Estandarizar formatos (por ejemplo, texto en minúsculas o fechas).

datos = datos.drop_duplicates()
datos['columna'] = datos['columna'].fillna(datos['columna'].mean())

4️⃣ Normalización y transformación ⚙️

Crear nuevas columnas derivadas.

Normalizar o escalar valores numéricos.

Codificar variables categóricas (One-Hot Encoding, Label Encoding).

datos['nueva_columna'] = datos['columna_a'] / datos['columna_b']

5️⃣ Verificación final ✅

Confirmar que no haya valores nulos ni duplicados.

Comprobar coherencia de tipos y rangos.

Guardar el dataset limpio para análisis o modelado.
