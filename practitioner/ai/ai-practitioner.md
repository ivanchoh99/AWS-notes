Amazon tiene un framework para medir la comparación y llama TCO (total cost ownership)
___
Costos de AWS
 1. Computación
 2. Almacenamiento 
 3. Transferencia de datos **fuera** del Cloud (AWS) - Este punto puede ser relativo, ya que depende de las regiones, las AZ y como configures la comunicacion entre servicios de AWS
___
# Fundamentos de IA y Maching Learning (ML)

# Deep Learning
## CNNs - Convolutional Neural Networks
- Estructuras cuadriculadas
- capas utilizan filtos (kernels)

## RNNs - Recurrent Neural Networks
- Tiene una estructura en la que la salida de cada neurona se retroalimenta 
- Utiles para tareas en donde la longitud de entrada y salida pueden variar (Traduccion de idiomas, generación de texto)
___
# Natural language Processing (NLP)
- Interacción entre las computadoras y los humanos 
- Permite entender, interpretar y generar lenguaje humano 

- Tokenización: Dividir texto en palabras, frases u otras unidades linguisticas 
- Lematización y Steamming: Reducción de palabras a su forma base o raiz
- Modelo de lenguaje: Un modelo estadístico que predice la probabilidad de una secuencia de palabras
___
# Transformer
Son una arquitectura de modelos de IA para procesamiento del lenguaje natural, pueden procesar oraciones completas en paralelo.

Utiliza un mecanismo llamado **Self-Attention**
    1. Evalua la importancia de cada palabra en el contexto
    2. Permite dar mas importancia a ciertas palabras 
    3. Traduce oraciones mas coherentes
___
# Matriz de confusion

*"Los modelos ademas de entrenarse, probarse, deben evaluarse"* 
Herramienta para evaluar la precisión de un modelo de clasificación, divide resultados en 4 cateforias
    - Verdaderos Positivos(TP): Real=1, Predicho=1 
    - Falsos Positivos(FP): Real=0, Predicho=1
    - Verdaderos Negativos(TP): Real=0, Predicho=0
    - Falsos Negativos(FN): Real=1, Predicho=0

Precision = TP / (TP + FP)
Recall =  TP / (TP + FN) (Importante detectar todos los casos positivos)
F1 = (2 * Precision * Recall) / (Precision + Recall)
Accuracy = (TP + TN) / (TP + TN + FP + FN)

# AUC - ROC
Mide la capacidad de un modelo para distinguir entre clases en clasificación binaria

- ROC: es una curva que muestra la relación entre la tas ade verdaderos positivos y la tasa de falsos positivos 
- AUC (Area bajo la curva): es el área total debajo de la curva ROC
    AUC = 1.0
    AUC = 0.5

Esto es util para comparar diferentes modelos de clasificación para una misma tarea

# Regresion
Aprendizaje supervisado
Predice un valor numerico continuo

# Clustering
- Tecnica de aprendizaje no supervisado
- El modelo agrupa datos similares sin usar etiquetas previas
- Cada grupo se llama cluster

## K-Means
Es un algoritmo que agrupa datos similares en K grupos, buscando que los puntos de cada grupo estén lo mas ceca posible entre si

