# M.R.AI
Prediction of Alzheimer's desease using image recognition
# Detección y Clasificación de Alzheimer mediante Neuroimagen (MRI) e Inteligencia Artificial

## Marco Académico e Institucional

**Proyecto de Clasificación de Imágenes MRI para Detección de Alzheimer**

* **Institución:** Universidad Francisco de Vitoria (UFV)
* **Asignatura:** Procesamiento de Imágenes Biomédicas con Inteligencia Artificial
* **Profesor:** Alberto de Santos
* **Contexto:** Ingeniería Biomédica
* **Curso/Fecha:** [Incluir el curso académico o la fecha de finalización]
* **URL del Repositorio:** [https://github.com/RAvila-bioeng/M.R.AI]

---

## Objetivo del Proyecto

El objetivo principal de este proyecto es desarrollar un modelo de **Deep Learning** robusto y, fundamentalmente, **interpretable** para la clasificación automatizada de imágenes de Resonancia Magnética (MRI) cerebral, con el fin de distinguir entre sujetos sanos (Normal Control, NC) y pacientes con diferentes estadios de la Enfermedad de Alzheimer (AD, MCI).

### Objetivos Específicos

1.  **Corto Plazo:** Implementar un *pipeline* completo de preprocesamiento de neuroimágenes (registro, normalización, etc.) y entrenar una Red Neuronal Convolucional (CNN) base.
2.  **Medio Plazo:** Optimizar la arquitectura del modelo (ej. 3D CNN, Transfer Learning) y lograr métricas de desempeño que superen los *benchmarks* académicos (ej. Accuracy > 88%).
3.  **Largo Plazo:** Integrar técnicas de **Explicabilidad (XAI)** como Grad-CAM, LIME o SHAP para justificar la clasificación y visualizar las regiones cerebrales de mayor relevancia diagnóstica.

---

## Descripción del Problema

La **Enfermedad de Alzheimer (EA)** es la causa más común de demencia, caracterizada por un deterioro cognitivo progresivo. El diagnóstico temprano es crucial para la gestión clínica y el inicio de tratamientos. Este proyecto aborda el desafío de la detección temprana y la clasificación mediante el análisis de neuroimágenes estructurales (MRI), que pueden mostrar atrofia cerebral, especialmente en el hipocampo y la corteza.

**Relevancia Clínica:** Un sistema de soporte a la decisión basado en IA puede ayudar a los radiólogos y neurólogos a mejorar la **objetividad** y **eficiencia** del diagnóstico, minimizando la variabilidad inter-observador.

---

## Stack Tecnológico

| Categoría | Herramientas/Librerías | Propósito |
| :--- | :--- | :--- |
| **Deep Learning** | TensorFlow, Keras, PyTorch | Desarrollo y entrenamiento de modelos CNN. |
| **Neuroimagen** | nibabel, SimpleITK | Lectura, escritura y manipulación de archivos MRI (NIfTI). |
| **Explicabilidad (XAI)** | LIME, SHAP, Grad-CAM | Interpretabilidad del modelo para justificar decisiones. |
| **Ciencia de Datos** | NumPy, Pandas, Scikit-learn | Preprocesamiento de datos, métricas y validación. |
| **Entorno** | Python 3.11, Conda/Pip | Gestión de dependencias. |

---

## Metodología Científica (Pipeline CRISP-DM)

El desarrollo del proyecto sigue un enfoque científico y reproducible:

1.  **Entendimiento del Negocio/Clínica:** Definición del problema del Alzheimer, selección de biomarcadores y métricas clínicamente relevantes.
2.  **Entendimiento de los Datos:** Exploración del *Dataset* (ej. ADNI, OASIS, o Kaggle). Análisis de la calidad de la imagen, distribución de clases y formato.
3.  **Preparación de Datos:**
    * Preprocesamiento: Conversión de formato, **registro** y **normalización** a un *template* estándar (ej. MNI).
    * Aumento de Datos (*Data Augmentation*) para mejorar la robustez del modelo.
4.  **Modelado:** Diseño e implementación de la arquitectura de Deep Learning (ej. Red 3D CNN adaptada).
5.  **Evaluación:** Validación rigurosa con métricas específicas y **Validación Cruzada** (*Cross-Validation*).
6.  **Despliegue/Comunicación:** Documentación, repositorio GitHub y demostración del modelo y sus explicaciones.

---

## Métricas de Evaluación Clínica

La evaluación no se limita a la precisión (*Accuracy*), sino que se centra en el **rigor diagnóstico** y las implicaciones clínicas:

* **Accuracy:** [Objetivo: 88-95%] - Proporción de predicciones correctas.
* **Sensibilidad (Recall):** [Objetivo: > 85%] - Capacidad de identificar correctamente a los pacientes enfermos (evitar Falsos Negativos). **Crucial para el *screening* temprano.**
* **Especificidad:** [Objetivo: > 90%] - Capacidad de identificar correctamente a los sujetos sanos (evitar Falsos Positivos).
* **AUC (Area Under the Curve):** [Objetivo: > 0.92] - Medida de discriminación entre las clases.

---

## Interpretabilidad y Explicabilidad (XAI)

Dada la aplicación médica, la interpretabilidad es fundamental. Se implementarán las siguientes técnicas:

* **Grad-CAM:** Generación de **Mapas de Activación** superpuestos en las imágenes MRI originales, destacando las regiones cerebrales (ej. hipocampo) que el modelo consideró más relevantes para la clasificación.
* **LIME (Local Interpretable Model-agnostic Explanations):** Proporcionar explicaciones para predicciones individuales (locales).
* **SHAP (SHapley Additive exPlanations):** Análisis de la contribución de diferentes características o regiones a la decisión final.

---

## Instalación y Uso

### 1. Clonar el Repositorio

```bash
git clone [https://dle.rae.es/repositorio](https://dle.rae.es/repositorio)
cd M.R.AI
