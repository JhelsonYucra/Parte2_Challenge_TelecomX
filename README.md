# 📊 Telecom X – Parte 2: Predicción de Cancelación (Churn)

Este proyecto corresponde a la segunda parte del desafío de **Alura**: desarrollar modelos predictivos para anticipar la cancelación de clientes (*churn*) en una empresa de telecomunicaciones.

---

## 🚀 Objetivo
Construir un pipeline de Machine Learning capaz de:
- Identificar qué clientes tienen mayor probabilidad de cancelar.  
- Analizar los factores más relevantes que influyen en la cancelación.  
- Proponer estrategias de retención basadas en los resultados obtenidos.  

---

## 📂 Flujo del Proyecto
1. **Carga de datos tratados**  
   Se parte del dataset ya limpiado y transformado en la Parte 1 del desafío.  

2. **Preprocesamiento**  
   - Eliminación de columnas irrelevantes (`customerID`).  
   - Codificación de variables categóricas (One-Hot Encoding).  
   - Verificación y balanceo de clases (SMOTE).  
   - Normalización/Estandarización (para modelos basados en distancia).  

3. **Análisis exploratorio dirigido**  
   - Correlación entre variables y churn.  
   - Relación entre *antigüedad*, *cargos* y cancelación.  

4. **Modelado**  
   - Modelos utilizados:  
     - **Regresión Logística** (sensible a la escala, requiere normalización).  
     - **Random Forest** (modelo basado en árboles, no sensible a la escala).  

5. **Evaluación de Modelos**  
   Métricas aplicadas:  
   - Exactitud (Accuracy)  
   - Precisión  
   - Recall  
   - F1-score  
   - Matriz de confusión  

6. **Interpretación**  
   - Regresión Logística: análisis de coeficientes.  
   - Random Forest: importancia de variables.  

7. **Conclusiones y Recomendaciones**  
   - Los clientes más nuevos presentan mayor riesgo de cancelar.  
   - Los cargos mensuales altos incrementan la probabilidad de churn.  
   - Los contratos mensuales y la facturación online son factores asociados a cancelación.  
   - Estrategias sugeridas:  
     - Incentivar contratos a largo plazo.  
     - Mejorar experiencia de facturación digital.  
     - Ofrecer beneficios a clientes en sus primeros meses.  

---

## 📈 Resultados Principales
- **F1-Score en test**:  
  - Regresión Logística: ~0.58  
  - Random Forest: ~0.59  
- Ambos modelos presentaron **overfitting**, con mejor rendimiento en entrenamiento que en prueba.  

---

## 🔧 Próximos Pasos
- Optimización de hiperparámetros (GridSearchCV / RandomizedSearchCV).  
- Uso de pipelines con validación cruzada + SMOTE integrado.  
- Ajuste del umbral de decisión para mejorar recall.  
- Implementación de modelos más robustos (XGBoost, LightGBM).  

---

## 📌 Requisitos
- Python 3.8+  
- Librerías principales:  
  - `pandas`, `numpy`, `matplotlib`, `seaborn`  
  - `scikit-learn`  
  - `imblearn`  

---

## 👤 Autor
Proyecto desarrollado por **Jhelson Yucra** como parte del desafío *Alura – Machine Learning*.
