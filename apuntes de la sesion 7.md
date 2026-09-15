¿Cuál es su valor?
Automatización: permite automatizar tareas que antes requerían intervención humana.
Predicción: puede analizar datos históricos para predecir comportamientos futuros, como ventas, demanda o riesgos.
Toma de decisiones: ayuda a las empresas a tomar decisiones basadas en datos.
Detección de patrones: encuentra relaciones o comportamientos difíciles de identificar manualmente.
Personalización: permite ofrecer recomendaciones adaptadas a cada usuario, como Netflix, YouTube o Spotify.
Eficiencia: puede procesar grandes cantidades de información rápidamente.
Innovación: permite desarrollar aplicaciones como reconocimiento facial, asistentes virtuales, detección de fraude y vehículos autónomos.
1. Flujos de datos

Un flujo de datos (data stream) es cuando los datos llegan continuamente, en lugar de tenerlos todos disponibles desde el principio.

Ejemplo:
Una aplicación recibe constantemente datos de usuarios:

Usuario → dato → modelo → predicción → nuevo dato → modelo...

Esto es útil cuando los datos cambian constantemente, como precios, sensores, tráfico o transacciones.
2. Ritmo de aprendizaje (Learning Rate)

El ritmo de aprendizaje indica qué tan grandes son los cambios que hace el modelo al aprender.

Ritmo alto: aprende rápidamente, pero puede pasarse de la solución adecuada.
Ritmo bajo: aprende lentamente, pero puede ser más estable.
Ritmo adecuado: permite llegar progresivamente a un buen modelo.

Por ejemplo, si el modelo tiene un error:

Error → ajuste → menor error → ajuste → menor error

El learning rate determina qué tan grande es cada ajuste.
3. Aprendizaje por lotes (Batch Learning)

En Batch Learning, el modelo recibe un conjunto de datos completo y aprende utilizando ese lote.

Ejemplo:

10.000 registros → entrenamiento → modelo actualizado

Después se puede volver a entrenar cuando se tengan nuevos datos.

Ventaja: puede ser eficiente para grandes conjuntos de datos almacenados.
Desventaja: no se adapta inmediatamente a nuevos datos.
4. Aprendizaje en línea (Online Learning)

En Online Learning, el modelo aprende poco a poco conforme llegan los datos.

Ejemplo:

Dato 1 → aprende
Dato 2 → aprende
Dato 3 → aprende
Dato 4 → aprende

Es especialmente útil cuando existe un flujo continuo de información.

Ventaja: se adapta rápidamente a cambios.
Desventaja: si recibe datos incorrectos o problemáticos, estos pueden afectar el modelo
Desafíos y riesgos de un sistema de Machine Learning
Ruido en los datos
Son datos incorrectos, incompletos o con información innecesaria.
Problema: el modelo puede aprender patrones equivocados.
Solución: limpiar los datos, eliminar valores anormales y verificar su calidad.
Errores en los datos
Puede haber información mal registrada o etiquetas incorrectas.
Problema: el modelo aprende de ejemplos equivocados.
Solución: revisar y validar los datos antes del entrenamiento.
Datos falsos o manipulados
Alguien puede introducir información falsa deliberadamente.
Problema: puede hacer que el modelo produzca predicciones incorrectas.
Solución: utilizar controles de seguridad, validación de datos y monitoreo constante.
Selección de características (features)
Las características son los datos que utiliza el modelo para aprender, por ejemplo: edad, precio, ubicación o historial.
Problema: seleccionar características irrelevantes puede reducir la precisión; seleccionar características inadecuadas también puede generar sesgos.
Solución: elegir las características realmente útiles y eliminar las innecesarias
Fases de evaluación
División de los datos
Se separan los datos en conjuntos:
Entrenamiento: el modelo aprende.
Validación: se ajustan los parámetros y se comparan alternativas.
Prueba: se comprueba el rendimiento final con datos que el modelo no ha visto.
Evaluación del modelo
Se mide qué tan buenas son sus predicciones.
Algunas métricas son:
Exactitud (accuracy)
Precisión (precision)
Recall
F1-score
Error medio, dependiendo del problema.
Comparación
Se comparan diferentes modelos o configuraciones para determinar cuál funciona mejor.
Prueba con datos nuevos
Se utiliza el modelo con datos que no utilizó durante el entrenamiento.
Esto permite saber si realmente puede generalizar y no simplemente memorizar los datos.
Monitoreo
Una vez puesto en funcionamiento, se sigue evaluando porque los datos pueden cambiar con el tiempo y el modelo puede perder precisión.
