# Proyecto-EDA
Realización de el Análisis Exploratorio de los Datos relacionados con campañas de marketing directo de una institución bancaria portuguesa. 
El objetivo es:

- Limpiar y transformar los datos
- Analizar patrones y relaciones
- Visualizar información relevante
- Extraer conclusiones fundamentadas
- Presentar los resultados mediante un informe técnico
- (Opcional – Nivel avanzado) Implementar un dashboard web con Django para visualizar métricas y gráficos

El proyecto sigue una estructura profesional basada en buenas prácticas de organización, control de versiones y separación por fases.

---

## 🛠️ 2. Tecnologías Utilizadas

- Python 3.11
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Django (Dashboard Web)
- Anaconda (gestión de entornos)
- Git & GitHub

---

## 🧭 3. Metodología de Trabajo

El proyecto se desarrolla siguiendo una metodología estructurada basada en ramas de Git para simular un entorno profesional.

### 🌿 Estrategia de ramas

```
main
 └── dev
      ├── feature/data-cleaning
      ├── feature/eda-analysis
      ├── feature/visualizations
      └── feature/report
```

### 📌 Función de cada rama

- **main**  
  Contiene la versión final estable lista para entrega o despliegue.

- **dev**  
  Rama de integración donde se unifican todas las funcionalidades antes de pasar a producción.

- **feature/data-cleaning**  
  Desarrollo de la limpieza, tratamiento de valores nulos, duplicados y transformación de variables.

- **feature/eda-analysis**  
  Implementación del análisis estadístico y exploratorio.

- **feature/visualizations**  
  Desarrollo de gráficos y exportación de visualizaciones.

- **feature/report**  
  Redacción del informe técnico final y documentación.

Esta estructura permite mantener el proyecto organizado, escalable y fácil de mantener.

---

## 📂 4. Estructura del Proyecto

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
│   └── 03_visualizations.ipynb
│
├── reports/
│   ├── figures/                 # Gráficos exportados en PNG
│   └── informe_final.docx
│
├── dashboard/                   # Proyecto Django
│   ├── manage.py
│   ├── eda_dashboard/
│   └── app/
│
├── requirements.txt
└── README.md
```

---

## 🧹 5. Fase 1 — Limpieza y Transformación de Datos

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

## 📊 6. Fase 2 — Análisis Exploratorio

Notebook: `02_eda_analysis.ipynb`

Análisis realizados:

- Estadística descriptiva (media, mediana, desviación estándar)
- Análisis de distribuciones
- Agrupaciones con `groupby()`
- Tablas resumen
- Análisis de correlación
- Identificación de patrones y posibles anomalías

---

## 📈 7. Fase 3 — Visualización de Datos

Notebook: `03_visualizations.ipynb`

Visualizaciones desarrolladas con:

- Matplotlib
- Seaborn

Tipos de gráficos utilizados:

- Histogramas
- Boxplots
- Gráficos de dispersión
- Heatmap de correlación

Los gráficos se exportan en formato PNG en:

```
reports/figures/
```

---

## 🌐 8. Fase 4 — Dashboard Web con Django

Como extensión del proyecto, se implementa un dashboard web básico utilizando Django para mostrar:

- Indicadores clave (KPIs)
- Tablas resumen
- Visualizaciones generadas en el EDA

### 🔹 Creación del proyecto Django

Desde la raíz del repositorio:

```bash
django-admin startproject eda_dashboard dashboard
cd dashboard
python manage.py startapp app
```

### 🔹 Ejecutar servidor local

```bash
cd dashboard
python manage.py runserver
```

Acceso en navegador:

```
http://127.0.0.1:8000/
```

Las visualizaciones pueden integrarse:

- Como imágenes exportadas desde el EDA
- O mediante librerías frontend (Chart.js / Plotly)

Esta fase demuestra capacidad de integración entre análisis de datos y desarrollo web.

---

## ⚙️ 9. Configuración del Entorno

### 🔹 Crear entorno virtual

```bash
conda create -n hackio python=3.11
conda activate hackio
```

### 🔹 Instalar dependencias

```bash
pip install -r requirements.txt
```

O manualmente:

```bash
pip install pandas numpy matplotlib seaborn jupyter django
```

---

## 🚀 10. Ejecución del Proyecto

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
- 03_visualizations

4. (Opcional) Ejecutar dashboard:

```bash
cd dashboard
python manage.py runserver
```

---

## 📄 11. Informe Final

El proyecto incluye un informe técnico en Word que contiene:

- Contexto y objetivo del análisis
- Proceso de limpieza y decisiones tomadas
- Resultados del análisis exploratorio
- Interpretación de visualizaciones
- Conclusiones y recomendaciones

Ubicación:

```
reports/informe_final.docx
```

---


## 👩‍💻 Autora

Patricia Romo Jiménez  

