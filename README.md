<h1 align="center">
Análisis de comportamiento de usuario, embudo de eventos y Test A/A/B
</h1>

## Objetivo 

Analizar el comportamiento del usuario en la aplicación móvil de una startup de foodtech para dos propósitos clave:

1. **Optimizar el Embudo de Ventas:** Identificar las etapas con mayor tasa de abandono (drop-off) antes de la compra.

2. **Validar Estadísticamente un Cambio de Diseño:** Determinar, mediante un Test A/A/B, si una modificación en las fuentes de la aplicación afecta negativamente la tasa de conversión o el flujo de usuario.

Este proyecto demuestra mi capacidad para **analizar el flujo de procesos** (Process Flow), utilizar **Estadística Inferencial** para la toma de decisiones críticas y mitigar riesgos antes de implementar cambios a gran escala.
<br>

## Metodología de Análisis y Validación 📑

**FASE 1: Análisis del Embudo de Ventas**

- **Objetivo:** Visualizar el flujo de usuario desde el primer evento hasta la compra para cuantificar la eficiencia de cada paso.
- **Métrica Clave:** **Tasa de Retención/Abando** entre eventos (e.g., desde el inicio hasta la visualización del carrito, y desde el carrito hasta la compra).
- **Habilidad Demostrada:** Mapeo de procesos y análisis de cuellos de botella.

**FASE 2: Test A/A/B (Validación de Diseño)**

- **Diseño Experimental:** Se utilizaron tres grupos de usuarios:

  - **Grupos A/A (Control):** Dos grupos idénticos (246 y 247) para asegurar la validez interna del experimento y la fiabilidad de la distribución de usuarios.

  - **Grupo B (Test):** El grupo que interactúa con la aplicación con el nuevo diseño de fuentes.

- **Pruebas de Hipótesis:** Uso de la **Prueba Z para Proporciones** para comparar las tasas de conversión (número de usuarios que llegan a cada etapa) entre los grupos (A vs B y A vs A).

- **Habilidad Demostrada:** Diseño experimental, rigor estadístico y control de la probabilidad de error (Alpha, Nivel de Significancia).

## 🧰⚙️🛠️
<br>
<p align="center"> 
  &emsp;
   <a href="https://www.python.org" target="_blank">
    <img alt="Python" src="https://img.shields.io/badge/Python%20-%2314354C.svg?style=plastic&logo=python&logoColor=white">
  </a>
  &emsp;
  <a href="#"><img alt="Pandas" src="https://img.shields.io/badge/Pandas-%2334A853.svg?"></a>
  &emsp;
  <a href="#"><img alt="NumPy" src="https://img.shields.io/badge/Numpy-0078d7.svg?"></a>
    &emsp;
  <a href="#"><img alt="pyplot" src="https://img.shields.io/badge/pyplot-%234479A1.svg?"></a>
  &emsp;
  <a href="#"><img alt="plotly" src="https://img.shields.io/badge/plotly-%23F7DF1E.svg?"></a>
</p>
<br>

## Resultados y Conclusiones 📊✔️

1. **Hallazgos del Embudo de Ventas**
   
  - **Cuello de Botella:** La transición del evento *CartScreenAppear* **(Visualizar Carrito)** a *PaymentScreenSuccessful* **(Compra Exitosa)** es el punto con el mayor drop-off en el flujo, indicando una posible fricción en el proceso de pago.
  - **Tasa de Compra Final:** El **47.7 %** de los usuarios realizan todo el viaje desde la pagina principal *MainScreenAppear* **(Pantalla principal)** hasta concretar el pago *PaymentScreenSuccessful* **(Pago exitoso)**.
  - **Recomendación:** Enfocar los esfuerzos de optimización del rendimiento técnico en la pantalla de pago para **mejorar la eficiencia de conversión**.

2. **Conclusión del Test A/A/B (Validación)**

  - **Nivel de Significancia:** Se utilizó un nivel $\alpha$ para las pruebas de hipótesis.
  - **Comparación A vs A (Control):** El Test A/A validó que los grupos de control eran indistinguibles estadísticamente, confirmando la fiabilidad del proceso de prueba.
  - **Comparación A vs B (Test):** El análisis estadístico no encontró **diferencias estadísticamente significativas** entre la tasa de conversión de los grupos de control y el grupo de prueba (Grupo B) en la mayoría de los eventos.
  - **Decisión Final:** Dado que la nueva versión (B) no mostró un rendimiento diferente (ni peor ni mejor) al grupo de control, la recomendación es que **el cambio de fuente es seguro de implementar** desde la perspectiva de la conversión y el flujo de usuario, ya que no representa un riesgo operativo.

## Instrucciones de Puesta en Marcha 🗒️👩‍💻

Para revisar el código completo y la ejecución del análisis:

1.	**Clonar el Repositorio**
2.	**Instalar Dependencias**
   Las librerías principales son: pandas, NumPy, seaborn, pyplot, plotly.
3. **Ejecutar el Notebook**
   Abre el archivo notebook.ipynb para recorrer el análisis del embudo, la definición de las pruebas estadísticas y la conclusión del Test A/A/B.
