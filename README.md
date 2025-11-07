# Análisis y Predicción del Precio del Café (2023–2025)

Este proyecto en **Python** descarga precios reales del **futuro del café (KC=F)** desde **Yahoo Finance**, y aplica **modelos de Machine Learning** para analizar su comportamiento y predecir la tendencia de precios.

Se incluyen:
- Un modelo de **Regresión (Random Forest)** que predice el **precio del día siguiente**.  
- Un modelo de **Clasificación (SVM)** que determina si el precio **sube o baja**.  
- Gráficos interactivos con **Plotly** para explorar los resultados de forma visual y dinámica.  
- Una **tabla descriptiva** con variables estadísticas básicas en español.

---

##  Uso

1. Descargue este repositorio con el botón verde **Code → Download ZIP**.  
2. Descomprima el archivo ZIP en su computador.  
3. Abra el archivo `proyecofinal.py` en su entorno de Python (VSCode, Jupyter, Colab o Anaconda).  
4. Ejecute el código para:
   - Entrenar los modelos de predicción.
   - Visualizar los gráficos interactivos.
   - Obtener los resultados de “precio real vs. predicho” y la predicción de mañana.

---

## Archivos del proyecto

| Archivo | Descripción |
|----------|--------------|
| `proyectofinal.py` | Código principal del proyecto (modelos, gráficos y comentarios). |
| `proyectofinal.ipynb` | Versión interactiva para Google Colab. |
| `requirements.txt` | Librerías necesarias para ejecutar el proyecto. |

---

## Contenido del análisis

El programa realiza los siguientes pasos:
1. **Descarga automática** de precios reales del café (`KC=F`) desde Yahoo Finance.  
2. **Limpieza y creación de variables estadísticas**: medias móviles (MA5, MA20), volatilidad y RSI.  
3. **Entrenamiento de modelos**:
   - Random Forest Regressor (precio futuro).  
   - SVM Classifier (sube/baja).  
4. **Visualizaciones**:
   - Gráfico “Precio real vs. Predicho”.  
   - Gráfico interactivo con *hover* para explorar precios recientes.  
   - Tabla descriptiva con las variables calculadas.  
5. **Predicción final**: muestra el precio real de hoy, el precio esperado mañana y si el modelo predice que **sube o baja**.

---

## Ejecutar en Google Colab

Si prefieres correrlo de forma interactiva sin descargar nada, abre el notebook en Colab con este botón:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Sebaasap/proyecto-ml-cafe/blob/main/proyectofinal.ipynb)



---

## Ejecutar en tu computador

1. Asegúrate de tener **Python 3.10 o superior**.  
2. Abre una terminal (CMD, PowerShell o Terminal de Mac/Linux).  
3. Crea un entorno virtual e instala las librerías:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate   # En Windows
   # source .venv/bin/activate   # En Mac/Linux

   pip install -r requirements.txt
