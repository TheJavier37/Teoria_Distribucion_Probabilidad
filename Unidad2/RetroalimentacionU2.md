# 📓 **Bitácora de Aprendizaje y Autoevaluación**

## 🧭 **1. Resumen del Aprendizaje Alcanzado**

Durante el desarrollo de esta unidad de cierre y la ejecución de este examen práctico, consolidé competencias críticas en ciencia de datos aplicada al ámbito macroambiental:
* **Inferencia Unimuestral vs. Multigrupo:** Comprendí el rol metodológico de la distribución $T$ de Student cuando la varianza poblacional ($\sigma$) es una incógnita, y cómo el Análisis de Varianza (ANOVA) desglosa las fuentes de variabilidad mediante el estadístico $F$ de Snedecor.
* **Control del Error Experimental:** Aprendí el peligro de la inflación del Error de Tipo I (falsos descubrimientos) al realizar múltiples comparaciones. Logré dominar el uso del algoritmo Post-Hoc de Tukey HSD como el mecanismo matemático ideal para preservar la tasa de error familiar al 95%.
* **Estructuración Algorítmica:** Pasé de la teoría matemática abstracta a la implementación computacional real, utilizando abstracciones avanzadas de `scipy.stats` y `statsmodels` para modelar dinámicas geográficas complejas (microclimas).

---

## 🛠️ **2. Dificultades Algorítmicas y Conceptuales Superadas**

### **La encrucijada de la violación de supuestos**
* **El Desafío:** Al ejecutar la prueba de Shapiro-Wilk, el subgrupo *Húmeda-Andina* arrojó un p-valor de $0.0077$, lo que inicialmente interpreté como una invalidación total para proceder con el modelo paramétrico lineal del ANOVA.
* **La Solución:** Mediante una revisión teórica profunda vinculada a los APEs anteriores, superé la rigidez conceptual comprendiendo el **Principio de Robustez del ANOVA**. Logré justificar la continuidad del test fundamentándome en el **Teorema del Límite Central (TLC)**, ya que al disponer de un diseño experimental balanceado y una muestra de tamaño representativo ($n = 120$), las medias muestrales convergen asintóticamente a la normalidad distributiva.

### **Optimización del entorno gráfico**
* **El Desafío:** Depurar mensajes de advertencia (*FutureWarnings*) en la consola debido a la depreciación de sintaxis en las librerías de visualización (`seaborn`), lo que restaba formalidad al reporte gráfico.
* **La Solución:** Modifiqué la estructura del script asignando de manera explícita el parámetro `hue` en el diagrama de cajas y bigotes, y limpiando los argumentos redundantes de la leyenda, logrando un renderizado impecable y estandarizado.

---

## 📊 **3. Escala de Autoevaluación Cualitativa**

| Criterio Evaluado | Nivel Alcanzado | Justificación Técnica |
| :--- | :---: | :--- |
| **Dominio Matemático** | Impecable | Formulación matemática rigurosa y correcta interpretación de las notaciones de hipótesis en $\LaTeX$. |
| **Criterio de Ingeniería** | Excelente | Capacidad de auditar supuestos estadísticos y tomar decisiones amparadas en teoremas asintóticos de la probabilidad. |
| **Defensa del Código** | Fluido | Buena comprensión  de los parámetros del script (grados de libertad, métricas del estadístico y escalas del error estándar). |

> 🎯 **Reflexión Final:** Este proyecto individual me demostró que la estadística inferencial no consiste únicamente en la ejecución mecánica de algoritmos en Python, sino en el criterio interpretativo y la honestidad intelectual para aprender más sobre la asignatura.

Atentamente, Javier Guarnizo 
