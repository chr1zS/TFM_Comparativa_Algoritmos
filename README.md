<p align="center">
  <img src="https://www.unir.net/wp-content/uploads/2019/11/Unir_2021_logo.svg" width="150" alt="UNIR Logo"/>
</p>

<h1 align="center">Comparativa de Algoritmos de Aprendizaje Automático para la Predicción de Cáncer de Colon</h1>

<p align="center">
  Trabajo De Fin de Master de Christian SUARZE HEUVAN - UNIR (2025)
</p>

Este proyecto tiene como objetivo aplicar y comparar distintos modelos de clasificación supervisada para predecir la probabilidad de padecer **cáncer de colon** a partir del consumo diario de **carbohidratos**, **azúcares** y **alcohol**, utilizando datos del sistema NHANES. Además, se presenta un ejemplo práctico de predicción personalizada para un paciente hipotético.

---

## 1. Estructura del Repositorio

| Archivo / Carpeta | Descripción |
|-------------------|-------------|
| `Comparativa_Algoritmos_Aprendizaje_Automatico.ipynb` | Notebook principal con el flujo completo: carga de datos, limpieza, balanceo, entrenamiento de modelos, evaluación y predicción individual. |
| `dataset/` | (Opcional) Carpeta para guardar los archivos NHANES utilizados como fuente de datos. |
| `requirements.txt` | Lista de dependencias necesarias para ejecutar el proyecto. |
| `README.md` | Este archivo, con toda la información del proyecto. |

---

## 2. ¿Cómo ejecutar este proyecto?

## 2.1 Ejecución desde Google Colab

Ir al siguiente enlace o pulsado el botón "Open in Colab" (Usar Google Chrome para la ejecución):
https://colab.research.google.com/github/chr1zS/TFM_Comparativa_Algoritmos/blob/main/Comparativa_Algoritmos_Aprendizaje_Automatico.ipynb
<p align="center">
  <a href="https://colab.research.google.com/github/chr1zS/TFM_Comparativa_Algoritmos/blob/main/Comparativa_Algoritmos_Aprendizaje_Automatico.ipynb" target="_blank">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Abrir en Google Colab"/>
  </a>
</p>

Esperar a que Colab conecte con un entorno de ejecución y luego pulsar el botón "Ejecutar Todas"

## 2.2 Ejecución desde un ordenador

#### 2.2.1 Clonar el repositorio
```bash
git clone https://github.com/chr1zS/TFM_Comparativa_Algoritmos.git
cd TFM_Comparativa_Algoritmos
```

#### 2.2.2 Crear un entorno virtual
```bash
python -m venv venv
source venv/bin/activate  # En Linux/Mac
venv\Scripts\activate     # En Windows
```

#### 2.2.3 Instalar dependencias
```bash
pip install -r requirements.txt
```

#### 2.2.4 Ejecutar el Nnotebook
```bash
jupyter notebook Comparativa_Algoritmos_Aprendizaje_Automatico.ipynb
```

---

## 3. Objetivos del Proyecto

El objetivo principal de este proyecto es aplicar técnicas de aprendizaje automático para predecir la probabilidad de que un individuo padezca **cáncer de colon** a partir del consumo diario de tres variables nutricionales clave:

- **Carbohidratos** (g/día)
- **Azúcares** (g/día)
- **Alcohol** (g/día)

Se entrena una serie de modelos clasificadores utilizando un dataset derivado de NHANES, aplicando técnicas de limpieza, balanceo (SMOTE) y evaluación de métricas.

---

## 4. Modelos Utilizados

Se implementaron y compararon los siguientes algoritmos de clasificación supervisada:

- **Árbol de Decisión**
- **Random Forest**
- **Regresión Logística**
- **Red Neuronal Multicapa** (MLPClassifier)

Los modelos fueron entrenados sobre un conjunto de datos balanceado y, cuando fue necesario, estandarizado para mejorar su rendimiento.

---

## 5. Métricas de Evaluación

La evaluación de los modelos se realizó utilizando varias métricas estándar para clasificación binaria, con el objetivo de obtener una visión completa del rendimiento de cada algoritmo:

- **Accuracy**: porcentaje de aciertos globales.
- **Precision**: proporción de verdaderos positivos entre los casos predichos como positivos.
- **Recall (Sensibilidad)**: proporción de verdaderos positivos entre todos los casos realmente positivos.
- **F1-score**: media armónica entre precision y recall.
- **AUC-ROC**: área bajo la curva ROC, mide la capacidad discriminativa del modelo.

Las métricas fueron visualizadas mediante gráficos y tablas comparativas para facilitar el análisis de resultados.

---

## 6. Ejemplo de Predicción

El proyecto incluye un ejemplo de predicción personalizada para un paciente hipotético con el siguiente perfil nutricional:

- **Carbohidratos**: 200 g/día
- **Azúcares**: 90 g/día
- **Alcohol**: 10 g/día

A partir de estos datos, el modelo entrenado estima la **probabilidad de padecer cáncer de colon** y genera un diagnóstico predictivo (Sí / No).

---

## 7. Referencias Nutricionales

| Nutriente        | Recomendación diaria        | Consumo de riesgo                 |
|------------------|-----------------------------|-----------------------------------|
| **Azúcares**     | 25–50 g/día                 | > 50–60 g/día                     |
| **Carbohidratos**| 225–325 g/día               | > 350 g/día                       |
| **Alcohol (puro)** | 10–20 g/día                | > 30 g/día                        |

> Estas recomendaciones están basadas en guías de salud pública emitidas por organismos internacionales como la **OMS**, la **EFSA** y el **USDA**. Los valores pueden variar según edad, sexo y condición médica de la persona.

---

## 8. Licencia

Este proyecto se encuentra bajo licencia **GNU General Public License v3.0**  
Desarrollado por **Christian SUARZE HEUVAN**  
**Universidad Internacional de La Rioja (UNIR)** – Año: 2025

Puedes consultar el texto completo de la licencia en el archivo [`LICENSE`](./LICENSE).


