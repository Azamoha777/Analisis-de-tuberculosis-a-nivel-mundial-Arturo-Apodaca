
# Analisis-de-tuberculosis-a-nivel-mundial-Arturo-Apodaca
# Tuberculosis Global Dashboard

Análisis exploratorio y visualización interactiva de datos globales de tuberculosis utilizando Python, con información epidemiológica de la Organización Mundial de la Salud (OMS) correspondiente al periodo 1995–2013.

---

## Descripción del Proyecto

La tuberculosis (TB) continúa siendo una de las enfermedades infecciosas más importantes a nivel mundial debido a su impacto sanitario, económico y social. Este proyecto desarrolla un análisis exploratorio de datos (EDA) para identificar patrones epidemiológicos, tendencias temporales, distribución geográfica y comportamiento demográfico de la enfermedad a nivel global.

El análisis fue desarrollado en Python mediante Google Colab, utilizando herramientas de ciencia de datos para limpieza, transformación y visualización de información epidemiológica.

---

## Objetivo General

Realizar un análisis exploratorio de los datos globales de tuberculosis entre 1995 y 2013 para identificar:

- Tendencias epidemiológicas.
- Distribución geográfica de los casos.
- Diferencias demográficas por género y edad.
- Tasas de incidencia por país.
- Comportamiento temporal de la enfermedad.

---

## Dataset Utilizado

El proyecto utiliza el conjunto de datos:

- **WHO Tuberculosis Dataset**
- Información poblacional complementaria para cálculo de incidencia.

### Archivos principales

- `who.csv`
- `population.csv`

Los datos contienen información de:

- 219 países y territorios.
- Casos registrados entre 1995 y 2013.
- Género.
- Grupo de edad.
- Tipo de diagnóstico.
- Casos reportados.
- Población total por país y año.

---

## Herramientas y Tecnologías

### Lenguaje

- Python

### Entorno de trabajo

- Google Colab
- Jupyter Notebook

### Librerías utilizadas

```python
pandas
numpy
matplotlib
seaborn
plotly
```

---

## Proceso de Limpieza y Transformación

El dataset original contenía variables codificadas y múltiples valores faltantes, por lo que se realizó un proceso completo de preparación de datos:

- Corrección de valores nulos.
- Limpieza de códigos ISO.
- Transformación de formato ancho a formato largo usando `melt()`.
- Separación de variables codificadas:
  - género
  - método diagnóstico
  - grupo de edad
- Integración de datos poblacionales mediante `merge()`.
- Cálculo de tasas de incidencia por cada 100,000 habitantes.

Estas transformaciones permitieron construir una base estructurada y lista para análisis estadístico y visualización.

---

## Principales Hallazgos

### Tendencia Temporal

- Entre 1995 y 2010 los casos globales aumentaron significativamente.
- El pico máximo se alcanzó alrededor de 2010.
- A partir de 2011 comenzó una reducción progresiva de casos.

### Distribución Geográfica

Los países con mayor número absoluto de casos fueron:

- India
- China
- Indonesia
- Pakistán
- Bangladesh

Sin embargo, las mayores tasas de incidencia por habitante se concentraron principalmente en África Subsahariana:

- Sudáfrica
- Suazilandia
- Lesoto
- Namibia
- Kiribati

### Análisis Demográfico

#### Género

La tuberculosis afecta de manera desproporcionada a la población masculina.

#### Edad

Más del 60% de los casos se concentra entre los 15 y 44 años, afectando principalmente a la población económicamente activa.

### Métodos de Diagnóstico

El análisis incluye:

- Casos pulmonares con frotis positivo.
- Casos pulmonares con frotis negativo.
- Casos extrapulmonares.
- Casos de recaída.

---

## Visualizaciones Incluidas

El proyecto incorpora gráficas y dashboards interactivos para:

- Evolución temporal de casos.
- Comparación entre países.
- Tasas de incidencia.
- Distribución por género.
- Distribución por grupo de edad.
- Mapas epidemiológicos.
- Análisis de recaídas.

---

## Estructura del Proyecto

```bash
├── Limpieza de datos.ipynb
├── who.csv
├── population.csv
├── README.md
└── visualizaciones/
```

---

## Resultados Relevantes

- Más de 43 millones de casos registrados en el periodo analizado.
- Fuerte concentración geográfica de casos.
- África Subsahariana presenta las tasas más elevadas de incidencia.
- La población masculina y económicamente activa representa el grupo más afectado.
- Las recaídas continúan siendo un desafío importante para los sistemas de salud pública.

---

## Conclusiones

El análisis demuestra que la tuberculosis sigue siendo un problema crítico de salud pública mundial, especialmente en regiones con altos niveles de pobreza, desigualdad y acceso limitado a servicios médicos.

Asimismo, el proyecto evidencia el potencial de Python y las herramientas de ciencia de datos para transformar grandes volúmenes de información epidemiológica en evidencia útil para la toma de decisiones y formulación de políticas públicas.

---

## Autor

**Arturo Azamoha Apodaca Pérez**  
Universidad de Colima  
Análisis Exploratorio de Datos

---

## Referencias

- Organización Mundial de la Salud (OMS)
- WHO Tuberculosis Dataset
- Naciones Unidas
- Datos poblacionales utilizados para cálculo de incidencia

[Ver reporte interactivo en Power BI](https://app.powerbi.com/links/u7m7tLTvDX?ctid=e20c85ea-e344-4e55-aa34-5729d5b38c14&pbi_source=linkShare)

[Ver reporte interactivo en Power BI](https://app.powerbi.com/links/2H9LS3h_fQ?ctid=e20c85ea-e344-4e55-aa34-5729d5b38c14&pbi_source=linkShare)
