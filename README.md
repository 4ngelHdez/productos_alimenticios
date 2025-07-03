Análisis del Comportamiento del Usuario en una Aplicación de Productos Alimenticios

Descripción del Proyecto<br>

En este proyecto, me enfoqué en el análisis del comportamiento del usuario dentro de una aplicación móvil de una empresa emergente de productos alimenticios. El objetivo principal fue investigar cómo interactúan los usuarios con la aplicación durante un período específico, identificar patrones de uso y evaluar la efectividad de las diferentes etapas del embudo de eventos mediante una prueba A/A/B.

Objetivos:<br>

   * Estudiar y validar la integridad de los datos de la aplicación.<br>
   * Analizar el embudo de eventos para comprender el flujo de los usuarios a través de la aplicación.<br> 
   * Estudiar los resultados de un experimento (A/A/B testing) para identificar posibles diferencias significativas entre los grupos.<br>

Metodología:<br>

Utilicé Python y librerías como pandas, numpy, seaborn, plotly, scipy y statsmodels para realizar un análisis exploratorio y evaluar la validez de la prueba A/A/B. El trabajo incluyó:<br>
    
   * Un análisis de datos de usuario recopilados entre el 25 de julio de 2019 y el 7 de agosto de 2019.<br>
   * Preparación exhaustiva de los datos, incluyendo la revisión de tipos de datos, la detección y eliminación de valores duplicados y transformación de columnas para un análisis más detallado.<br>
   * Análisis de las frecuencias de los eventos y el número de usuarios únicos en cada etapa del embudo.<br>
   * Se examinó el período de tiempo cubierto por los datos para identificar y excluir cualquier dato atípico inicial que pudiera distorsionar los resultados del experimento, enfocándose en el período de mayor actividad de la aplicación (agosto de 2019).<br>
   * Realización de pruebas estadísticas de proporciones y la prueba de Mann-Whitney U para comparar los grupos del experimento (246, 247 y 248) y determinar si existían diferencias significativas entre ellos.<br>


Conclusiones:<br>

   - Se identificó que el evento más frecuente es "MainScreenAppear" (pantalla principal), seguido por "OffersScreenAppear" (pantalla de ofertas), "CartScreenAppear" (carrito de compras) y "PaymentScreenSuccessful" (pago exitoso). El "Tutorial" es el evento menos frecuente.<br>

   - La aplicación registró un total de 7,551 usuarios únicos durante el período de estudio.<br> 

   - El promedio de eventos por usuario es de 32.28.<br> 

   - Las etapas donde se pierden más usuarios son la transición de la pantalla principal a la de ofertas (2,826 usuarios únicos perdidos) y de la página de pago exitoso a los tutoriales (2,699 usuarios únicos perdidos).<br>

   - Solo el 11.15% de los usuarios completan todo el proceso, desde su primer evento hasta el pago exitoso.<br> 

   - A pesar de los ajustes en el umbral y la corrección de alpha con el método Sidak, las pruebas estadísticas (prueba de proporciones Z y Mann-Whitney U) indicaron diferencias significativas entre los grupos del experimento (246, 247 y 248). Esto sugiere que las muestras de los grupos no fueron tomadas correctamente o que existe una diferencia inherente en el comportamiento de los usuarios en estos grupos.<br> 


Lenguajes y herramientas principales:<br>

   * Python (pandas, numpy, seaborn, matplotlib, plotly express, scipy).<br>
   * Jupyter Notebook para documentación del análisis.<br>
   * Prueba Z de proporciones y Mann-Whitney U para validación estadística.<br>

Este análisis proporciona una comprensión detallada del comportamiento del usuario en la aplicación, destacando áreas clave de mejora en el embudo de conversión y la importancia de asegurar la correcta aleatorización de los grupos en futuros experimentos A/A/B.
