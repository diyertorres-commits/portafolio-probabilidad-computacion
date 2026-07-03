# 📈 Unidad 1: Fundamentos de Probabilidad y Distribuciones
## 📁 Contenido Interno de la Unidad
Este directorio almacena la producción experimental y analítica correspondiente al primer bloque de la asignatura:
1. **Guías de Laboratorio (APE00 a APE05):** Resoluciones detalladas y código enfocado en estadística descriptiva, cálculo probabilístico, modelamiento de variables aleatorias y cálculo de momentos.

---

## 🗺️ 1. Estructura de Actividades Prácticas Experimentales (Laboratorios)

* [📄 Laboratorio APE00: Fundamentos de Probabilidad y Espacios Muestrales](./APEs/APE00.ipynb)  
  *Establecimiento y simulación algorítmica de experimentos aleatorios, álgebra de eventos y cálculo de probabilidades clásicas y empíricas en Python.*
* [📄 Laboratorio APE01: Variables Aleatorias y Distribuciones de Probabilidad](./APEs/APE01.ipynb)  
  *Modelamiento computacional de variables aleatorias y evaluación de sus propiedades mediante funciones de masa y densidad de probabilidad.*
* [📄 Laboratorio APE02: Distribuciones Muestrales y Teorema del Límite Central](./APEs/APE02.ipynb)  
  *Demostración empírica del comportamiento de las medias muestrales y su convergencia asintótica hacia la normalidad estadística.*
* [📄 Laboratorio APE03: Variables Aleatorias Discretas y Continuas](./APEs/APE03.ipynb)  
  *Implementación de cálculo integral y numérico aplicado a densidades continuas frente a la acumulación discreta de datos.*
* [📄 Laboratorio APE04: Momentos Estadísticos y Análisis de Tendencia Central con Python](./APEs/APE04.ipynb)  
  *Cálculo automatizado de la Esperanza Matemática $E[X]$, Varianza Teórica $V[X]$ y momentos de orden superior para describir la forma de los datos.*
* [📄 Laboratorio APE05: Distribuciones Discretas Notables](./APEs/APE05.ipynb)  
  *Simulación y análisis de escenarios prácticos utilizando los modelos probabilísticos Binomial y de Poisson mediante `scipy.stats`.*

---

## 📓 2. Bitácora de Autoevaluación y Reflexión Crítica

### A. Aprendizajes Significativos Adquiridos
A lo largo de esta unidad fundamental, se sentaron las bases analíticas necesarias para la transición desde el análisis exploratorio clásico hacia el pensamiento estocástico formal:
* **Sistematización de Datos Crudos y Momentos:** Dominio de las medidas de tendencia central (Media $\mu$, Mediana y Moda) y de dispersión (Varianza $\sigma^2$ y Desviación Estándar $\sigma$), comprendiendo cómo resumen el comportamiento de una distribución a través del cálculo de momentos estadísticos con Python.
* **Modelamiento del Espacio Muestral:** Análisis de la probabilidad clásica, empírica y subjetiva, estructurando correctamente los eventos y las reglas fundamentales de adición y multiplicación.
* **Formalismo de Variables Aleatorias (V.A.):** Diferenciación matemática entre el soporte de una V.A. Discreta y una Continua, asimilando el uso de la Función de Masa de Probabilidad (PMF) y la Función de Densidad de Probabilidad (PDF), combinadas con las Distribuciones Discretas Notables.
* **Teorema del Límite Central:** Comprensión de cómo las distribuciones muestrales de la media tienden asintóticamente a la normalidad a medida que aumenta el tamaño de la muestra, sentando la base para la inferencia estadística de la siguiente unidad.

### B. Dificultades Algorítmicas Superadas
* **Modelamiento e Integración Analítica:** Una de las principales dificultades conceptuales radicó en comprender que la PDF en variables continuas no representa una probabilidad directa en un punto, sino una densidad, requiriendo el uso de cálculo integral o aproximaciones numéricas computacionales para hallar probabilidades sobre un intervalo.
* **Manipulación de Datos y Visualización de Densidades:** En el entorno de Python, la correcta escala al graficar histogramas de frecuencia frente a curvas de densidad teóricas requirió el dominio de parámetros clave como `density=True` en `matplotlib` o `sns.histplot`. Esto evitó discrepancias de escala entre conteos absolutos y áreas probabilísticas unitarias.

### C. Conclusión del Proceso
La Unidad 1 representó el puente indispensable entre la manipulación de software descriptivo y la fundamentación teórica de la computación científica. La asimilación de estos conceptos probabilísticos dota de sentido matemático a los análisis inferenciales avanzados que se ejecutan posteriormente sobre los conjuntos de datos de nuestra provincia.
