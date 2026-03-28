# Detección de Fraude en Facturación Médica – Proyecto Final Integrador

Este repositorio reúne el desarrollo del Proyecto Final Integrador del Diplomado en Ciencia de Datos y Análisis Avanzado.

El trabajo se centra en el análisis de datos de facturación médica con el objetivo de identificar proveedores que presentan comportamientos atípicos, potencialmente asociados a fraude. A partir de la integración de información de pacientes, prestaciones y proveedores, se desarrolló un enfoque de Machine Learning orientado a detectar estos patrones y aportar una herramienta de apoyo para procesos de auditoría.

---

## Contenido

- fraud_detection.ipynb: Notebook principal que incluye carga de datos, limpieza, integración, generación de variables, modelado y evaluación.

- data/: Carpeta donde deben colocarse los archivos del dataset descargados desde Kaggle.

- README.md: Documento descriptivo del proyecto.

---

## Requisitos

- Python 3.10 o superior  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  

---

## Instalación

Clonar o descargar el repositorio.

Crear un entorno virtual (opcional):

```
python -m venv env
```

Activar entorno:

En Windows:
```
env\Scripts\activate
```

En Mac/Linux:
```
source env/bin/activate
```

Instalar dependencias:

```
pip install pandas numpy scikit-learn matplotlib
```

---

## Descarga de datos

El dataset utilizado en este proyecto corresponde a "Healthcare Provider Fraud Detection", disponible en Kaggle.

Para el desarrollo del modelo se utilizaron exclusivamente los archivos de entrenamiento (Train), descartando los archivos de test.

En particular, se emplearon los siguientes archivos:

- Train_Beneficiarydata-1542865627584.csv  
- Train_Inpatientdata-1542865627584.csv  
- Train_Outpatientdata-1542865627584.csv  
- Train-1542865627584.csv  

Los archivos correspondientes a "Test" no fueron utilizados en este análisis.

### Instrucciones

1. Descargar el dataset desde Kaggle.  
2. Ubicar los archivos mencionados en la carpeta `data/` del repositorio.  

### Uso en Google Colab

Si se ejecuta el notebook en Google Colab, es necesario subir manualmente los archivos CSV:

- Ir al panel lateral izquierdo (ícono de carpeta)  
- Seleccionar "Subir archivos"  
- Cargar los archivos CSV utilizados  

Los archivos deben quedar en la ruta raíz (`/content/`) para que el notebook pueda acceder correctamente.
---

## Ejecución

Abrir el notebook:

```
jupyter notebook fraud_detection.ipynb
```

Ejecutar las celdas en orden:

- carga de datos  
- integración de tablas  
- limpieza  
- feature engineering  
- entrenamiento de modelos  
- evaluación  

---

## Modelado

Se evaluaron los siguientes modelos:

- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Dado el desbalance de clases, se priorizó la métrica recall.

---

## Resultados

El modelo Random Forest presentó el mejor desempeño general.

---

## Aplicación

El modelo puede utilizarse para:

- priorizar auditorías médicas  
- optimizar recursos  
- reducir pérdidas económicas  

---

## Fuente de datos

Healthcare Provider Fraud Detection – Kaggle

---

## Autora

Moyra Blanco Panzich Vrdoljak
