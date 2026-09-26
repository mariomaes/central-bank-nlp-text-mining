# NLP y Text Mining Aplicado a la Banca Central: Informes Anuales del Banco de España (2013–2022)

Proyecto de procesamiento de datos no estructurados y minería de texto en `R` (`quanteda`, `tidytext`, `tidyverse`) que analiza la evolución temática, macroeconómica y financiera del discurso oficial del **Banco de España (BdE)** a lo largo de diez años de Informes Anuales.

## 🛠️ Pipeline de Procesamiento y Análisis Textual
1. **Ingesta y Limpieza de Datos No Estructurados:** Extracción automatizada del texto de los informes anuales en formato PDF (2013–2022), normalización mediante expresiones regulares (regex), tokenización y filtrado de *stopwords*.
2. **Análisis Léxico y N-Gramas:** Evolución temporal y agregada de frecuencias de términos, construcción de **bigramas y trigramas** por año para capturar conceptos económicos compuestos (p. ej., política monetaria, deuda pública, tipos de interés, inflación).
3. **Ponderación TF-IDF:** Identificación de los términos con mayor especificidad informativa en cada ejercicio anual, aislando los *shocks* macroeconómicos propios de cada etapa (recuperación post-crisis soberana, pandemia COVID-19 en 2020, crisis inflacionaria y energética en 2021-2022).
4. **Estadística Textual Avanzada (`quanteda`):**
   * Matrices de **similitud entre documentos** y correlación temporal de términos clave.
   * Análisis de **Keyness** para contrastar estadísticamente el cambio de vocabulario entre distintos periodos económicos.
   * Exploración contextual mediante **KWIC (*Keyword in Context*)** y grafos de **redes de co-ocurrencia semántica**.
