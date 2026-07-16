# Plan de Estudios: Data Science, Seguros & Trading

## MES 1: Estadística Descriptiva y Fundamentos de Datos
- [x] **Semana 1: Medidas de Tendencia Central y Dispersión**
    - [x] **Qué estudiar:** Media, mediana, moda. Varianza, desviación estándar y rango intercuartílico (IQR).
    - [x] **En Python:** `numpy.mean()`, `numpy.std()`, `pandas.DataFrame.describe()`.
    - [x] **Aplicación Práctica:**
        - **Seguros:** Calcular la prima promedio de camiones y entender su dispersión.
        - **Trading:** Calcular precio promedio de Bitcoin a 30 días y medir su volatilidad.

- [x] **Semana 2: Distribuciones de Probabilidad y Visualización**
    - [x] **Qué estudiar:** Distribución Normal (Campana de Gauss), sesgo (skewness), curtosis y *outliers*.
    - [x] **En Python:** `seaborn.histplot()`, `seaborn.boxplot()`.
    - [x] **Aplicación Práctica:**
        - **Seguros:** Graficar edades de conductores (detectar sesgos o errores como 150 años).
        - **Trading:** Graficar rendimientos diarios de acciones para demostrar colas pesadas.

- [ ] **Semana 3: Correlación y Covarianza**
    - [x] **Qué estudiar:** Coeficiente de correlación de Pearson y Spearman. Diferencia entre correlación y causalidad.
    - [x] **En Python:** `pandas.DataFrame.corr()`, `seaborn.heatmap()`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Matriz de correlación (¿A mayor peso del camión, mayor costo?).
        - **Trading:** Analizar correlación entre el precio del Oro y Bitcoin.

- [ ] **Semana 4: SQL + Probabilidad Básica**
    - [ ] **Qué estudiar:** Espacio muestral, eventos independientes y dependientes. Consultas SQL básicas (`SELECT`, `WHERE`, `GROUP BY`).
    - [ ] **En Python:** Conectar Python a SQL usando `sqlite3` o `SQLAlchemy`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Extraer base de datos vía SQL y calcular probabilidad simple de ubicación del cliente (ej. Texas vs California).

---

## MES 2: Probabilidad Avanzada e Inferencia Estadística
- [ ] **Semana 5: Probabilidad Condicional y Teorema de Bayes**
    - [ ] **Qué estudiar:** Probabilidad condicional $P(A|B)$ y Teorema de Bayes.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Probabilidad de accidente dado que el conductor es menor de 25 años.
        - **Trading:** Probabilidad de subida hoy dado que ayer cayó un 5%.

- [ ] **Semana 6: Distribuciones Binomial y de Poisson**
    - [ ] **Qué estudiar:** Modelado de eventos discretos. Poisson (intervalos de tiempo) y Binomial (éxito/fracaso).
    - [ ] **En Python:** `scipy.stats.poisson`, `scipy.stats.binom`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Usar Poisson para modelar el número de reclamos semanales en la MGA.
        - **Trading:** Calcular probabilidad de tener 5 días seguidos de ganancias (Binomial).

- [ ] **Semana 7: Muestreo y el Teorema del Límite Central (TLC)**
    - [ ] **Qué estudiar:** Población vs. Muestra. Importancia del TLC con muestras pequeñas. Error estándar.
    - [ ] **En Python:** `pandas.DataFrame.sample()`.
    - [ ] **Aplicación Práctica:**
        - **Seguros/Trading:** Demostrar que las medias de múltiples muestras forman una campana de Gauss.

- [ ] **Semana 8: Intervalos de Confianza**
    - [ ] **Qué estudiar:** Margen de error, niveles de confianza (95%, 99%) y Z-scores.
    - [ ] **En Python:** `scipy.stats.norm.interval()`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Estimar el costo promedio de reclamo con un 95% de confianza (ej. entre $4,800 y $5,200).

---

## MES 3: Pruebas de Hipótesis (Tomando decisiones con datos)
- [ ] **Semana 9: Fundamentos de Pruebas de Hipótesis**
    - [ ] **Qué estudiar:** Hipótesis Nula ($H_0$) e Alternativa ($H_1$), Errores Tipo I y II, y el *p-value*.
    - [ ] **Aplicación Práctica:**
        - **Estrategia:** Demostrar matemáticamente si una suposición de negocio es falsa o verdadera antes de codear.

