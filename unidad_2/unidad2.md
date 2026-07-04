# 📊 Unidad 2: Inferencia Estadística y Pruebas de Hipótesis
## 📁 Contenido Interno de la Unidad
Este directorio almacena de forma limpia y sistematizada la producción científica y algorítmica desarrollada en el bloque de cierre de la asignatura:
1. **Guías de Laboratorio (APE06 a APE10):** Resoluciones experimentales de distribuciones avanzadas, simulaciones estocásticas y contrastes de hipótesis.
2. **Evaluación Sumativa Final:** Cuaderno técnico (`Diyer_Torres_Examen_U2.ipynb`) con el desarrollo del Live Coding analítico de pruebas paramétricas.
3. **Origen de Datos (`data_source/`):** Base de datos gubernamental real sobre las remuneraciones del GAD Municipal de Loja.

---

## 🗺️ 1. Estructura de Actividades Prácticas Experimentales (Laboratorios)
Haga clic en cualquiera de los enlaces para revisar la documentación, el código y la resolución técnica interactiva:

* [📄 Laboratorio APE06: Distribuciones Continuas Notables](./APEs/APE06.ipynb)  
  *Estudio profundo de la Distribución Normal (Campana de Gauss), procesos de estandarización matemática y uso computacional del estadístico Z.*
* [📄 Laboratorio APE07: Distribuciones Muestrales y Teorema del Límite Central (TLC) mediante Simulación Estocástica](./APEs/APE07.ipynb)  
  *Generación de múltiples muestras aleatorias por computadora para validar el comportamiento exponencial del TLC en la estimación de parámetros.*
* [📄 Laboratorio APE08: Inferencia Estadística: Estimación de Parámetros e Intervalos de Confianza (Z y T de Student)](./APEs/APE08.ipynb)  
  *Construcción de márgenes de error e intervalos de confianza paramétricos para estimar medias poblacionales bajo escenarios de varianza conocida y desconocida.*
* [📄 Laboratorio APE09: Inferencia Estadística: Pruebas de Hipótesis Paramétricas (Z y T) y Análisis del Valor-p](./APEs/APE09.ipynb)  
  *Diseño y ejecución de contrastes de hipótesis de una y dos muestras, analizando el valor-$p$ como métrica crítica para el rechazo de la hipótesis nula.*
* [📄 Laboratorio APE10: Inferencia Estadística Multigrupo: Análisis de Varianza (ANOVA de 1 factor) y Pruebas Post-Hoc (Tukey)](./APEs/APE10.ipynb)  
  *Modelamiento lineal y comparación múltiple simultánea para identificar diferencias salariales significativas entre más de dos regímenes laborales institucionales.*

---

  ## 📝 2. Evaluaciones Sumativas (Exámenes)
* [💻 Examen Práctico Unidad 2](./Proyecto_Inferencia_Estadistica_Diyer.ipynb)  
  *Desarrollo e implementación del examen práctico de la asignatura, ejecutando el pipeline completo de análisis paramétrico, pruebas multigrupo y validación estadística.*

---

  ## 🎥 3. Defensa Audiovisual y Sustentación Técnica
* [▶️ Video de la Defensa](https://drive.google.com/file/d/1bvQgsiUKIJ2Pve4-Gmm1vgcHzdcoHBJ9/view?usp=sharing)  
  *Exposición técnica y demostración en vivo donde se sustenta el criterio metodológico de las pruebas paramétricas, los grados de libertad y la interpretación rigurosa del valor-p.*

---

## 📓 4. Bitácora de Autoevaluación y Reflexión Crítica

### A. Aprendizajes Significativos Adquiridos
Durante esta unidad de inferencia estadística, el aprendizaje trascendió la teoría matemática tradicional hacia la automatización, simulación y modelamiento computacional avanzado:
* **Modelamiento de Variables Notables:** Análisis de funciones de masa (PMF) y distribución acumulada (CDF) para fenómenos discretos (Binomial y Poisson) y la estandarización continua mediante la Campana de Gauss utilizando la tabla Z.
* **Simulación Estocástica del TLC:** Demostración algorítmica de cómo la suma de variables aleatorias independientes e idénticamente distribuidas converge a una normal, aproximando también la distribución binomial mediante software.
* **Abstracción de Modelos Inferenciales:** Dominio práctico de la librería `scipy.stats` para pruebas unimuestrales ($t$ de Student) y la versatilidad de las fórmulas tipo R en `statsmodels` (`ols`) para ejecutar un Análisis de Varianza (ANOVA) de un factor.
* **Rigurosidad del Contraste Múltiple:** Comprensión del Error de Familia (FWER) y la obligatoriedad matemática de aplicar algoritmos post-hoc como la prueba de Tukey HSD para controlar la inflación del error Tipo I al contrastar múltiples subgrupos.

### B. Dificultades Algorítmicas Superadas
La manipulación y limpieza de las bases de datos del GAD de Loja presentó desafíos técnicos complejos que requirieron destrezas avanzadas de ingeniería de datos:
1. **Resolución de Conflictos de Formato e Inferencia (`UnicodeDecodeError`):** Se superó la barrera de formatos inconsistentes migrando de parsers planos (`pd.read_csv`) a motores estructurados de lectura de hojas de cálculo comprimidas mediante la dependencia `openpyxl`.
2. **Sanitización Dinámica de Atributos (Strings):** Los encabezados originales presentaban espacios invisibles y discrepancias de tildes (ej. `"Remuneración mensual unificada "`), lo cual rompía las fórmulas del modelo OLS. Se resolvió aplicando transformaciones vectorizadas `df.columns.str.strip()`.
3. **Interpretación Escalar en Muestras Masivas:** Al trabajar con una muestra robusta ($N = 2883$), se asimiló matemáticamente por qué los estadísticos $t$ y $F$ se disparaban a magnitudes tan elevadas y los valores-$p$ caían a escalas infinitesimales en notación científica (`e-236`). Se comprendió que a mayor tamaño muestral, el error estándar disminuye drásticamente, incrementando el poder de resolución del algoritmo.

### C. Conclusión del Proceso
Esta unidad consolidó la intersección natural entre la **Computación** y la **Estadística**. El desarrollo de este portafolio demuestra que la programación científica es una herramienta indispensable para transformar datos crudos gubernamentales en conocimiento analítico real, transparente y auditable para nuestra sociedad.
