La IA generativa es un campo de IA que crea contenido nuevo como conversaciones, imagenes, videos y musica.
Se enfoca en aprender y palicar conocimientos en una amplia gama de areas 
Utiliza datos para resolver problemas nuevos nunca antes vistos

# Modelos fundacionales (FM)

Son grandes modelos de IA entrenados con grandes cantidades de datos para comprender y generar información
- BERT(Google)
- GPT(OpenIA) 
- Claude (Anthropic)
- DALL-E (OpenAI)
- LLaMa (Meta)

# Large Language Model (LLM)
Los modelos de lenguaje generativos son *no deterministas* el mismo prompt puede generar un resultado diferente

# Transformer
Introduce la arquitectura Transformer basada unicamente únicamente en mecanismos de atención
Sienta las bases de los modelos de  lenguajes modernos
Paper "Attention is all you need(2017)"

Reemplaza a las redes recurrentes 
Procesa palabras en paralelo, no de manera secuencial
Usa atención para encontrar qué partes del texto son relevantes
Base de todos los modelos modernos: GPT, BERT, T5, LLaMa, Phi, etc

Los transformers entienden relaciones entre palabras sin procesarlas una por una

## ¿Como funciona?
*Codificación posicional sobre texto*

1. Se crea un vector numerico único para cada posicion
2. Usa funciones de seno y coseno
3. Se suma al embedding

### Atención (Self Atenttion)

El modelo decide que palabras son relevantes para entender otra palabra

$$ \text{Atención}(Q, K, V) = \text{softmax}\left( \frac{QK^T}{\sqrt{d_k}} \right) V $$

Cada token se convierte en 
    - Q(Query)
    - K (Key)
    - V (Value)
Se calcula la relevancia entre Q y todas las K
Se combinan los valores V con sus pesos

#### Codificador 
Procesa la secuencia de entrada y crea una representación que capture el contexto de cada token
#### Descodificador 
Genera la secuencia de salida prestando atención a la representación del codificador y prediciendo el siguiente token

Los Transformers son esenciales para GenAI
- Permiten comprender contex complejo
- Generar texto coherente y contextualizado
- Escalan a miles de millones de parámetros
- Soportan múltiples modalidadesL texto, imagenes, video, audio
- Son la base de Azure, OpenAI, ChatGPT, Gemini, Claude, LLaMA

# Inferencia en el borde
Realizar cálculos y predicciones directamente en dispositivos cercanos a donde se generan los datos, no depende de un servidor en la nube

Small Language Models (SLM) en el dispositivo de borde
    - Puede funcionar sin conexion a Internet
    - Debido a su tamaño pequeño, tiene baja latencia
    - Puedde hacer predicciones rapidamente
Large Language Models (LLM) en un servidor remoto
    - Las predicciones tardan mas en llegar al dispositivo (mayor latencia)
    - Requieren una conexión a Internet para se accesibles

# Generative Adversarial Networks (GANs)

Redes generativas antagonicas: es un tipo de modelo de inteligencia artificial que pertenece al campo de la IA generativa

Redes diseñadas para generar nuevos datos
Posee 2 redes neuronales, generador y el discriminador

*Generador:* Crea datos falsos a partir de ruido aleatorio, con el objetivo de engañar al discriminador para que los clasifique como reales

*Discriminador:* Evalua tanto los datos reales como los generado, aprendiendo a distinguir entre ellos. Su objetivo es detectar cuándo los datos son falsos

# Modelo de difusion
Son un tipo de modelo generativo que ha demostrado dser muy eficaz para generar contenido de alta calidad (especialmente imagenes)

Se basan en un proceso que simula la forma en que las particulas se dispersan en un espacion
- Proceso de difusion directa: Convierte la imagen en ruido (Entrenar modelso)

- Proceso de difusion inversa: Convierte el ruido en imagen

# Modelos multimodales
Capacidad par acombinar informasción de doversas modalidades(texto, imagenes, audio, video y mas) para generar salidas mas competas y contextuales 

# Hiperparametros
Controlan el comportamiento del modelo durante el entrenamiento
Los hiperparametros son configuraciones externas al modelo
El ajuste de hiperparametros mejora la precision y eficiencia del modelo

Ajuste de hiperparámetros (implica probar diferentes combinaciones de estos valores para mejorar el modelo) permite optimizar el rendimiento del modelo de machine learning

Hiperparametros:
- Taza de aprendizaje
- Tamaño del lote
- Nomero de épocas 