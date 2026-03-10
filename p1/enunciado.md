A partir del siguiente enunciado tenenmos que hacer lo siguiente:
Aquí tienes el contenido del documento convertido a formato Markdown:

Técnicas de Aprendizaje Automático 2026 - UCLM 

## Prueba de progreso 1: Predicción de la Calidad del Vino. 

Clasificación vs regresión 

Usando un conjunto de datos con diversas características de vinos, predice la calidad de estos usando un algoritmo de regresión y otro de clasificación y compara el desempeño de ambos. Para cada tarea, tendrás que seleccionar y usar un algoritmo, analizar su desempeño y extraer conclusiones. Se recomienda probar diferentes algoritmos y parámetros; todas las pruebas deben reflejarse en el cuaderno de Jupyter.

Datos 

Debe usarse el conjunto de datos sobre la calidad del vino que contiene propiedades químicas y una puntuación de calidad.

**Instalación y carga:** 

```python
pip install ucimlrepo

from ucimlrepo import fetch_ucirepo

# Descarga del dataset
wine_quality = fetch_ucirepo(id=186)

# Datos brutos en formato Dataframe de pandas
X = wine_quality.data.features
y = wine_quality.data.targets

# Metadatos e información
print(wine_quality.metadata)
print(wine_quality.variables)

```

Descripción de variables 

| Nombre de Variable | Función | Tipo | ¿Faltan valores? |
| --- | --- | --- | --- |
| `fixed_acidity` | Característica | Continua | No |
| `volatile_acidity` | Característica | Continua | No |
| `citric_acid` | Característica | Continua | No |
| `residual_sugar` | Característica | Continua | No |
| `chlorides` | Característica | Continua | No |
| `free sulfur dioxide` | Característica | Continua | No |
| `total_sulfur_dioxide` | Característica | Continua | No |
| `density` | Característica | Continua | No |
| `pH` | Característica | Continua | No |
| `sulphates` | Característica | Continua | No |
| `alcohol` | Característica | Continua | No |
| `quality` | Objetivo | Categórica | No |

---

Normas y estructura 

* La tarea es **individual**.


* Se recomienda alojar el código en un repositorio git (GitHub, GitLab, etc.).


* El envío será uno o varios cuadernos de Jupyter (.ipynb) bien documentados.



Procedimiento 

1. 
**Elección de algoritmo:** Selecciona y justifica un algoritmo de **regresión** (variable continua) y uno de **clasificación** (variable categórica).


2. **Evaluación de los modelos:**
* 
**Regresión:** Usa métricas como MAE, MSE o $R^2$.


* 
**Clasificación:** Usa al menos una técnica como matriz de confusión, ROC o F1-score.




3. 
**Comparación:** Incluye una sección final comparando ambos desempeños y reflexionando sobre cuál funciona mejor y por qué.



Evaluación y Envío 

* 
**Valoración:** 7,5% (prueba de progreso) + 8% (prácticas) = 15,5% del total de la asignatura.


* 
**Fecha límite:** 11 de marzo de 2025 a las 23:59.

# Datos importantes

tengo que hacer una prueba de progreso sobre predicción de la calidad del vino usando técnicas de aprendizaje automático. Debo seleccionar un algoritmo de regresión y otro de clasificación, evaluar su desempeño con métricas adecuadas y comparar los resultados. El conjunto de datos contiene características químicas del vino y una puntuación de calidad, sin valores faltantes. La tarea es individual y se recomienda usar un repositorio git para alojar el código, que debe ser enviado en formato Jupyter Notebook antes del 11 de marzo de 2025 a las 23:59.

He pensado elegir esots algorimot Random Forest, decision tree y Naive Bayes el de  para clasificación y regresión, respectivamente.
Debes elegir el mejor de los tres de cada algoritmo para cada tarea y justificar tu elección. Luego, evalúa el desempeño de cada modelo utilizando las métricas mencionadas (MAE, MSE, R^2 para regresión y matriz de confusión, ROC, F1-score para clasificación) y finalmente compara los resultados para determinar cuál modelo funciona mejor en este caso específico.
Una vez que hayas realizado estas tareas, asegúrate de documentar todo el proceso en un cuaderno de Jupyter, explicando cada paso y las decisiones tomadas. Esto no solo ayudará a entender tu enfoque, sino que también facilitará la evaluación de tu trabajo.
Una vez que haya elegido el mejor algoritmo para clasificacion y regresion debes de compara ambos y decir cual es el mejor resultados te de y porque crees que es mejor en este caso específico. Recuerda que la comparación debe basarse en las métricas de evaluación y en la naturaleza de los datos y el problema que estás abordando.

# Datos del autor
**Nombre:** Daniel Tomas Gallego
**Asignatura:** Tecnicas de Aprendizaje Automático
**Curso:** 2026
**Universidad:** UCLM 