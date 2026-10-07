# 👁️‍🗨️ Clasificación de Imágenes con Redes Neuronales y CIFAR-10 🧠🤖

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
</p>

Este repositorio contiene una implementación práctica en Python utilizando **TensorFlow** y **Keras** para entrenar un modelo de aprendizaje automático enfocado en la clasificación de imágenes del popular conjunto de datos **CIFAR-10**. 🎯

---

## 📌 1. Descripción Temática del Proyecto

El proyecto aborda un problema clásico dentro del campo de la **Visión por Computador (Computer Vision)** y el **Aprendizaje Profundo (Deep Learning)**: la clasificación multiclase de imágenes a color de baja resolución (32x32 píxeles). 

### 📦 El Conjunto de Datos (CIFAR-10)
Se emplea el dataset integrado `cifar10` de Keras, el cual se compone de:
* 🏋️ **50,000 imágenes de entrenamiento** a color (32x32 píxeles).
* 🧪 **10,000 imágenes de prueba / verificación**[cite: 2].
* 🏷️ **10 clases mutuamente excluyentes**[cite: 2]:
  1. ✈️ `airplane` (Avión)[cite: 2]
  2. 🚗 `automobile` (Automóvil)[cite: 2]
  3. 🐦 `bird` (Pájaro)[cite: 2]
  4. 🐱 `cat` (Gato)[cite: 2]
  5. 🦌 `deer` (Ciervo)[cite: 2]
  6. 🐶 `dog` (Perro)[cite: 2]
  7. 🐸 `frog` (Rana)[cite: 2]
  8. 🐴 `horse` (Caballo)[cite: 2]
  9. 🚢 `ship` (Barco)[cite: 2]
  10. 🚚 `truck` (Camión)[cite: 2]

---

## 🛠️ 2. Tecnologías y Librerías Utilizadas

El script está diseñado para ejecutarse en un entorno de **Google Colab**, haciendo uso de las siguientes herramientas del ecosistema de ciencia de datos:
* 🧠 **TensorFlow / Keras:** Framework principal para la carga de datos y construcción de las redes neuronales.
* 🔢 **NumPy:** Manipulación eficiente de arreglos numéricos y matrices multidimensionales.
* 📊 **Pandas:** Gestión y análisis de estructuras tabulares.
* 📈 **Matplotlib:** Visualización gráfica de los datos y despliegue de las miniaturas de las imágenes del dataset[cite: 2].
* 🖼️ **PIL (Pillow):** Procesamiento y manipulación avanzada de imágenes.

---

## 📋 3. Flujo de Trabajo del Código

1. **📥 Importación de librerías:** Carga de los módulos esenciales de TensorFlow, Keras, NumPy, Pandas y Matplotlib[cite: 2].
2. **📂 Carga de datos:** Descarga automática y división del dataset CIFAR-10 en conjuntos de entrenamiento y verificación (`imagenes_entrenamiento`, `etiquetas_entrenamiento`, `imagenes_verificacion`, `etiquetas_verificacion`)[cite: 2].
3. **🔍 Exploración inicial:** Inspección de las dimensiones de los tensores (por ejemplo, `(50000, 32, 32, 3)` para las imágenes de entrenamiento)[cite: 2].
4. **⚡ Preprocesamiento y Normalización:** Escalado de los valores de los píxeles dividiendo entre `255.0` para acotar los datos en un rango flotante de `0` a `1`, optimizando así el entrenamiento del modelo[cite: 2].
5. **🏷️ Mapeo de Clases:** Definición de las etiquetas textuales correspondientes a los índices numéricos de las clases (del `0` al `9`)[cite: 2].
6. **📉 Visualización:** Implementación de una función auxiliar (`mostrar()`) basada en `matplotlib` para graficar una cuadrícula con las primeras imágenes del entrenamiento y sus respectivas etiquetas[cite: 2].

---

## 🚀 4. Cómo Ejecutar el Proyecto

1. Clona este repositorio o descarga directamente el archivo del notebook (`.ipynb`).
2. Sube el archivo a [Google Colab](https://colab.research.google.com/) o ábrelo en tu entorno local de Jupyter Notebook con soporte para TensorFlow.
3. Ejecuta las celdas de forma secuencial para reproducir la descarga, normalización y visualización del conjunto de datos.

---
⭐ *¡No olvides darle una estrella ⭐ al repositorio si te ha resultado útil!*