- [ ] **Semana 10: Pruebas T de Student (T-Test)**
    - [ ] **Qué estudiar:** Comparación de medias entre dos grupos independientes.
    - [ ] **En Python:** `scipy.stats.ttest_ind`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Validar si los camiones pesados pagan significativamente más que los ligeros.
        - **Trading:** Evaluar si una estrategia rinde más los lunes que los viernes de forma real.

- [ ] **Semana 11: Prueba de Chi-Cuadrado ($\chi^2$)**
    - [ ] **Qué estudiar:** Pruebas de independencia para variables categóricas (texto/grupos).
    - [ ] **En Python:** `scipy.stats.chi2_contingency`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Analizar si el tipo de seguro está asociado con el estado de EE. UU. donde opera el camión.

- [ ] **Semana 12: SQL Avanzado para Segmentación**
    - [ ] **Qué estudiar:** `INNER JOIN`, `LEFT JOIN`, funciones de ventana (`ROW_NUMBER()`, `PARTITION BY`).
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Cruzar tabla de "Clientes" con "Pólizas Históricas" para dejar los datos listos para modelar.

---

## MES 4: Álgebra Lineal y Regresión Lineal (El inicio de la predicción)
- [ ] **Semana 13: Vectores y Matrices en Data Science**
    - [ ] **Qué estudiar:** Operaciones con matrices (Suma, multiplicación, transposición). Representación de datos.
    - [ ] **En Python:** Operaciones matriciales avanzadas usando `NumPy`.
    - [ ] **Aplicación Práctica:**
        - **Estructura:** Convertir una tabla de clientes entera en una matriz matemática para procesamiento veloz.

- [ ] **Semana 14: Regresión Lineal Simple**
    - [ ] **Qué estudiar:** Ecuación de la recta ($y = mx + b$), Mínimos Cuadrados (OLS) y métrica $R^2$.
    - [ ] **En Python:** `statsmodels.api.OLS` o `sklearn.linear_model.LinearRegression`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Predecir precio de prima ($y$) basado en años de experiencia del conductor ($x$).
        - **Trading:** Calcular el "Beta" de una acción frente al mercado.

- [ ] **Semana 15: Regresión Lineal Múltiple**
    - [ ] **Qué estudiar:** Predicción multivariable y el problema de la Multicolinealidad.
    - [ ] **En Python:** Modelado múltiple en `Scikit-Learn`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Crear software de cotización automático (Edad + Peso + Historial = Precio).

- [ ] **Semana 16: Métricas de Evaluación de Modelos**
    - [ ] **Qué estudiar:** MAE (Error Absoluto Medio) y RMSE (Raíz del Error Cuadrático Medio).
    - [ ] **Aplicación Práctica:**
        - **Seguros/Trading:** Medir el error del modelo (ej. "El algoritmo predice el precio con un error promedio de $15").

---

##  MES 5: Introducción al Machine Learning y Modelos de Clasificación
- [ ] **Semana 17: Regresión Logística (La matemática del Sí o No)**
    - [ ] **Qué estudiar:** Función Sigmoide y probabilidades Log-Odds. Predicción de pertenencia a categorías.
    - [ ] **En Python:** `sklearn.linear_model.LogisticRegression`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Calcular probabilidad de que un cliente cancele su póliza el próximo mes (*Churn rate*).
        - **Trading:** Clasificar si el mercado mañana cerrará en Alza (1) o Baja (0).

- [ ] **Semana 18: Matriz de Confusión y Métricas de Clasificación**
    - [ ] **Qué estudiar:** Precisión, Sensibilidad (*Recall*), F1-Score. Falsos Positivos vs. Falsos Negativos.
    - [ ] **En Python:** `sklearn.metrics.classification_report`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Detector de fraudes (Entender por qué es peor un falso negativo que un falso positivo).

- [ ] **Semana 19: Árboles de Decisión (Decision Trees)**
    - [ ] **Qué estudiar:** Entropía y Ganancia de Información para división lógica de datos.
    - [ ] **En Python:** `sklearn.tree.DecisionTreeClassifier`.
    - [ ] **Aplicación Práctica:**
        - **Seguros:** Generar árbol visual de riesgos (Ej: Si Edad < 25 y Estado == 'Texas' -> Riesgo Alto).

- [ ] **Semana 20: Automatización del Pipeline y Presentación**
    - [ ] **Qué estudiar:** Unir el código en un único script limpio (SQL -> Matemáticas -> Modelo -> Resultados).
    - [ ] **Aplicación Práctica:**
        - **Trabajo:** Presentar el primer sistema automatizado de analítica predictiva de seguros de camiones.