# marketing_digital_ecommerce_validaci-n_hipotesis
Proyecto 8: Validando hipótesis de negocio con pruebas estadísticas

Como analista de datos en el equipo de marketing digital de una empresa de ecommerce se ejecutó un experimento A/B en la página de inicio (landing page), comparando dos versiones (A y B) con el objetivo de mejorar la tasa de conversión y el valor económico por usuario. La empresa necesitaba una decisión basada en datos para definir qué versión implementar, considerando la tasa de conversión, el gasto promedio y el comportamiento por canal de tráfico y tipo de usuario.

# Objetivo del proyecto

- Explorar, validar y analizar estadísticamente el experimento A/B para identificar diferencias significativas entre las páginas y traducir los resultados en recomendaciones para el negocio

- Responder a las siguientes preguntas de negocio:
¿Existe una diferencia significativa en el gasto promedio por usuario convertido entre ambas versiones?
¿Qué versión de la página (A o B) genera mayor tasa de conversión?
¿La conversión depende de la fuente de tráfico?
¿El tipo de usuario (nuevo o recurrente) influye en la conversión?
¿Qué hallazgos o insights permiten optimizar la estrategia de marketing y el diseño de la página de inicio (landing page)?

# Datasets utilizados

El archivo /datasets/landing_experiment.csv contiene información de usuarios expuestos a dos versiones de la página de inicio (landing page) dentro del experimento A/B. Para ello, se trabajó con una fuente de datos:

[df landing_experiment.csv] (https://drive.google.com/uc?export=download&id=15zGd_F-LzxCOcwNc74n_1x_o6OjAWYUV)

El dataset contiene las siguientes columnas:

user_id |	Categórica (UUID)	| Identificador único del usuario	| 26f3052e-8500-44ea-8fff-06de65258abb
date	| Fecha (YYYY-MM-DD) |	Fecha en la que el usuario fue expuesto a la página	| 2026-01-01
landing	| Categórica	| Versión de la página mostrada al usuario	| A, B
region	| Categórica	| Región geográfica del usuario	| Norte, Centro, Sur, Occidente, Oriente
dispositivo	| Categórica	| Tipo de dispositivo utilizado por el usuario	| Mobile, Desktop
traffic_source	| Categórica	| Canal por el que llegó el usuario	| Organic, Ads, Email, Referral
user_type	| Categórica	| Tipo de usuario según historial previo	| Nuevo, Recurrente
converted	| Binaria (0/1)	| Indica si el usuario realizó una conversión	| 0, 1
gasto	Numérica | (float)	| Monto gastado por el usuario (0 si no convirtió)	| 38.08



# Etapas del análisis realizadas

Paso Acción Resultado para el negocio (Flujo general del proyecto):

1. Cargar y validar datos	para dar confianza en la calidad del experimento
2. Comparar gasto promedio (A vs. B)	para identificar qué página genera más valor
3. Comparar tasa de conversión (A vs. B)	para identificar la página más efectiva
4. Analizar tráfico y conversión	para optimizar inversión en canales
5. Analizar tipo de usuario y conversión	para evaluar si segmentar usuarios
6. Visualización	para respaldar visualmente las conclusiones
7. Insight ejecutivo	para que los stakeholders decidan con claridad


# Cómo ejecutar el notebook

Abrirlo en Google Colab o desde el repositorio de GitHub
Si se desea de pueden cargar los datasets manualmente descargando los archivos desde los links anexados inicialmente o simplemente ejecutar las lineas mencionadas


# Guía breve de reproducción

Tabla principal: Usuarios expuestos a dos versiones de la página de inicio (landing page) dentro del experimento A/B ('/datasets/landing_experiment.csv').
Métrica foco: tasa de conversión y gasto promedio (valor generado por cada cliente).
Naturaleza del análisis: validación de hipótesis, correlacional e inferencial, no causal.
Tipos de relaciones analizadas: Numéricas (lineales y monotónicas), Binarias vs. numéricas & Categóricas
Resultado final: un reporte de análisis de validación de diversas hipótesis estadísticas que combine Evidencia visual, Evidencia numérica, Interpretación responsable e Implicaciones de negocio

Sigue el flujo de trabajo descrito en cada celda del Jupyter Notebook; ahí encontrarás instrucciones paso a paso, pre-código y notas que te servirán de guía para entender el proyecto realizado.


