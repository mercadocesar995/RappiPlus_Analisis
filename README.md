# RappiPlus_Analisis

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![SQL](https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sql.com/)

## 🎯 Objetivo del Proyecto
Analizar el desempeño comercial y la rentabilidad de **RappiPlus** mediante el procesamiento de **25,100+ pedidos**, evaluando la calidad de los datos, el comportamiento de los usuarios en el embudo de compra y validando estadísticamente un experimento A/B en el proceso de checkout.

---
❓ **Preguntas clave**

¿Cómo se comportan las ventas, costos y rentabilidad?

¿La calidad de los datos permite realizar un análisis financiero confiable?

¿En qué etapas del proceso de compra se concentran las diferencias en usuarios?

¿La modificación del checkout genera una diferencia en la tasa de conversión?


---
🔎 **Metodología**

1. **Calidad de datos**
Exploración, limpieza y validación de 25.100 pedidos, identificando duplicados, valores faltantes, cantidades negativas, registros extremos e inconsistencias entre variables.

2. **Análisis comercial**
Evaluación de ingresos, costos, beneficio, pedidos, unidades, ticket promedio, productos, categorías, países, dispositivos y fuentes de referencia.

3. **Comportamiento de usuarios**
Análisis de eventos desde la primera visita hasta la compra para identificar diferencias en las distintas etapas del proceso.

4. **A/B Testing**
Comparación de las tasas de conversión de Control vs. Tratamiento mediante una prueba de proporciones.

5. **Business Intelligence**
Construcción de un dashboard en Power BI, utilizando DAX y Power Query para transformar datos y desarrollar KPIs.


---
## 🛠️ Tech Stack & Metodología
* **Data Quality & Prep:** Python (Pandas, NumPy) para limpieza de inconsistencias, deduplicación y filtrado de atípicos.
* **Estadística & A/B Testing:** SciPy para pruebas de hipótesis e inferencia estadística (conversión de checkout).
* **Business Intelligence:** Power BI, DAX y Power Query para el modelado de datos y desarrollo de KPIs comerciales.

---

## 📊 Principales Hallazgos & Resultados

### 1. Calidad de Datos & Finanzas
* Se identificaron y depuraron **100 registros duplicados** y **10 atípicos extremos** (ventas masivas de *Laptop-Gaming-16GB*), garantizando un análisis financiero sin distorsiones en los márgenes de beneficio.

### 2. Experimento A/B (Rediseño de Checkout)
Se evaluó el impacto de la modificación del checkout sobre la tasa de conversión global

> **Conclusión Estadística:** A pesar del incremento observado del +0.60%, el $p\text{-value} > 0.05$ demuestra que **no existe evidencia estadística suficiente** para afirmar que el nuevo checkout supere al anterior. Se recomendó no implementar el cambio sin iterar la propuesta.

---

## 🔗 Enlaces del Proyecto

* 📊 **[Ver Dashboard Interactivo en Power BI]** https://app.powerbi.com/view?r=eyJrIjoiMjRiOTk0OGMtNDgxMy00YWM0LWE0YTUtOTEzYzEwYzBkMDZmIiwidCI6ImQ1MTM4OGVmLTZhYjAtNDM2My05Zjk0LWQ1NjY0NGE0NTk3MCIsImMiOjR9 **
* 📁 **[Explorar Cuadernos de Análisis y Código en Python](./notebooks)
