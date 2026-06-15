Exploración, limpieza y segmentación de clientes de una empresa de telecomunicaciones para identificar patrones de uso y oportunidades de monetización.

Este proyecto realiza un análisis exploratorio completo sobre la base de clientes de ConnectaTel, una empresa de telecomunicaciones con planes Básico y Premium. El objetivo es entender el comportamiento de los usuarios, detectar problemas de calidad en los datos y generar segmentos accionables para el equipo de negocio.

Distribuciones analizadas

Edad (age): Distribución uniforme entre 18–79 años (mediana: 48). Sin outliers. Posible muestreo balanceado del dataset.
Cantidad de mensajes (cant_mensajes): Sesgada a la derecha. Mediana: 5. Outliers reales en 12–17 mensajes.
Cantidad de llamadas (cant_llamadas): Sesgada a la derecha. Mediana: 4. Outliers reales en 11–15 llamadas.
Minutos de llamada (cant_minutos_llamada): Alta dispersión (std: 18.17). Mediana: 19.78 min. Cluster anómalo entre 130–160 min que requiere validación.

Conclusiones y recomendaciones

Planes diferenciados por segmento etario: beneficios digitales para jóvenes, paquetes balanceados para adultos y enfoque en llamadas + simplicidad para adultos mayores.
Campaña de upsell para usuarios de alto uso: son los más activos pero no están en Premium — son el segmento de mayor potencial de conversión.
Monitoreo del cluster 130–160 min: investigar si son registros válidos o errores de captura antes de incluirlos en modelos predictivos.
Validaciones en sistemas de captura: prevenir valores sentinel, ciudades inválidas ("?") y nulos masivos en columnas críticas como duration y length.
Análisis temporal: excluir 2026 de tendencias históricas hasta contar con el año completo.

Tecnologías utilizadas

Python
Pandas
Seaborn
Matplotlib
Jupyter Notebook
