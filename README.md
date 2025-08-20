# 📊 Telecom X — Análisis de Churn (EDA + Modelado)

Este proyecto desarrolla un **pipeline completo de analítica y machine learning** aplicado a datos de clientes de TelecomX.  
El objetivo es **entender los factores que impulsan la cancelación de clientes (churn)** y proponer estrategias de retención basadas en evidencia.

---

## 🚀 Contenido del Notebook
1. **Extracción / ETL**  
   - Lectura de JSON desde repositorio público.  
   - Normalización de estructuras (`customer`, `account`, `internet`, `phone`).  
   - Unión en un único DataFrame para análisis.

2. **Transformación (ETL)**  
   - Limpieza de valores vacíos y casting numérico.  
   - Normalización de la variable target (`Churn`).  
   - Creación de variables derivadas (ej. `Cuentas_Diarias`).  

3. **EDA — Análisis Exploratorio de Datos**  
   - Distribución general de churn (barplot + pie chart).  
   - Variables categóricas vs churn (proporciones).  
   - Variables numéricas vs churn (boxplots).  
   - Dispersión (`MonthlyCharges` vs `TotalCharges`).  
   - Matriz de correlación con variables numéricas y de servicios contratados.

4. **Modelado Predictivo**  
   - Preparación con **One-Hot Encoding** y **train/test split**.  
   - Entrenamiento de múltiples algoritmos:
     - **Regresión Logística**  
     - **Random Forest**  
     - **KNN**  
     - **SVM Lineal**  
   - Comparación con métricas:  
     - Matriz de confusión  
     - Curvas ROC y Precision-Recall (AUC / AP)

5. **Importancia de Variables**  
   - Coeficientes en Logística.  
   - Importancias de Random Forest.  

6. **Conclusiones e Insights**  
   - Contrato *month-to-month* y cargos mensuales altos → mayor churn.  
   - Tenure alto y acumulación de gasto → mayor retención.  
   - Estrategias recomendadas:  
     - Migrar clientes a contratos más largos.  
     - Ajustar pricing para clientes con ARPU alto.  
     - Bundles de valor agregado (seguridad, soporte).  
     - Campañas proactivas basadas en **scores de propensión a churn**.  

---

## 🛠️ Stack Tecnológico
- **Python 3.10+**
- **Pandas, NumPy** → ETL / manipulación de datos  
- **Matplotlib** → visualización  
- **Scikit-Learn** → modelado predictivo (LogReg, RF, KNN, SVM)  

---

## 📂 Estructura
```
📁 TelecomX-Churn
 ├── 📄 TelecomX_Churn_EDA_Modelado.ipynb   # Notebook principal
 ├── 📄 README.md                           # Este archivo
```

---

## 📌 Cómo usar
1. Clonar el repositorio o descargar el notebook.  
2. Instalar dependencias:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```
3. Ejecutar el notebook paso a paso (Jupyter / VSCode).  

---

## ✨ Autoría
Creado para fines de aprendizaje y divulgación en **LinkedIn**.  
Presenta un flujo reproducible, visual y fácil de entender para profesionales en **Data Science aplicado a Customer Analytics**.

---
