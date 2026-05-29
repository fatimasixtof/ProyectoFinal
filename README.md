# ProyectoFinal
Archivos completos para el Proyecto final de la materia Proyecto I impartida por el maestro Luis Guillermo García Jácome
# Dinámicas de Hiperconsumismo y Fast Fashion: Un Modelo Basado en Agentes

## Descripción del Modelo
Este proyecto es una simulación basada en agentes desarrollada en **NetLogo** que modela el ciclo de vida de las tendencias de moda bajo condiciones de hiperconsumismo y *fast fashion*. 

El modelo simula una sociedad espacialmente distribuida en un látice bidimensional, donde 1089 agentes interactúan estrictamente con su vecindad de Moore (sus 8 vecinos directos). El objetivo principal es observar cómo interactúan dos fuerzas opuestas:
1. **La influencia externa (Industria):** El bombardeo de tendencias globales dictadas por las marcas.
2. **El contagio local:** La influencia social directa entre vecinos.

A medida que avanza la simulación, los agentes experimentan un desgaste en su satisfacción (*tasa de aburrimiento*). Cuando esta llega a cero, deben decidir si adoptan la moda global, copian a un vecino o, en una menor probabilidad, innovan con un color completamente nuevo. El modelo demuestra visual y cuantitativamente que las tendencias efímeras requieren de un alto nivel de desgaste poblacional y una fuerte imposición central para lograr homogeneizaciones masivas y fugaces.

## Archivos del Repositorio
Para cumplir con los lineamientos del proyecto, este repositorio incluye los siguientes archivos:

* `ProyectoI_FinalProyecto.nlogo`: El script principal del modelo desarrollado en NetLogo. Contiene toda la lógica de los agentes, la red espacial y la interfaz gráfica.
* `resultados_hiperconsumismo.csv`: Base de datos generada a través de la herramienta *BehaviorSpace* de NetLogo, documentando múltiples corridas del modelo bajo diferentes parámetros de aburrimiento e influencia externa.
* `Lector-deCSV.ipynb`: Script de Python (utilizando Pandas y Seaborn) empleado para limpiar los datos del CSV y generar las gráficas analíticas presentadas en el reporte final.

## Instrucciones de Uso
1. Abre el archivo `.nlogo` en NetLogo (versión 6.1 o superior, yo utilice 6.4.0).
2. Presiona el botón **setup** para inicializar el mundo y generar la vecindad.
3. Ajusta los parámetros `tasa-de-aburrimiento` e `influencia-externa` en la interfaz.
4. Presiona el botón **go** para correr la simulación de manera continua.
