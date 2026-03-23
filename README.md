# pytorch-generative-and-classification
Este repositorio contiene una colección de proyectos prácticos enfocados en la implementación de arquitecturas de Deep Learning utilizando **PyTorch**. Los proyectos abarcan desde la clasificación de imágenes tradicionales hasta modelos generativos avanzados no supervisados.

## Proyectos Incluidos
### 1. Image Classification with Linear Neural Networks (CIFAR-10)
**Archivo:** [`Clasificación_CIFAR_10.ipynb`](./Clasificación_CIFAR_10.ipynb)  
Implementación de un modelo base (*baseline*) de clasificación de imágenes desde cero. El modelo utiliza transformaciones lineales para clasificar el dataset CIFAR-10 y está optimizado para ejecución dinámica en CPU y GPU (CUDA).

### 2. Hierarchical Image Classification (CIFAR-100)
**Archivo:** [`Clasificación_Jerárquica_CIFAR_100.ipynb`](./Clasificación_Jerárquica_CIFAR_100.ipynb)  
Exploración de cómo la información jerárquica mejora el rendimiento en Deep Learning. Implementa el teorema de la probabilidad condicionada para aprovechar la estructura de 20 superclases (etiquetado grueso) y refinar la predicción de las 100 clases finas del dataset.

### 3. Dimensionality Reduction and Feature Extraction
**Archivo:** [`Autoencoder_Clásico.ipynb`](./Autoencoder_Clásico.ipynb)  
Implementación de un modelo de aprendizaje no supervisado mediante un Autoencoder profundo. Diseñado para comprimir datos en un espacio latente de menor dimensionalidad y reconstruirlos, extrayendo las características más importantes sin necesidad de etiquetas.

### 4. Generative AI: Variational Autoencoder (VAE)
**Archivo:** [`Variational_Autoencoder_VAE.ipynb`](./Variational_Autoencoder_VAE.ipynb)  
Introducción a los modelos generativos profundos. A diferencia de un autoencoder tradicional, este VAE modela el espacio latente mediante distribuciones gaussianas ($\mu, \sigma^2$), permitiendo un muestreo continuo para la generación de datos sintéticos de alta fidelidad.

## Tecnologías y Herramientas
* **Lenguaje:** Python 3
* **Framework Principal:** PyTorch (`torch.nn`, `torch.optim`, CUDA)
* **Visión Artificial:** Torchvision (Datasets, Transforms)
* **Análisis y Visualización:** Matplotlib, NumPy, Scikit-learn, TQDM

## Cómo ejecutar los cuadernos
Puedes visualizar estos proyectos directamente aquí en GitHub. Para ejecutarlos e interactuar con el código, la opción más rápida es abrir los archivos `.ipynb` en [Google Colab](https://colab.research.google.com/).

Si deseas ejecutarlos en un entorno local, asegúrate de instalar las dependencias necesarias:
```bash
pip install torch torchvision matplotlib numpy scikit-learn tqdm
