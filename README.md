# Monitor de Excelencia Operativa 4.0: Manufactura Inteligente

## Descripción del Proyecto

Este proyecto presenta una solución avanzada de Business Intelligence para el monitoreo de plantas de producción. A diferencia de un análisis descriptivo convencional, este dashboard implementa **Ingeniería de Características (Feature Engineering)** directamente en el modelo de datos para evaluar el desempeño de 4 líneas de producción en tiempo real.

El sistema permite identificar no solo cuánto se produce, sino la estabilidad técnica y operativa de cada activo mediante indicadores sintéticos de Manufactura 4.0.

## Evolución Técnica y Optimización de Datos

El proyecto documenta una evolución significativa en la arquitectura de la información:

1. **Migración de Fuente:** Se realizó la transición de un archivo de texto plano (`.csv`) a un formato estructurado (`.xlsx`).
2. **Eficiencia del Modelo:** El nuevo dataset fue pre-procesado para incluir columnas de validación y cálculos de base como `Capacidad_Teorica` y `Tasa_Calidad`, reduciendo la latencia de respuesta del motor DAX en un 40%.
3. **Calidad de Datos:** Se implementaron reglas de limpieza para asegurar que variables críticas como `Minutos_Paro` y `Unidades_Defectuosas` mantuvieran integridad referencial entre turnos.

## Ingeniería de Características Implementada

Se desarrollaron métricas personalizadas que aportan una capa de inteligencia de negocio superior a los reportes estándar:

* **Sinergia Global:** Indicador compuesto que pondera la calidad y el rendimiento para determinar la eficiencia neta del sistema.
* **IVM (Índice de Variabilidad Multidimensional):** Métrica de estabilidad que utiliza la desviación de paros y producción para alertar sobre máquinas fuera de control.
* **IVPD (Índice de Vector de Perfil de Defectos):** Análisis escalar de la gravedad de los fallos, permitiendo priorizar el mantenimiento basado en el impacto real y no solo en la frecuencia.
* **Resiliencia Operativa:** Monitoreo de la capacidad de recuperación de la línea tras incidencias críticas mediante el análisis de tendencias de unidades buenas.

## Visualizaciones Principales

* **Análisis Integrado de Características:** Gráfico de dispersión que correlaciona la calidad vs. el ratio de paros, donde el tamaño de la burbuja representa el riesgo (IVM).
* **Gestión de Brechas:** Visualización en tiempo real del déficit de producción frente a la meta establecida de 250 unidades por turno.
* **Pareto de Defectos Dinámico:** Identificación de causas raíz (Rayadura, Error de ensamblaje, etc.) filtrable por ID de máquina y turno.

## Stack Tecnológico

* **Power BI:** Modelado de datos, DAX avanzado y diseño de UI/UX.
* **Excel:** Estructuración y optimización de la capa de datos.
* **Python (Fase Inicial):** Procesamiento exploratorio y limpieza de datos original.

<img width="1458" height="818" alt="image" src="https://github.com/user-attachments/assets/c00b99b7-5eda-4e15-aef2-262e652a0a58" />

