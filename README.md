# Healthcare Fraud Detection using Machine Learning

Repositorio correspondiente al Proyecto Final Integrador de la Diplomatura en Ciencia de Datos y Análisis Avanzado.

El objetivo del proyecto es identificar proveedores médicos con comportamientos atípicos potencialmente asociados a fraude, a partir del análisis de datos de facturación. Para ello, se integraron múltiples fuentes de información y se desarrolló un modelo de Machine Learning orientado a detectar patrones relevantes y asistir en procesos de auditoría.

---

## Contenido

- Healthcare_Fraud_Detection_Project.ipynb: Notebook principal con el desarrollo completo del proyecto (EDA, feature engineering, modelado y evaluación).
- data/: Carpeta donde deben ubicarse los archivos del dataset descargados desde Kaggle.
- README.md: Documentación del proyecto.

---

## Requisitos

- Python 3.10 o superior  
- Librerías: `pandas`, `numpy`, `scikit-learn`, `matplotlib`  
- Opcional: `xgboost`, `shap`

---

## Instalación

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

## Datos

El dataset utilizado corresponde a:

Healthcare Provider Fraud Detection – Kaggle  
https://www.kaggle.com/datasets/rohitrox/healthcare-provider-fraud-detection-analysis

Se utilizaron únicamente los archivos de entrenamiento:

- Train_Beneficiarydata.csv  
- Train_Inpatientdata.csv  
- Train_Outpatientdata.csv  
- Train.csv  

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

El modelo Random Forest presentó el mejor desempeño, destacándose en métricas como recall y F1-score, lo que indica una mayor capacidad para detectar correctamente los casos de fraude y reducir falsos negativos.

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

Ejecutar las celdas en orden:

1. carga de datos  
2. integración  
3. limpieza  
4. feature engineering  
5. entrenamiento  
6. evaluación  

---

## Uso en Google Colab

Si se ejecuta en Google Colab:

- Subir manualmente los archivos CSV  
- Ubicarlos en /content/  

---

## Autora

Moyra Blanco Panzich Vrdoljak
