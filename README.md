# 🧠 Proyecto Módulo 3 – Preparación de Datos

Este repositorio contiene el desarrollo completo del proyecto de **Preparación de Datos**, realizado en el marco del Módulo 3 del curso de Ciencia de Datos. El proyecto aborda el proceso de generación, recolección, limpieza, transformación e integración de datos provenientes de múltiples fuentes, dejando un dataset final listo para análisis.

---

## 📁 Estructura del repositorio

├── Proyecto módulo 3_F. Rojas.ipynb # Notebook principal con el flujo completo del proyecto
├── datos_clientes.npy # Datos base de clientes generados con NumPy
├── datos_transacciones.npy # Datos de transacciones simuladas
├── datos_sucios_clientes.csv # Dataset de clientes sin limpiar
├── datos_sucios_transacciones.xlsx # Dataset de transacciones sin limpiar
├── datos_uf_2025.csv # Valores de la UF 2025 extraídos desde la web
├── datos_unificados.csv # Dataset consolidado de múltiples fuentes
├── datos_limpio.csv # Dataset tras limpieza inicial
├── datos_optimizado.csv # Dataset con variables transformadas
├── dataset_final_limpio.csv # Dataset final listo para análisis
├── Reporte_2025.xlsx # Reporte con métricas y resúmenes


---

## 🧩 Descripción del proyecto

El objetivo del proyecto es implementar un flujo de trabajo eficiente para la preparación de datos, utilizando **NumPy y Pandas**, que permita integrar información de distintas fuentes, asegurar la calidad de los datos y estructurarlos adecuadamente para su posterior análisis.

El proceso incluye generación de datos sintéticos, extracción de información desde fuentes externas, limpieza, transformación y consolidación en un único DataFrame.

---

## 🛠 Técnicas aplicadas

- Generación de datos sintéticos mediante **NumPy**.
- Extracción de datos externos desde páginas web (valores de UF 2025).
- Integración de múltiples fuentes (CSV, Excel y HTML).
- Limpieza de datos:
  - Eliminación de duplicados.
  - Imputación de valores nulos.
  - Tratamiento de outliers mediante el método IQR.
- Normalización y ajuste de tipos de datos.
- Creación de variables derivadas para enriquecer el dataset.
- Agrupamiento y generación de métricas resumen con `groupby()`.

---

## 🚀 Principales decisiones técnicas

- Se definió el **año 2025 como referencia temporal** para la generación de los datos, con el objetivo de mantener coherencia con los valores de la UF extraídos desde fuentes externas.
- Las tablas obtenidas desde la web requirieron un proceso específico de limpieza, incluyendo selección de columnas relevantes, normalización de nombres y conversión de tipos de datos.
- El flujo de trabajo se orientó a priorizar la **calidad, consistencia y reutilización** del dataset final.

---

## 📦 Requisitos

Para ejecutar el notebook se requiere:

- Python 3.x
- NumPy
- Pandas
- openpyxl (para manejo de archivos Excel)

Instalación de dependencias:

```bash
pip install numpy pandas openpyxl
