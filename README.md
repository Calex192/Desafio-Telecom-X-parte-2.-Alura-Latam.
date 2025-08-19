[readme.md](https://github.com/user-attachments/files/21855905/readme.md)

# Predicción de Churn en Telecomunicaciones

Este repositorio contiene un análisis completo sobre cancelación de clientes (churn) en una empresa de telecomunicaciones, utilizando diferentes modelos de Machine Learning para identificar los factores que más influyen en la fuga de clientes y proponer estrategias de retención.  

## Contenido del repositorio

- **`Telecom_part2.ipynb`** → Cuadernillo principal con:  
  - Exploración de datos y correlaciones con churn.  
  - Preparación y reducción de variables relevantes.  
  - Entrenamiento y evaluación de distintos modelos de clasificación (Random Forest, KNN, entre otros).  
  - Métricas de desempeño (accuracy, F1-score, recall, matriz de confusión).  
  - Identificación de las variables más influyentes en la cancelación.  
  - Conclusiones y estrategias de negocio para retención de clientes.  

- **README.md** → Documento explicativo (este archivo).  

## Modelos utilizados

- **Random Forest Classifier**  
  - Buen balance entre accuracy y recall.  
  - F1-score en test cercano al 0.77.  

- **K-Nearest Neighbors (KNN)**  
  - Evaluación con ajuste de `n_neighbors`.  
  - Menor rendimiento en general comparado con Random Forest.  

## Principales hallazgos

- **Factores más influyentes en churn**:  
  - `tenure` (antigüedad del cliente): los clientes nuevos son más propensos a cancelar.  
  - `charges.monthly` (cargo mensual): tickets altos se asocian a mayor churn.  
  - `internetservice_fiber optic`: usuarios de fibra óptica muestran mayor probabilidad de fuga.  
  - `paperlessbilling` y `seniorcitizen` también contribuyen al riesgo.  

- **Rendimiento de modelos**:  
  - Random Forest fue el modelo con mejor desempeño en test.  
  - El recall en la clase de cancelación fue mejorado respecto a otros algoritmos, aunque aún hay margen de mejora.  

## Estrategias de retención propuestas

- **Onboarding/Nurturing**: acompañar activamente a los clientes en los primeros 90 días.  
- **Segmentación de alto ticket**: dar beneficios adicionales a usuarios de fibra óptica con cargos altos (descuentos progresivos, bundles, upgrades gratuitos).  
- **Lock-in positivo**: ofrecer servicios complementarios que aumenten el valor percibido y reduzcan el incentivo a cambiarse.  
- **Facturación clara**: reducir errores o sorpresas en la primera factura, ya que es una causa frecuente de cancelación temprana.  

## Tecnologías

- Python 3.x  
- Scikit-learn  
- Pandas / NumPy  
- Matplotlib / Seaborn  

## Autor

Proyecto desarrollado como práctica de análisis predictivo aplicado a churn en telecomunicaciones.  
