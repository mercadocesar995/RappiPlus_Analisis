# RappiPlus_Analisis

## RappiPlus — Análisis de Ventas, Rentabilidad y Comportamiento de Usuarios
Objetivo del proyecto

Este proyecto analiza el desempeño comercial de RappiPlus a partir de información de pedidos, productos, costos, marketing y comportamiento de usuarios.

El objetivo principal es evaluar las ventas y rentabilidad del negocio, identificar problemas de calidad en los datos y analizar el comportamiento de los usuarios durante el proceso de compra.

Además, se realizó un experimento A/B para evaluar si una modificación en la interfaz de checkout generaba diferencias en la tasa de conversión.

El proyecto combina análisis exploratorio, limpieza y validación de datos, consultas SQL, análisis estadístico y visualización en Power BI.

## Conjunto de datos utilizado

### El proyecto utiliza tres conjuntos de datos principales:



**1. Pedidos**

Contiene 25.100 registros y 12 variables relacionadas con las órdenes realizadas en la plataforma.

Variables principales:

**id_pedido**: identificador del pedido.

**id_usuario**: identificador del usuario.

**fecha_hora_pedido**: fecha y hora del pedido.

**pais**: país asociado al pedido.

**dispositivo**: dispositivo utilizado.

**fuente_referencia**: fuente de adquisición o referencia.

**nombre_producto**: producto comprado.

**categoria_producto**: categoría del producto.

**cantidad**: cantidad de unidades del pedido.

**precio_unitario**: precio por unidad.

**monto_descuento**: descuento aplicado.

**monto_total**: valor total del pedido.






**2. Catálogo de productos**

Contiene información sobre los productos comercializados:

**nombre_producto**: nombre del producto.

**categoria_producto**: categoría.

**costo_unitario**: costo del producto.

**proveedor**: proveedor asociado.






**3. Marketing**

Contiene información sobre la inversión en campañas:

**fecha**: fecha de la inversión.

**pais**: país.

**id_campaña**: identificador de la campaña.

**canal**: canal de marketing.

**gasto**: inversión realizada.

También se utilizó información de eventos de usuarios y un conjunto de datos correspondiente al experimento A/B del checkout.





### Herramientas utilizadas

**Python**

**Pandas**

**NumPy**

**Matplotlib**

**Seaborn**

**SQL**

**SciPy**

**Power BI**

**DAX**

**Power Query**

**Jupyter Notebook**

**Google Colab**

**GitHub**





### Etapas del análisis



**1. Exploración y validación inicial**

Se realizó una revisión inicial de los conjuntos de datos para identificar:

Dimensiones de las tablas.

Tipos de datos.

Valores faltantes.

Registros duplicados.

Estadísticas descriptivas.

Rangos de las variables numéricas.

Valores atípicos.

Posibles inconsistencias entre variables.

En la tabla de pedidos se identificaron 100 registros duplicados, además de valores faltantes en algunas variables.





**2. Limpieza y calidad de datos**

Se realizaron procesos de limpieza y validación para preparar los datos para el análisis.

Entre las principales revisiones se encontraron:

100 registros duplicados.

Valores faltantes en diferentes variables.

4 registros con cantidades negativas.

10 registros con cantidades superiores a 100 unidades.

Los 10 registros con cantidades extremas correspondían al producto Laptop-Gaming-16GB.

Se identificaron inconsistencias entre el monto total y el cálculo esperado a partir de cantidad, precio y descuento.

Los registros con cantidades extremas fueron excluidos de los análisis financieros para evitar que distorsionaran los resultados.





**3. Análisis exploratorio de ventas**

Se analizaron diferentes dimensiones del desempeño comercial:

Ingresos.

Costos.

Beneficio.

Unidades vendidas.

Pedidos.

Ticket promedio.

Productos por pedido.

Categorías de producto.

País.

Dispositivo.

Fuente de referencia.

El análisis permitió construir indicadores para evaluar el desempeño comercial y la rentabilidad.





**4. Análisis del comportamiento de usuarios**

Se analizaron las diferentes etapas del recorrido del usuario:

Primera visita.

Selección de producto.

Agregado al carrito.

Inicio del checkout.

Ingreso de información de pago.

Compra.

Se comparó el número de usuarios registrados en cada evento para identificar diferencias en el comportamiento a lo largo del proceso.

Nota: los usuarios registrados en cada evento no representan necesariamente subconjuntos secuenciales de los mismos usuarios, por lo que estos datos deben interpretarse como usuarios únicos por etapa y no como un funnel secuencial tradicional.





**5. Análisis estadístico y experimento A/B**

Se realizó un experimento A/B para evaluar una modificación en la interfaz del proceso de checkout.

Se compararon:

Grupo Control.

Grupo Treatment.

Tasa de conversión.

Diferencia entre grupos.

Estadístico Z.

Valor p.

Resultado

La tasa de conversión observada fue:

Control: 15,69 %
Treatment: 16,29 %
Diferencia: +0,60 puntos porcentuales
p-value: 0,416

Con un nivel de significancia de 0,05, no se encontró evidencia estadística suficiente para afirmar que la modificación del checkout haya producido una diferencia significativa en la conversión.





**6. Análisis en Power BI**

Los resultados del análisis fueron utilizados para construir un dashboard interactivo en Power BI.

El dashboard permite analizar:

Ingresos.

Costos.

Beneficio.

Gasto de marketing.

Pedidos.

Unidades vendidas.

Ticket promedio.

Productos por pedido.

Evolución mensual.

Desempeño por país.

Categorías de producto.

Fuentes de referencia.

Comportamiento de usuarios.

Se utilizaron DAX y Power Query para la construcción de métricas, transformación de datos y análisis dentro del modelo.





### Principales hallazgos

Calidad de datos

Se identificaron problemas de calidad relacionados con duplicados, valores faltantes, cantidades negativas y registros extremos que podían distorsionar el análisis financiero.

Ventas y rentabilidad

Después de excluir los registros con cantidades no válidas o extremas, se obtuvo una base más consistente para analizar ingresos, costos, unidades y rentabilidad.

Comportamiento de usuarios

El análisis permitió identificar diferencias en el número de usuarios registrados en las diferentes etapas del recorrido de compra y explorar dónde se concentran las mayores variaciones.

Experimento A/B

La variante del checkout presentó una conversión ligeramente superior a la del grupo Control (+0,60 puntos porcentuales), pero la prueba estadística no mostró evidencia suficiente de una diferencia significativa.





### Conclusiones

El proyecto permitió desarrollar un flujo completo de análisis de datos, desde la exploración y validación de la información hasta el análisis estadístico y la visualización de resultados en Power BI.

Uno de los principales aprendizajes fue la importancia de revisar la calidad de los datos antes de utilizar la información para calcular indicadores o generar conclusiones.

El proyecto también permitió combinar análisis comercial, comportamiento de usuarios y experimentación A/B para obtener una visión más completa del desempeño de RappiPlus.





### Cómo ejecutar el proyecto

### Power BI

Abre el archivo:

dashboard/RappiPlus_Dashboard.pbix

El dashboard contiene las métricas y visualizaciones desarrolladas a partir de los datos procesados.
