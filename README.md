# Comparativa de Algoritmos de Aprendizaje Automático para la Predicción de Cáncer de Colon

Este proyecto tiene como objetivo aplicar y comparar distintos modelos de clasificación supervisada para predecir la probabilidad de padecer **cáncer de colon** a partir del consumo diario de **carbohidratos**, **azúcares** y **alcohol**, utilizando datos del sistema NHANES. Además, se presenta un ejemplo práctico de predicción personalizada para un paciente hipotético.

---

## 📁 Estructura del Repositorio

| Archivo / Carpeta | Descripción |
|-------------------|-------------|
| `Comparativa_Algoritmos_Aprendizaje_automatico.ipynb` | Notebook principal con el flujo completo: carga de datos, limpieza, balanceo, entrenamiento de modelos, evaluación y predicción individual. |
| `dataset/` | (Opcional) Carpeta para guardar los archivos NHANES utilizados como fuente de datos. |
| `requirements.txt` | Lista de dependencias necesarias para ejecutar el proyecto. |
| `README.md` | Este archivo, con toda la información del proyecto. |

---

##  ¿Cómo ejecutar este proyecto?

### 1. Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
```

### 2. Crear un entorno virtual
```bash
python -m venv venv
source venv/bin/activate  # En Linux/Mac
venv\Scripts\activate     # En Windows
```

### 3. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 4. Ejecutar el Nnotebook
```bash
jupyter notebook Comparativa_Algoritmos_Aprendizaje_automatico.ipynb
```

---

## Objetivos del Proyecto

El objetivo principal de este proyecto es aplicar técnicas de aprendizaje automático para predecir la probabilidad de que un individuo padezca **cáncer de colon** a partir del consumo diario de tres variables nutricionales clave:

- **Carbohidratos** (g/día)
- **Azúcares** (g/día)
- **Alcohol** (g/día)

Se entrena una serie de modelos clasificadores utilizando un dataset derivado de NHANES, aplicando técnicas de limpieza, balanceo (SMOTE) y evaluación de métricas.

---

## Modelos Utilizados

Se implementaron y compararon los siguientes algoritmos de clasificación supervisada:

- **Árbol de Decisión**
- **Random Forest**
- **Regresión Logística**
- **Red Neuronal Multicapa** (MLPClassifier)

Los modelos fueron entrenados sobre un conjunto de datos balanceado y, cuando fue necesario, estandarizado para mejorar su rendimiento.

---

## Métricas de Evaluación

La evaluación de los modelos se realizó utilizando varias métricas estándar para clasificación binaria, con el objetivo de obtener una visión completa del rendimiento de cada algoritmo:

- **Accuracy**: porcentaje de aciertos globales.
- **Precision**: proporción de verdaderos positivos entre los casos predichos como positivos.
- **Recall (Sensibilidad)**: proporción de verdaderos positivos entre todos los casos realmente positivos.
- **F1-score**: media armónica entre precision y recall.
- **AUC-ROC**: área bajo la curva ROC, mide la capacidad discriminativa del modelo.

Las métricas fueron visualizadas mediante gráficos y tablas comparativas para facilitar el análisis de resultados.

---

## Ejemplo de Predicción

El proyecto incluye un ejemplo de predicción personalizada para un paciente hipotético con el siguiente perfil nutricional:

- **Carbohidratos**: 200 g/día
- **Azúcares**: 90 g/día
- **Alcohol**: 10 g/día

A partir de estos datos, el modelo entrenado estima la **probabilidad de padecer cáncer de colon** y genera un diagnóstico predictivo (Sí / No).

---

## Referencias Nutricionales

| Nutriente        | Recomendación diaria        | Consumo de riesgo                 |
|------------------|-----------------------------|-----------------------------------|
| **Azúcares**     | 25–50 g/día                 | > 50–60 g/día                     |
| **Carbohidratos**| 225–325 g/día               | > 350 g/día                       |
| **Alcohol (puro)** | 10–20 g/día                | > 30 g/día                        |

> Estas recomendaciones están basadas en guías de salud pública emitidas por organismos internacionales como la **OMS**, la **EFSA** y el **USDA**. Los valores pueden variar según edad, sexo y condición médica de la persona.

---

## Licencia

Proyecto desarrollado por **Christian SUARZE HEUVAN**  
**Universidad Internacional de La Rioja (UNIR)**  
**Año: 2025**

Este proyecto puede utilizarse para fines académicos, educativos y de investigación.  
No se autoriza su uso con fines comerciales sin autorización expresa.

