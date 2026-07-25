# Ficha de análisis

## 1. Nombre del Space

* **Nombre:** lmz/candle-yolo
* **Enlace:** [https://huggingface.co/spaces/lmz/candle-yolo](https://huggingface.co/spaces/lmz/candle-yolo)
------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

El agente detecta y localiza objetos y personas dentro de una imagen mostrando los resultados mediante cuadros alrededor del obejto o persona y un numero que indica que tan confiable es la deteccion.

------------------------------------------------------------------------

## 3. Análisis PEAS

| Elemento | Pregunta | Respuesta |
| :--- | :--- | :--- |
| **Performance** | *¿Qué significa que el agente haga bien su trabajo?* | Que detecte y localice correctamente los objetos o personas, asignando una etiqueta precisa y un nivel de confianza certero. |
| **Environment** | *¿Con qué interactúa el agente?* | Entorno digital basado en imágenes estáticas cargadas por el usuario. |
| **Actuators** | *¿Qué acciones produce?* | Genera una versión visual de la imagen resaltando los objetos detectados mediante recuadros, con su etiqueta de categoría y porcentaje de confiabilidad. |
| **Sensors** | *¿Qué información recibe como entrada?* | Recibe una imagen digital (matriz de píxeles) enviada por el usuario para su análisis. |

------------------------------------------------------------------------

## 4. Clasificación del entorno

| Propiedad | Clasificación | Justificación |
| :--- | :--- | :--- |
| **Observable** | Total | El agente recibe la entrada completa (la totalidad de los píxeles de la imagen) en un solo instante. |
| **Determinista** | No | La detección puede variar según la calidad de la imagen, los umbrales de confianza configurados o la naturaleza del modelo de inferencia. |
| **Episódico** | Sí | Cada imagen se procesa de manera independiente; el análisis actual no depende ni afecta los análisis previos. |
| **Estático** | Sí | La imagen no cambia ni evoluciona mientras el agente la está procesando. |
| **Discreto** | No | La imagen contiene información continua (valores de color, coordenadas relativas, posiciones de píxeles). |
| **Conocido** | Sí | Las reglas del entorno y la interpretación de los datos están definidas por un modelo matemático previamente entrenado. |

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Seleccione la opción que consideren más adecuada y explique por qué.

-   Agente de reflejo simple
-   Agente basado en modelo
-   Agente basado en objetivos
-   Agente basado en utilidad
-   Agente con aprendizaje

> **Importante:** No existe una única respuesta correcta. Lo importante
> es justificar la elección a partir del comportamiento observado.

### Selección:
* [x] **Agente con aprendizaje**

### Justificación:
Agente con aprendizaje ya que utiliza un modelo de IA previamente entrenado para reconocer los objetos de las imagenes y se puede seguir aprendiendo para mejorar su precision o reconocer nuevos tipos de objetos.

------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**
2.  **Parcialmente observable, estocástico y secuencial.**

Justifique su respuesta.
