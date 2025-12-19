# Dashboard-Doble-Vista-Stack-Overflow-Survey
📌 Descripción general

Este proyecto implementa un dashboard de doble vista (Double-View Dashboard) utilizando Python y datos reales del Stack Overflow Developer Survey. El objetivo es demostrar una arquitectura profesional de análisis de datos que separa claramente:

Vista Ejecutiva: enfocada en KPIs, tendencias y toma de decisiones estratégicas.

Vista Operativa: orientada al análisis granular, exploración de datos y trabajo diario con información detallada.

Este tipo de arquitectura es ampliamente utilizada en entornos corporativos, ya que permite ofrecer información relevante a distintos niveles de la organización sin exponer datos innecesarios.

🏗️ Arquitectura del proyecto

El proyecto está dividido conceptualmente en dos capas:

1️⃣ Capa ETL (Data Preparation)

Carga del dataset original del Stack Overflow Survey.

Limpieza y normalización de datos.

Generación de dos vistas:

vista_operativa.csv

vista_ejecutiva.csv

Esta capa actúa como motor de datos y puede reutilizarse para múltiples dashboards o herramientas.

2️⃣ Capa de Visualización

Lectura directa de las vistas generadas por el ETL.

Generación de dashboards y gráficos ejecutivos.

Exportación automática de visualizaciones en formato imagen (.png).

📊 Vistas implementadas
🔹 Vista Ejecutiva

Pensada para perfiles de liderazgo y toma de decisiones.

Incluye:

KPIs globales:

Cantidad de países analizados

Salario promedio global

Total de respuestas

Customer Journey Funnel (simulado)

Top 10 países por salario promedio

Distribución salarial global

Comparación salario promedio vs mediano

Países con mayor volumen de respuestas

Relación entre experiencia y salario

Lenguajes de programación más utilizados

Todas estas visualizaciones se exportan automáticamente como imágenes para su uso en reportes, presentaciones o GitHub.

🔹 Vista Operativa

Orientada al análisis detallado.

Incluye:

Tabla completa de respuestas

Filtros por país

Conteo dinámico de registros

Permite explorar los datos a nivel individual sin perder trazabilidad.

🛠️ Tecnologías utilizadas

Python 3

Pandas – Manipulación y análisis de datos

Plotly – Visualizaciones ejecutivas

Matplotlib – Gráficos complementarios

Streamlit – Interfaz de dashboard

Statsmodels – Análisis de tendencia (regresión)
