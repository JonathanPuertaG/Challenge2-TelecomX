# Telecom X - Análisis de Evasión de Clientes

## 💡Acerca del desafío 💡

Este proyecto lo desarrollé para analizar el comportamiento de abandono de clientes (churn) en una empresa de telecomunicaciones. A partir de un dataset realista, busqué identificar patrones y variables clave que puedan ayudar a la empresa a anticipar la pérdida de usuarios y tomar decisiones estratégicas.

## 📥 Extracción de Datos

Primero, realicé la carga de datos directamente desde un archivo JSON alojado en GitHub. Para ello utilicé requests junto con pandas, "https://raw.githubusercontent.com/sthemonica/alura-voz/refs/heads/main/Dados/Telco-Customer-Churn.json".

También realicé una validación inicial del dataset, identificando:
- Total de registros: {{df.shape[0]}}
- Total de columnas: {{df.shape[1]}}
- Tipos de datos y columnas cargadas correctamente.


## 🧹 Transformación de Datos

Después de importar el dataset en formato JSON, identifiqué que varias columnas estaban estructuradas como diccionarios anidados. Para poder analizarlas de forma efectiva, aplané estos campos y los convertí en columnas individuales utilizando herramientas de pandas. 

Esto permitió estructurar correctamente la información para el análisis exploratorio y las visualizaciones.



## 🔧 Requisitos

- Python 3.x
- Pandas
- Matplotlib / Seaborn
- Google Colab (recomendado para ejecución)

## 🚀 Instrucciones

1. Clona el repositorio.
2. Abre `Challenge Telecom X.ipynb` en Google Colab.
3. Ejecuta las celdas para ver el análisis completo y visualizaciones.

## 👤 Autor

Jonathan Puerta Gallego

