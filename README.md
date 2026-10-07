# ⭐👁️‍🗨️Clasificación de Imágenes con Redes Neuronales y CIFAR-10🧠🤖

<p align="center">
  <img src="https://img.shields.io/badge/Estado-Completado-success?style=for-the-badge&logo=none" />
  <img src="https://img.shields.io/badge/Mantenimiento-Activo-blue?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Versión-1.0.0-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Licencia-MIT-purple?style=for-the-badge&logo=open-source-initiative&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-326690?style=for-the-badge&logo=python&logoColor=white" />
</p>

⭐ *Este es mi repositorio oficial de una implementación práctica en Python utilizando **TensorFlow** y **Keras**. En este proyecto, entrené un modelo de aprendizaje automático enfocado en la clasificación de imágenes del popular conjunto de datos **CIFAR-10**.* 🎯

---

## 📌 1. Sobre el Proyecto

He abordado un problema clásico dentro del campo de la **Visión por Computador (Computer Vision)** y el **Aprendizaje Profundo (Deep Learning)**: la clasificación multiclase de imágenes a color de baja resolución (32x32 píxeles). 

### 📦 El Conjunto de Datos (CIFAR-10)
Para este desarrollo, utilicé el dataset integrado `cifar10` de Keras, el cual se compone de:
* 🏋️ **50,000 imágenes de entrenamiento** a color (32x32 píxeles).
* 🧪 **10,000 imágenes de prueba / verificación**.
* 🏷️ **10 clases mutuamente excluyentes**:
  1. ✈️ `airplane` (Avión)
  2. 🚗 `automobile` (Automóvil)
  3. 🐦 `bird` (Pájaro)
  4. 🐱 `cat` (Gato)
  5. 🦌 `deer` (Ciervo)
  6. 🐶 `dog` (Perro)
  7. 🐸 `frog` (Rana)
  8. 🐴 `horse` (Caballo)
  9. 🚢 `ship` (Barco)
  10. 🚚 `truck` (Camión)

---

## 🛠️ 2. Tecnologías y Librerías Utilizadas

Desarrollé el script en un entorno de **Google Colab**, haciendo uso de las siguientes herramientas del ecosistema de ciencia de datos:
* 🧠 **TensorFlow / Keras:** Framework principal para la carga de datos y construcción de las redes neuronales.
* 🔢 **NumPy:** Manipulación eficiente de arreglos numéricos y matrices multidimensionales.
* 📊 **Pandas:** Gestión y análisis de estructuras tabulares.
* 📈 **Matplotlib:** Visualización gráfica de los datos y despliegue de las miniaturas de las imágenes del dataset.
* 🖼️ **PIL (Pillow):** Procesamiento y manipulación avanzada de imágenes.

---

## 📋 3. Flujo de Trabajo que Implementé

1. **📥 Importación de librerías:** Carga de los módulos esenciales de TensorFlow, Keras, NumPy, Pandas y Matplotlib.
2. **📂 Carga de datos:** Descarga automática y división del dataset CIFAR-10 en conjuntos de entrenamiento y verificación (`imagenes_entrenamiento`, `etiquetas_entrenamiento`, `imagenes_verificacion`, `etiquetas_verificacion`).
3. **🔍 Exploración inicial:** Inspección de las dimensiones de los tensores (por ejemplo, `(50000, 32, 32, 3)` para las imágenes de entrenamiento)
4. **⚡ Preprocesamiento y Normalización:** Escalado de los valores de los píxeles dividiendo entre `255.0` para acotar los datos en un rango flotante de `0` a `1`, optimizando así el rendimiento del entrenamiento del modelo.
5. **🏷️ Mapeo de Clases:** Definición de las etiquetas textuales correspondientes a los índices numéricos de las clases (del `0` al `9`).
6. **📉 Visualización:** Implementación de una función auxiliar (`mostrar()`) basada en `matplotlib` para graficar una cuadrícula con las primeras imágenes del entrenamiento y sus respectivas etiquetas.
