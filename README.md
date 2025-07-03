Análisis del Comportamiento del Usuario en una Aplicación de Productos Alimenticios

Descripción del Proyecto

En este proyecto, me enfoqué en el análisis del comportamiento del usuario dentro de una aplicación móvil de una empresa emergente de productos alimenticios. El objetivo principal fue investigar cómo interactúan los usuarios con la aplicación durante un período específico, identificar patrones de uso y evaluar la efectividad de las diferentes etapas del embudo de eventos mediante una prueba A/A/B. 

Objetivos:

    * Estudiar y validar la integridad de los datos de la aplicación. 
    * Analizar el embudo de eventos para comprender el flujo de los usuarios a través de la aplicación. 
    * Estudiar los resultados de un experimento (A/A/B testing) para identificar posibles diferencias significativas entre los grupos. 

Metodología:

Utilicé Python y librerías como pandas, numpy, seaborn, plotly, scipy y statsmodels para realizar un análisis exploratorio y evaluar la validez de la prueba A/A/B. El trabajo incluyó:
    
    * Un análisis de datos de usuario recopilados entre el 25 de julio de 2019 y el 7 de agosto de 2019. 
    * Preparación exhaustiva de los datos, incluyendo la revisión de tipos de datos, la detección y eliminación de valores duplicados y transformación de columnas para un análisis más detallado.
    * Análisis de las frecuencias de los eventos y el número de usuarios únicos en cada etapa del embudo. 
    * Se examinó el período de tiempo cubierto por los datos para identificar y excluir cualquier dato atípico inicial que pudiera distorsionar los resultados del experimento, enfocándose en el período de mayor actividad de la aplicación (agosto de 2019). 
    * Realización de pruebas estadísticas de proporciones y la prueba de Mann-Whitney U para comparar los grupos del experimento (246, 247 y 248) y determinar si existían diferencias significativas entre ellos. 


Conclusiones:

    - Se identificó que el evento más frecuente es "MainScreenAppear" (pantalla principal), seguido por "OffersScreenAppear" (pantalla de ofertas), "CartScreenAppear" (carrito de compras) y "PaymentScreenSuccessful" (pago exitoso). El "Tutorial" es el evento menos frecuente. 

    - La aplicación registró un total de 7,551 usuarios únicos durante el período de estudio. 

    - El promedio de eventos por usuario es de 32.28. 

    - Las etapas donde se pierden más usuarios son la transición de la pantalla principal a la de ofertas (2,826 usuarios únicos perdidos) y de la página de pago exitoso a los tutoriales (2,699 usuarios únicos perdidos). 

    - Solo el 11.15% de los usuarios completan todo el proceso, desde su primer evento hasta el pago exitoso. 

    - A pesar de los ajustes en el umbral y la corrección de alpha con el método Sidak, las pruebas estadísticas (prueba de proporciones Z y Mann-Whitney U) indicaron diferencias significativas entre los grupos del experimento (246, 247 y 248). Esto sugiere que las muestras de los grupos no fueron tomadas correctamente o que existe una diferencia inherente en el comportamiento de los usuarios en estos grupos. 


Lenguajes y herramientas principales:

    * Python (pandas, numpy, seaborn, matplotlib, plotly express, scipy)
    * Jupyter Notebook para documentación del análisis
    * Prueba Z de proporciones y Mann-Whitney U para validación estadística 

Este análisis proporciona una comprensión detallada del comportamiento del usuario en la aplicación, destacando áreas clave de mejora en el embudo de conversión y la importancia de asegurar la correcta aleatorización de los grupos en futuros experimentos A/A/B.