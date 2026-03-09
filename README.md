# Predicción de Ventas: Análisis de Series Temporales 📈

Este repositorio contiene un proyecto de predicción de ventas (Time Series Forecasting) desarrollado para una empresa de retail online. El objetivo es pronosticar el volumen de ventas totales por país para el próximo mes, optimizando así la planificación logística y financiera de la compañía.

## 🎯 Objetivo del Proyecto
Pasar de un análisis puramente descriptivo del histórico de ventas a un **modelo predictivo accionable**. La meta es anticipar la demanda a 4 semanas vista para tomar decisiones estratégicas sobre inventario, especialmente de cara a los picos estacionales.

## 🛠️ Herramientas y Tecnologías
- **Lenguaje:** Python
- **Manipulación y Análisis:** Pandas, Numpy
- **Modelos Estadísticos y Clásicos:** SARIMAX
- **Modelos de Machine Learning:** Prophet (Meta), XGBoost
- **Métrica de Evaluación:** MAPE (Mean Absolute Percentage Error)

## 🔄 Metodología del Proyecto
El desarrollo se estructuró en las siguientes fases metodológicas:

1. **Análisis Exploratorio y Preprocesamiento:** Limpieza de datos, extracción de estacionalidad, análisis de autocorrelación y descomposición de la serie temporal partiendo de un histórico de un año (Dic 2022 - Dic 2023).
2. **Desarrollo de Modelos:** Se entrenaron diferentes enfoques:
   - *Prophet* para capturar tendencias y estacionalidades de forma rápida.
   - *SARIMAX* incorporando una variable exógena para la "temporada alta".
   - *XGBoost* alimentado con variables de calendario y retardos temporales (lags).
3. **Selección Dinámica:** En lugar de usar un único modelo para todo, se evaluó el rendimiento mediante el error MAPE y se seleccionó **el mejor modelo de forma individual para cada país**.

## 💡 Conclusiones y Recomendaciones de Negocio
El valor real de este modelo radica en su aplicación práctica. A partir de las predicciones, se extrajeron las siguientes directrices estratégicas:

* **Anticipación del Q4 (Cuarto Trimestre):** Se detectó la necesidad de reforzar la logística y el inventario desde el mes de septiembre para hacer frente al pico estacional de ventas.
* **Dependencia del Mercado:** Actualmente, más del 80% de las ventas se concentran en un solo país (UK). Es vital utilizar las predicciones para diversificar y potenciar mercados secundarios con gran margen de crecimiento (Alemania, Irlanda, Francia).
* **Integración Financiera:** Las predicciones de este modelo sirven como base matemática sólida (input) para los modelos de valoración financiera frente a una futura ampliación de capital de la empresa.
