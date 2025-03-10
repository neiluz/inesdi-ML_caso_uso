# Caso de Uso:   Proyecto de ML para la Predicción de Fraude Energético
## 📌 Descripción del Proyecto

El fraude energético representa un desafío significativo para las empresas del sector, generando pérdidas económicas y afectando la distribución justa del servicio. Este proyecto tiene como objetivo desarrollar un sistema de detección automatizada de fraude utilizando técnicas de Machine Learning, permitiendo a las compañías priorizar inspecciones y mitigar riesgos financieros.

Para ello, exploramos y analizamos datos históricos de clientes y consumos, aplicamos métodos avanzados de preprocesamiento, balanceo de clases y optimización de modelos para mejorar la precisión y recall en la identificación de fraudes. Además, implementamos estrategias de ensamblado y modelos en cascada para mejorar la clasificación de casos dudosos y reducir falsos positivos.

## 📁 Estructura del Proyecto

El proyecto se divide en tres notebooks principales:

1. **Notebook_1_EDA.ipynb** → Análisis exploratorio de datos (EDA):
   - Integración de los datasets `clients.csv` e `invoices.csv`
   - Visualización de patrones y distribución de variables
   - Identificación de outliers y valores faltantes

2. **Notebook_2_pre_procesamiento_feature.ipynb** → Preprocesamiento y generación de características:
   - Limpieza de datos y manejo de valores nulos
   - Creación de nuevas variables a partir de las existentes
   - Codificación de variables categóricas y normalización

3. **Notebook_3_normalización_modelado.ipynb** → Modelado y evaluación:
   - Pruebas con distintos algoritmos (XGBoost, LightGBM, CatBoost, Random Forest, Regresión Logística)
   - Uso de estrategias de balanceo de clases (RUS, SMOTE)
   - Evaluación de métricas clave (Recall, F1-Score, AUC-ROC)
   - Implementación de modelos en cascada y ensamblado

## 🏗 Metodología

1. **Preparación de datos:**
   - Análisis de distribución de clases (fraude vs. no fraude)
   - Ingeniería de características clave
   - Normalización y selección de variables

2. **Modelado:**
   - Comparación de modelos de Machine Learning
   - Optimización de hiperparámetros
   - Evaluación de diferentes estrategias de balanceo

3. **Implementación de modelos avanzados:**
   - Sistema en cascada (XGBoost + LightGBM)

## 🚀 Cómo ejecutar el proyecto

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/proyecto_fraude_energetico.git
   cd proyecto_fraude_energetico
   ```

2. Crear un entorno virtual e instalar dependencias:
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Ejecutar los notebooks en Jupyter:
   ```bash
   jupyter notebook
   ```

## 📊 Resultados

- **Mejor modelo:** XGBoost con RUS_50_50
- **F1-Score óptimo:** 0.2245
- **Estrategia más efectiva:** Reducción de la clase mayoritaria + ajuste de umbrales
- **Sistema de dos etapas:** Se logró mejorar el recall sin comprometer excesivamente la precisión

## 📌 Conclusiones

- Se confirma la importancia de ajustar los umbrales de decisión para mejorar la detección de fraudes.
- El balanceo de clases mediante RUS y SMOTE mejora la capacidad de predicción.
- Un modelo en cascada puede reducir falsos positivos y mejorar la confiabilidad del sistema.

## 📌 Próximos pasos

- Ajustar hiperparámetros en mayor profundidad.
- Implementar técnicas de interpretación de modelos (SHAP, LIME).
- Explorar el uso de redes neuronales para mejorar la predicción.

---
📌 **Autores:** Neivys Luz González Gómez, Carlos Alamilla Medina, Luis Diego Gazel Quirós, Humberto David Hernández Pérez, Adrià Nuñez Fernández


