# 📚 ETL Project: Goodreads vs Amazon  Detector de discrepancias en el Rating

## 🎯 Objetivo del Proyecto

Comparar ratings de libros entre Goodreads (comunidad de lectores) y Amazon (plataforma de compras) para identificar discrepancias y analizar patrones de comportamiento entre ambas audiencias.

---

## Resultados del Análisis de Viabilidad

**Matching Validado:**
- ✅ **~1,000 matches** de alta calidad (HIGH quality)

**Estrategia de Matching:**
- Normalización de títulos (remoción de artículos, puntuación, subtítulos)
- Validación cruzada por autor
- Filtrado de matches de baja confianza

---

## Arquitectura

Data (S3)
    books_clean.csv (Goodreads: 11,119 libros)
    Books_rating.csv (Amazon)
    books_data.csv (Amazon)
         ↓
    [Lambda 1: Extract & Clean]
         ↓
Cleaned  (S3)
     goodreads_cleaned.csv
    amazon_clean_merged.csv
         ↓
    [Lambda 2: Transform & Match]
         ↓
    [Lambda 3: Load to Database]
         ↓
   Dashboard (Streamlit)

##  Stack Tecnológico

**Cloud & Infrastructure:**
- AWS Lambda (Python 3.12)
- AWS S3 (Storage)

**Data Processing:**
- Pandas (ETL)
- FuzzyWuzzy (Matching)
- Regular Expressions (Normalización)

**Visualization:**
- Streamlit (Dashboard interactivo)
- Plotly/Matplotlib (Gráficas)



##  Progreso del Proyecto

###  Día 1 - Setup & Extract (Completado)
Análisis de viabilidad y matching
Creación de buckets S3
Lambda 1: Extract & Clean implementado
Pipeline de extracción funcionando
Validación de datos en S3
Limpieza básica de datos

###  Día 2 - Transform & Match (En progreso)
-  Lambda 2: Transform & Match
-  Normalización de títulos y autores
-  Matching con validación
-  Cálculo de discrepancias de ratings
