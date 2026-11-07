
# Detección y Clasificación de Neumonía en Radiografías de Tórax mediante CNNs

**Asignatura:** Procesamiento de Imágenes Digitales (PID)  
**Institución:** Universidad de Sevilla  
**Curso Académico:** 2024 / 2025

---

## 👥 Miembros del Equipo

- **Daniel Álvarez Corcho**
- **Diego Rodríguez Sandru**
- **Álvaro Castro Sanleandro**

---

## 📄 Descripción del Proyecto

La neumonía es una infección respiratoria caracterizada por la inflamación de los sacos alveolares y la acumulación de fluidos en los pulmones. Las radiografías de tórax (CXR) son la prueba diagnóstica principal por su bajo coste y accesibilidad, aunque su interpretación manual presenta variabilidad interobservador y requiere experiencia radiológica.

El objetivo de este proyecto es diseñar, implementar y evaluar un sistema automatizado para la **detección y clasificación binaria de neumonía** (*neumonía* vs. *no-neumonía*) mediante **técnicas de Procesamiento Digital de Imágenes (PDI)** y **Redes Neuronales Convolucionales (CNN)**.

El desarrollo se plantea con un enfoque didáctico progresivo distribuido en **8 bloques metodológicos** y una dedicación de 50 horas por integrante (150 horas totales).

---

## 📊 Dataset

Se utiliza el conjunto de datos [**Neumonía X-Rays Dataset (Kaggle)**](https://www.kaggle.com/datasets/gonzajl/neumona-x-rays-dataset):

- **Total de imágenes:** 10.498 radiografías de tórax.
- **Clases:** Neumonía / No-neumonía (Normal).
- **Formato:** Imágenes en blanco y negro / escala de grises acompañadas de un archivo `.csv` con las etiquetas diagnósticas y las rutas de los archivos.

---

## 🛠️ Estructura del Trabajo (8 Bloques)

1. **Bloque 1: Fundamentación Teórica y Estado del Arte:** Estudio bibliográfico de modelos convolucionales aplicados a radiología torácica.

2. **Bloque 2: CNN Propia Base:** Diseño e implementación de un modelo *baseline* propio procesando imágenes en escala de grises redimensionadas a (224, 224).

3. **Bloque 3: Preprocesamiento y Data Augmentation:** Aplicación de transformaciones geométricas (rotaciones, giros, escalado) para mejorar la generalización del modelo.

4. **Bloque 4: Regularización y Optimización:** Integración de capas de *Dropout*, *Batch Normalization* y ajuste de hiperparámetros (*tuning*).

5. **Bloque 5: Modelo de la Literatura:** Implementación y evaluación de una arquitectura publicada en la literatura científica de referencia.

6. **Bloque 6: Transfer Learning y Fine-Tuning:** Evaluación opcional de arquitecturas complejas preentrenadas (p. ej., VGG16, ResNet50) sobre ImageNet.

7. **Bloque 7: Protocolo de Evaluación Comparativa:** Evaluación transversal comparando Matrices de Confusión, Exactitud (*Accuracy*), Sensibilidad (*Recall*), Precisión, F1-score y curvas ROC-AUC.

8. **Bloque 8: Memoria Final y Autoevaluación:** Redacción de la memoria autocontenida en LaTeX y consolidación de la hoja de tiempos.

---

## 📁 Estructura del Repositorio

```text
.
├── README.md                         # Presentación e instrucciones del repositorio
├── .gitignore                        # Archivos excluidos de control de versiones
├── memoria/                          # Código fuente de la memoria en LaTeX
│   ├── main.tex                      # Fichero principal de la memoria
│   ├── referencias.bib               # Archivo BibTeX de referencias bibliográficas
│   └── figuras/                      # Gráficas, diagramas y capturas
└── notebooks/                        # Cuadernos Jupyter ordenados por bloques
    ├── 01_eda_y_preprocesado.ipynb
    ├── 02_cnn_propia_base.ipynb
    ├── 03_data_augmentation.ipynb
    ├── 04_regularizacion_y_tuning.ipynb
    ├── 05_modelo_literatura.ipynb
    ├── 06_transfer_learning.ipynb
    └── 07_evaluacion_comparativa.ipynb
```
