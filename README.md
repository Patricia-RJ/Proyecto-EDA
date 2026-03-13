# Proyecto-EDA

Realización de el Análisis Exploratorio de los Datos relacionados con campañas de marketing directo de una institución bancaria portuguesa.

El objetivo es:

- Limpiar y transformar los datos
- Analizar patrones y relaciones
- Visualizar información relevante
- Extraer conclusiones fundamentadas
- Construir un modelo sencillo de Machine Learning
- Presentar los resultados mediante un dashboard en Power BI

El proyecto sigue una estructura profesional basada en buenas prácticas de organización, control de versiones y separación por fases.

---

## 2. Tecnologías Utilizadas

- Python 3.11
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Power BI (Dashboard)
- Anaconda (gestión de entornos)
- Git & GitHub

---

## 3. Metodología de Trabajo

El proyecto se desarrolla siguiendo una metodología estructurada basada en ramas de Git para simular un entorno profesional.

### Estrategia de ramas

```
main
 └── dev
      ├── feature/data-cleaning
      ├── feature/eda-analysis
      ├── feature/ml-dashboard
      └── feature/report
```

### Función de cada rama

- **main**  
  Contiene la versión final estable lista para entrega o despliegue.

- **dev**  
  Rama de integración donde se unifican todas las funcionalidades antes de pasar a producción.

- **feature/data-cleaning**  
  Desarrollo de la limpieza, tratamiento de valores nulos, duplicados y transformación de variables.

- **feature/eda-analysis**  
  Implementación del análisis estadístico y exploratorio.

- **feature/ml-dashboard**  
  Desarrollo del modelo de Machine Learning para predecir la suscripción del depósito y dashboard explicativo.

- **feature/report**  
  Redacción del informe técnico final y documentación.

Esta estructura permite mantener el proyecto organizado, escalable y fácil de mantener.

---

## 4. Estructura del Proyecto

```
eda-proyecto/
│
├── data/
│   ├── raw/                     # Dataset original (sin modificar)
│   └── processed/               # Dataset limpio y transformado
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda_analysis.ipynb
│   └── 03_ml_model.ipynb
│
├── reports/
│   └── Informe_Proyecto_EDA.pdf
│
├── dashboard/
│   └── bank_marketing_dashboard.pbix
│
├── requirements.txt
└── README.md
```

---

## 5. Fase 1 — Limpieza y Transformación de Datos

Notebook: `01_data_cleaning.ipynb`

Procesos realizados:

- Carga y exploración inicial del dataset
- Identificación de valores nulos
- Tratamiento o eliminación de nulos
- Eliminación de duplicados
- Conversión de tipos de datos
- Creación de nuevas variables (si procede)
- Exportación del dataset limpio a:

```
data/processed/
```

---

## 6. Fase 2 — Análisis Exploratorio

Notebook: `02_eda_analysis.ipynb`

Análisis realizados:

- Estadística descriptiva (media, mediana, desviación estándar)
- Análisis de distribuciones
- Agrupaciones con `groupby()`
- Tablas resumen
- Análisis de correlación
- Identificación de patrones y posibles anomalías
- Análisis de factores relacionados con la suscripción del depósito

---

## 7. Fase 3 — Modelo de Machine Learning

Notebook: `03_ml_model.ipynb`

Se construye un modelo sencillo de Machine Learning para predecir si un cliente contratará el depósito.

El proceso incluye:

- Selección de variables relevantes
- División del dataset en train y test
- Escalado de variables
- Entrenamiento de un modelo de **Regresión Logística**
- Evaluación del modelo mediante:
  - Accuracy
  - Classification Report
  - Matriz de confusión

Además se aplica una mejora utilizando:

```python
class_weight="balanced"
```

para manejar el desbalanceo de la variable objetivo.

---

## 8. Visualización y Dashboard

Los resultados del análisis se presentan mediante un **dashboard interactivo en Power BI**.

El dashboard incluye visualizaciones como:

- Tasa de conversión de la campaña
- Distribución de clientes que contratan vs no contratan
- Contrataciones por canal de contacto
- Contrataciones por ocupación
- Relación entre variables económicas (Euribor) y comportamiento del cliente
- Línea temporal de contrataciones

Ubicación del dashboard:

```
dashboard/bank_marketing_dashboard.pbix
```

---

## 9. Configuración del Entorno

### Crear entorno virtual

```bash
conda create -n hackio python=3.11
conda activate hackio
```

### Instalar dependencias

```bash
pip install -r requirements.txt
```

O manualmente:

```bash
pip install pandas matplotlib seaborn scikit-learn jupyter
```

---

## 10. Ejecución del Proyecto

1. Clonar repositorio:

```bash
git clone <url_del_repositorio>
cd eda-proyecto
```

2. Activar entorno:

```bash
conda activate hackio
```

3. Ejecutar notebooks en orden:

- 01_data_cleaning  
- 02_eda_analysis  
- 03_ml_model

---

## 11. Informe Final

El proyecto incluye un informe técnico en Word que contiene:

- Contexto y objetivo del análisis
- Proceso de limpieza y decisiones tomadas
- Resultados del análisis exploratorio
- Interpretación de visualizaciones
- Resultados del modelo de Machine Learning
- Conclusiones y recomendaciones

Ubicación:

```
reports/informe Proyecto EDA.pdf
```

---

## Autora

Patricia Romo Jiménez