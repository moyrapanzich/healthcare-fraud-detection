# Healthcare Fraud Detection using Machine Learning

Repositorio correspondiente al Proyecto Final Integrador de la Diplomatura en Ciencia de Datos y Análisis Avanzado.

El objetivo del proyecto es identificar proveedores médicos con comportamientos atípicos potencialmente asociados a fraude, a partir del análisis de datos de facturación. Para ello, se integraron múltiples fuentes de información y se desarrolló un modelo de Machine Learning orientado a detectar patrones relevantes y asistir en procesos de auditoría.

---

## Contenido

- [Healthcare_Fraud_Detection_Project.ipynb](https://colab.research.google.com/drive/1tl9ZrbKmNhg1aFrtIweoQaBXIFgHcCZp?usp=sharing): Notebook principal con el desarrollo completo del proyecto (EDA, feature engineering, modelado y evaluación).
- content/: Carpeta donde deben ubicarse los archivos del dataset descargados desde Kaggle.
- README.md: Documentación del proyecto.

---

## Requisitos

- Python 3.10 o superior  
- Librerías: `pandas`, `numpy`, `scikit-learn`, `matplotlib`  
- Opcional: `xgboost`, `shap`

---

## Instalación (ejecución local)

Clonar el repositorio o descargar los archivos.

Crear un entorno virtual (opcional):

```bash
python -m venv env
```

Activar entorno:

Windows:
```bash
env\Scripts\activate
```

Mac/Linux:
```bash
source env/bin/activate
```

Instalar dependencias:

```bash
pip install pandas numpy scikit-learn matplotlib
```

---

## Uso en Google Colab

El proyecto también puede ejecutarse en Google Colab sin necesidad de instalación local.

Pasos:

- Abrir el notebook `.ipynb` en Google Colab  
- Subir manualmente los archivos CSV del dataset  
- Ubicarlos en `/content/`  
- Ejecutar las celdas en orden  

No se requiere instalación de librerías ya que Colab incluye las dependencias necesarias por defecto.


---

## Datos

El dataset utilizado corresponde a:

Healthcare Provider Fraud Detection – Kaggle  
https://www.kaggle.com/datasets/rohitrox/healthcare-provider-fraud-detection-analysis

Para el desarrollo del modelo se utilizaron exclusivamente los archivos de entrenamiento (Train), descartando los archivos de test.

Archivos utilizados:

- Train_Beneficiarydata-1542865627584.csv  
- Train_Inpatientdata-1542865627584.csv  
- Train_Outpatientdata-1542865627584.csv  
- Train-1542865627584.csv  

Los archivos deben ubicarse en la carpeta `content/` (o en `/content/` si se utiliza Google Colab).  

---

## Metodología

Se utilizó la metodología CRISP-DM, estructurando el proyecto en las siguientes etapas:

- comprensión del problema  
- análisis de datos (EDA)  
- preparación de datos  
- modelado  
- evaluación e interpretación  

---

## Análisis Exploratorio (EDA)

Se identificó un fuerte desbalance de clases, donde los casos de fraude representan aproximadamente el 9% del total.

También se detectaron patrones relevantes en variables económicas y de utilización de servicios, lo que permitió orientar el modelado y la selección de variables.

---

## Preparación de datos

- Integración de múltiples fuentes  
- Limpieza de datos  
- Tratamiento de valores faltantes  
- Generación de variables agregadas a nivel proveedor  

---

## Modelado

Se evaluaron los siguientes algoritmos:

- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Dado el desbalance de clases, se priorizó el uso de métricas como recall y F1-score.

---

## Resultados

El modelo Logistic Regression presentó el mejor desempeño bajo el criterio de selección adoptado, priorizando métricas como recall y F1-score.

Asimismo, se utilizó Random Forest como apoyo interpretativo para analizar la importancia de variables.

---

## Aplicación

El modelo puede utilizarse para:

- priorizar auditorías médicas  
- optimizar la asignación de recursos  
- reducir pérdidas económicas asociadas a fraude  

---

## Ejecución

Abrir el notebook:

```bash
jupyter notebook Healthcare_Fraud_Detection_Project.ipynb
```

1. Ejecutar todas las celdas en orden secuencial (de arriba hacia abajo) para reproducir el análisis completo del proyecto.
El notebook realiza los siguientes pasos:
- Importación de librerías y configuración
- Carga e integración de múltiples fuentes de datos
- Limpieza y preparación de datos
- Generación de variables (feature engineering) a nivel proveedor
- Definición y entrenamiento de modelos (Logistic Regression, Random Forest y Gradient Boosting)
- Evaluación de métricas (recall, F1-score, entre otras)
- Comparación de modelos y selección del modelo final
- Análisis de importancia de variables

Al finalizar, se obtienen las métricas de desempeño y los gráficos que permiten interpretar los resultados del modelo.

---

## Autora

Moyra Blanco Panzich Vrdoljak
