# ⚙️ Cálculo de Momentos de Inercia con Integración Numérica

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17La2lYeeEsNLuW0Yg8tYGCC9qMDvUg7R?usp=sharing)

Este proyecto aplica métodos numéricos avanzados para resolver problemas de **Dinámica de Maquinaria** y **Cálculo Vectorial**. Se desarrolló un algoritmo en Python capaz de calcular las propiedades inerciales (momentos y productos de inercia) de elementos mecánicos complejos mediante integrales múltiples, superando las limitaciones de los métodos analíticos tradicionales.

## 📄 Resumen del Proyecto

El objetivo principal fue determinar el momento de inercia de masa de un elemento de máquina con geometría compuesta. En lugar de discretizar volúmenes manualmente, se implementó un barrido volumétrico exacto utilizando funciones matemáticas y librerías de computación científica.

**Documentación:** Para ver el planteamiento matemático detallado y la validación de errores, consulta el [Reporte Técnico (PDF)](./Reporte_Tecnico_Inercia.pdf).

## 🛠️ Tecnologías y Métodos

* **Lenguaje:** Python 3.
* **Librerías Clave:**
    * `SciPy` (`dblquad`, `tplquad`): Para la resolución de integrales dobles y triples.
    * `NumPy`: Para operaciones vectoriales.
    * `Matplotlib`: Para la visualización de las regiones de integración.
* **Métodos Matemáticos:**
    * Integración Numérica (Cuadratura).
    * Cálculo de Centroides y Volúmenes.
    * Teorema de los Ejes Paralelos (Steiner).

## 📊 Resultados y Validación

El algoritmo demostró una alta precisión al comparar los resultados computacionales con los modelos teóricos tradicionales:

* **Cálculo Teórico:** $-176A^4$ $mm^4$
* **Cálculo Computacional (SciPy):** $-176.00$ $mm^4$
* **Error Relativo:** ~0.0%

Esto valida el uso de la integración numérica como una herramienta fiable para el diseño ingenieril de piezas no convencionales.

## 📂 Estructura del Repositorio

* `Calculo_Inercia_Integracion_Numerica.ipynb`: Notebook con el código fuente y las funciones de integración.
* `Reporte_Tecnico_Inercia.pdf`: Documento académico con la fundamentación física y matemática.

## 🎓 Contexto Académico

Proyecto desarrollado para la materia de **Cálculo Vectorial** en la **ESPOL (Escuela Superior Politécnica del Litoral)**.

**Grupo 7:**
* Paladines Sánchez José Luis
* Córdova Magallán Ashley Gabriela
* Tandazo Sarango Pauleth Natasha
* Tenelema Pucuna Joselyn Dayana

---
*Ingeniería aplicada mediante métodos numéricos computacionales.*
