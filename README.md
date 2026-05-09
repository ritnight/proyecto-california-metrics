# Proyecto California Real Estate: Tasación y Segmentación de Mercado

Este proyecto tiene como objetivo analizar, explorar y modelar datos del mercado inmobiliario del estado de California. A través de un enfoque basado en ciencia de datos, buscamos automatizar la predicción de precios de viviendas utilizando algoritmos de Aprendizaje Supervisado, y comprender la geografía económica del mercado mediante Aprendizaje No Supervisado.

## 🚀 Estructura del Proyecto

El proyecto está organizado para seguir un flujo de trabajo profesional de Machine Learning:

```bash
Proyecto-RealEstate/
├── data/              # Datasets brutos (.csv) y procesados (.pkl)
├── models/            # Modelos entrenados y optimizados exportados
├── notebooks/         # Jupyter Notebooks con el flujo completo de análisis y modelado
└── environment.yml    # Configuración del entorno virtual (Conda)
```

## 🛠️ Configuración del Entorno

Para asegurar que todos los miembros del equipo trabajen con las mismas versiones de herramientas y evitar problemas de dependencias, utilizamos **Miniconda**.

### Instalación

1. Asegúrate de tener instalado [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
2. Clona este repositorio y navega a la carpeta del proyecto.
3. Crea y activa el entorno con los siguientes comandos:

```bash
# Crear el entorno desde el archivo de configuración
conda env create -f environment.yml

# Activar el entorno
conda activate california_housing_ml_pipeline

# Si necesitas actualizar el entorno después de agregar nuevas librerías:
conda env update -f environment.yml --prune
```

## 📊 Fases del Proyecto

El desarrollo se documenta a través de 5 cuadernos principales, cubriendo todo el ciclo de vida del dato:

| Cuaderno | Fase | Descripción |
| --- | --- | --- |
| `01_eda.ipynb` | **Exploración y Limpieza** | Análisis exploratorio de datos (EDA), tratamiento de valores nulos, identificación de outliers y análisis de distribuciones. |
| `02_supervised_modeling.ipynb` | **Preprocesamiento y Modelado** | Creación de Pipelines de transformación (OneHotEncoding, Escalado) y entrenamiento de Regresión Lineal y Random Forest. |
| `03_model_evaluation.ipynb` | **Evaluación de Modelos** | Validación cruzada (Cross-Validation) y cálculo de métricas de error continuo (MAE, RMSE, R2). |
| `04_hyperparameter_optimization.ipynb` | **Optimización (Tuning)** | Ajuste fino del Random Forest mediante `RandomizedSearchCV` y análisis de Importancia de Variables (Feature Importance). |
| `05_final_analysis.ipynb` | **Segmentación e Integración** | Aplicación de Aprendizaje No Supervisado (K-Means) para descubrir nichos de mercado (mercado masivo vs. ultra-lujo) y conclusiones de negocio. |

## 👥 Contribuciones

Este proyecto fue desarrollado bajo una metodología de trabajo colaborativo mediante GitHub. Cada integrante es responsable de aportar en distintas etapas del flujo de datos, asegurando la trazabilidad, modularidad y calidad del análisis.

- Constanza Gonzalez  
- Alejandra Gonzalez  
- Genesis Baeza  
- Jimena Galicia  
