# Detección de Fraude en Facturación Médica – Proyecto Final Integrador


## Descripción del proyecto

Este proyecto tiene como objetivo detectar proveedores médicos potencialmente fraudulentos a partir del análisis de datos de reclamos de salud.

El trabajo se basa en la integración y análisis de múltiples fuentes de datos, incluyendo información de pacientes, proveedores y prestaciones médicas, con el fin de identificar patrones de comportamiento atípicos que puedan estar asociados a fraude.

---

## Dataset

Se utilizó el dataset público "Healthcare Provider Fraud Detection", disponible en Kaggle.

Este dataset contiene información anonimizada estructurada en múltiples tablas:

- Beneficiary: datos demográficos y clínicos de pacientes  
- Outpatient: reclamos médicos ambulatorios  
- Provider: información del proveedor y variable objetivo (PotentialFraud)  

Luego del proceso de integración, se obtuvo un dataset consolidado con:

- cientos de miles de registros  
- más de 50 variables  

Los datos no contienen información personal identificable, lo que permite su uso con fines analíticos.

---

## Problema a resolver

El fraude en la facturación médica representa una problemática relevante en los sistemas de salud, generando pérdidas económicas y dificultando la eficiencia de los procesos de auditoría.

Los métodos tradicionales de detección suelen ser manuales, lo que limita la capacidad de analizar grandes volúmenes de datos.

---

## Objetivo

Desarrollar un modelo de Machine Learning que permita identificar proveedores con alta probabilidad de fraude, utilizando información derivada de:

- volumen de reclamos  
- cantidad de diagnósticos  
- procedimientos realizados  
- montos facturados  
- características del paciente  

---

## Metodología

El proyecto se desarrolló siguiendo la metodología CRISP-DM, abordando las siguientes etapas:

1. Comprensión del negocio  
2. Comprensión de los datos  
3. Preparación de los datos  
4. Modelado  
5. Evaluación  

### Procesos realizados

- Integración de datasets mediante operaciones de merge  
- Limpieza de datos y tratamiento de valores faltantes  
- Feature engineering  
- Transformación de variables  
- División en conjunto de entrenamiento y prueba  

---

## Modelado

Se abordó el problema como una tarea de clasificación supervisada, donde la variable objetivo es PotentialFraud.

Se evaluaron distintos modelos:

- Logistic Regression (baseline)  
- Random Forest  
- Gradient Boosting  

Dado el desbalance de clases (aprox. 90% no fraude vs 10% fraude), se priorizó el uso de métricas adecuadas para este tipo de problemas.

---

## Evaluación de modelos

Se utilizaron las siguientes métricas:

- Precision  
- Recall  
- F1-score  
- Matriz de confusión  

El modelo Random Forest obtuvo el mejor desempeño general, logrando:

- mayor capacidad de detección de fraude (recall)  
- mejor equilibrio entre falsos positivos y falsos negativos  

Esto sugiere la presencia de relaciones no lineales en los datos, capturadas de forma más efectiva por modelos basados en árboles.

---

## Impacto en el negocio

La implementación de este modelo permitiría:

- priorizar auditorías médicas en proveedores de mayor riesgo  
- reducir costos asociados al fraude  
- optimizar el uso de recursos humanos  
- mejorar la eficiencia operativa  

En un entorno real, podría integrarse como herramienta de soporte para la toma de decisiones en áreas de auditoría.

---

## Limitaciones

- Dataset con desbalance de clases  
- Datos anonimizados sin contexto clínico completo  
- Posible mejora mediante técnicas de balanceo (SMOTE, etc.)  
- Posible incorporación de modelos más avanzados  

---

## Contenido del repositorio

- fraud_detection.ipynb: Notebook principal con el flujo completo del proyecto (carga de datos, limpieza, feature engineering, modelado y evaluación).

- data/: Carpeta destinada a almacenar los archivos del dataset (Beneficiary, Outpatient y Provider).  
  Nota: los archivos deben descargarse desde Kaggle y colocarse manualmente en esta carpeta.

- README.md: Documento descriptivo del proyecto.

---

## Cómo ejecutar el proyecto

1. Descargar el dataset desde Kaggle  
2. Colocar los archivos en la carpeta /data  
3. Abrir el notebook fraud_detection.ipynb en Jupyter o Google Colab  
4. Ejecutar las celdas en orden  

---

## Requisitos

- Python 3.x  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  

---

## Autora

Moyra Blanco Panzich Vrdoljak
