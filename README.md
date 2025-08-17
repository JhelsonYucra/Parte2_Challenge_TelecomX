# Challenge Telecom – Parte 2: Predicción de Cancelación de Clientes (Churn)

## Descripción
Este proyecto corresponde a la segunda parte del desafío **Telecom X** del programa Alura + Oracle Next Education.  
El objetivo fue construir modelos de *machine learning* para predecir la cancelación de clientes (*churn*), utilizando los datos tratados en la primera etapa.

El desarrollo se realizó en Google Colab, partiendo del archivo `datos_tratados.csv`.

---

## Flujo de trabajo
1. **Carga de datos tratados**: Importación del dataset trabajado en la Parte 1.  
2. **Preprocesamiento**:  
   - Eliminación de columnas irrelevantes  
   - Codificación de variables categóricas (*One-Hot Encoding*)  
   - Balanceo de clases con SMOTE  
   - Normalización aplicada solo en modelos sensibles a la escala  
3. **Modelado**:  
   - Regresión Logística  
   - Random Forest  
4. **Evaluación**:  
   - Exactitud, Precisión, Recall, F1-score  
   - Matriz de confusión  
5. **Interpretación de variables**:  
   - Coeficientes en la Regresión Logística  
   - Importancia de características en Random Forest  

---

## Resultados
- Ambos modelos mostraron señales de *overfitting*.  
- Random Forest alcanzó un desempeño ligeramente superior en pruebas.  
- Las variables más influyentes en la predicción fueron:  
  - Tipo de contrato  
  - Cargos mensuales  
  - Antigüedad del cliente  

---

## Tecnologías utilizadas
- Python  
- Pandas, Numpy, Matplotlib, Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  

---

## Conclusiones
El análisis permitió identificar los principales factores de la cancelación.  
Algunas estrategias sugeridas para la retención de clientes incluyen:  

- Incentivar contratos de mayor plazo  
- Revisar políticas de cobro en clientes con cargos elevados  
- Diseñar programas de fidelización para usuarios con poca antigüedad  


