# Telecom X - Análisis de Evasión de Clientes

Este proyecto lo desarrollé para analizar el comportamiento de abandono de clientes (churn) en una empresa de telecomunicaciones. A partir de un dataset realista, busqué identificar patrones y variables clave que puedan ayudar a la empresa a anticipar la pérdida de usuarios y tomar decisiones estratégicas.

## 📥 Extracción de Datos

Primero, realicé la carga de datos directamente desde un archivo JSON alojado en GitHub. Para ello utilicé requests junto con pandas, "https://raw.githubusercontent.com/sthemonica/alura-voz/refs/heads/main/Dados/Telco-Customer-Churn.json".

## 🧹 Transformación de Datos

Después de importar el dataset en formato JSON, identifiqué que varias columnas estaban estructuradas como diccionarios anidados. Para poder analizarlas de forma efectiva, aplané estos campos y los convertí en columnas individuales utilizando herramientas de pandas. 

Posteriormente realicé una limpieza completa sobre el dataframe, que incluyó:

1. Conversión de la columna Charges.Total a tipo numérico (float), ya que originalmente estaba en formato object.

2. Identificación de valores nulos reales en Charges.Total (11 registros), los cuales podrían deberse a errores de entrada o clientes nuevos sin cobros acumulados. Por ahora los mantengo para análisis posterior.

3. Verificación de valores únicos y atípicos en columnas categóricas como Contract, InternetService, PaymentMethod, entre otras.

4. Validación de consistencia en la columna Churn, asegurando que no existan valores vacíos o desconocidos.

Estas transformaciones dejaron el dataset listo para el análisis exploratorio.

## 📈 Análisis Exploratorio (EDA)

Durante el EDA, identifiqué relaciones importantes entre la cancelación de clientes y ciertas variables, tales como:

- Clientes con contrato "Month-to-month" tienden a cancelar más.

- El método de pago "Electronic check" está asociado con un mayor churn.

- La ausencia de servicios como OnlineSecurity o TechSupport también muestra correlación con cancelaciones.

Incluí visualizaciones con matplotlib y seaborn para ilustrar estas tendencias.


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

