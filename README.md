# Detección de Fraude en Facturación Médica – Proyecto Final Integrador

Este repositorio contiene el código y los recursos correspondientes al Proyecto Final Integrador del Diplomado en Ciencia de Datos y Análisis Avanzado.

El objetivo del proyecto es identificar proveedores médicos potencialmente fraudulentos a partir del análisis de datos de reclamos, utilizando técnicas de Machine Learning y siguiendo la metodología CRISP-DM.

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

Descargar el dataset "Healthcare Provider Fraud Detection" desde Kaggle y colocar los archivos en la carpeta data/.

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
