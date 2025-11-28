# Análisis de Expectativas Económicas en el Perú

## Descripción del Proyecto

Nuestro trabajo final integra todos los elementos desarrollados a lo largo del curso, combinando exploración rigurosa de datos (EDA), modelos lineales y no lineales, regularización, ensambles, análisis causal mediante DAGs y estimación basada en redes neuronales tipo MLP. El objetivo es construir un análisis completo, técnico y reproducible que permita comprender e interpretar cómo las variables macroeconómicas inciden en la formación de expectativas económicas de los agentes.

### Pregunta de Investigación

**¿En qué medida la dinámica macroeconómica —inflación, tipo de cambio, actividad económica y política monetaria— influye en que los agentes económicos adopten expectativas optimistas o pesimistas sobre la economía peruana?**

## Estructura del Proyecto

### 1. Introducción y Configuración
- **Contexto**: La economía peruana ha experimentado choques significativos en los últimos años (pandemia, presiones inflacionarias, volatilidad cambiaria y fluctuaciones en política monetaria)
- **Relevancia**: Las expectativas cumplen un rol central en la toma de decisiones de consumo, inversión y planificación empresarial
- **Fuente de datos**: Banco Central de Reserva del Perú (BCRP)

### 2. Metodología

#### 2.1. Análisis Exploratorio de Datos (EDA)
- Exploración inicial de las variables macroeconómicas
- Análisis de distribución del índice de expectativas
- Creación de variable objetivo binaria (optimista/pesimista)

#### 2.2. Modelo Logit
- Establecimiento de línea base para predecir expectativas optimistas
- Modelo lineal como punto de partida

#### 2.3. Modelos No Lineales
- **Random Forest**: Captura relaciones no lineales entre variables
- **XGBoost**: Modelo de ensamble más sofisticado
- Comparación de desempeño con el modelo Logit

#### 2.4. Análisis Causal
- **DAGs (Directed Acyclic Graphs)**: Clarificación de supuestos sobre relaciones entre variables
- Marco teórico para interpretación causal

#### 2.5. Red Neuronal (MLP)
- Arquitectura flexible para mejorar predicción del optimismo económico
- Comparación con modelos tradicionales

### 3. Variables del Dataset

- **Fecha**: Serie temporal desde enero 2015
- **Tasa_Referencia_PM**: Tasa de referencia de política monetaria 
- **Expectativas_Economia**: Índice de expectativas económicas
- **Tipo_Cambio_Promedio**: Tipo de cambio promedio 
- **PBI_Mensual**: Producto Bruto Interno mensual 
- **IPC**: Índice de Precios al Consumidor 

### 4. Hallazgos Principales

#### 4.1. Distribución de Expectativas
- Concentración de valores entre 40-55 puntos (expectativas moderadas)
- Proporción balanceada: 55% no optimistas vs 45% optimistas
- Presencia de valores extremadamente bajos en períodos de crisis

#### 4.2. Variables Macroecónomicas
- **Tasa de referencia**: Rango amplio (0.25%-7.75%) refleja cambios en política monetaria
- **Tipo de cambio**: Volatilidad moderada (3.01-4.11 PEN/USD)
- **PBI**: Crecimiento económico con fluctuaciones
- **IPC**: Tendencia inflacionaria evidente

### 5. Tecnologías Utilizadas

- **Librerías principales empleadas**:
  - pandas, numpy: Manipulación de datos
  - scikit-learn: Modelos de machine learning
  - matplotlib, seaborn: Visualización
  - xgboost: Algoritmos de ensamble
  - causalgraphicalmodels: Análisis causal

### 6. Resultados Esperados

1. **Descripción completa** del comportamiento de variables macroeconómicas y expectativas
2. **Modelos predictivos** robustos para anticipar cambios en el optimismo económico
3. **Análisis causal** que conecte teoría económica con evidencia empírica
4. **Comparación metodológica** entre enfoques estadísticos y de machine learning
5. **Interpretación económica** de resultados para toma de decisiones

### 7. Aplicaciones Prácticas

- **Política económica**: Informar decisiones de política monetaria y fiscal
- **Sector empresarial**: Mejorar planificación estratégica basada en expectativas
- **Análisis de riesgo**: Evaluar vulnerabilidades económicas
- **Investigación académica**: Contribuir al entendimiento de formación de expectativas


---

