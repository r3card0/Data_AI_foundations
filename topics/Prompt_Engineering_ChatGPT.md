# ChatGPT
Es una modelo de inteligencia artificial que genera lenguaje estructurado.

- [ ] [Como escribir prompts en ChatGPT](https://github.com/r3card0/Data_AI_foundations/blob/main/topics/Prompt_Engineering_ChatGPT.md#como-escribir-prompts-en-chatgpt)
- [ ] [Técnicas básicas de prompt engineering](https://github.com/r3card0/Data_AI_foundations/blob/main/topics/Prompt_Engineering_ChatGPT.md#t%C3%A9cnicas-b%C3%A1sicas-de-prompt-engineering)
- [ ] [Técnicas avanzadas de prompt engineering](https://github.com/r3card0/Data_AI_foundations/blob/main/topics/Prompt_Engineering_ChatGPT.md#t%C3%A9cnicas-avanzadas-de-prompt-engineering)
- [ ] [Casos de uso]()

# Como escribir prompts en ChatGPT
Un prompt es una pregunta que se le hace a ChatGPT. Es recomendable considerar la fecha del tema porque los modelos pueden tener información actuializada haste la fecha considerada. Por ejemplo, ChatGPT, en su lanzamiento, tuvo información hasta septiembre del 2021.

## Estructura de un prompt
Un prompt tiene los siguientes puntos que le dan estructura y son: *instrucción, contexto, inputs y outputs*. Cabe señalar, que no es necesario que los 4 puntos están inlcuidos en un prompt.

#### Instrucción
Se trata de la tarea o instrucción a resolver. Es la tarea solicitada al modelo (ChatGPT). Esta solicitud, puede ser una pregunta simple o compleja. 

Ejemplo:
```
¿qué es una base de datos relacional?
```


#### Contexto
Es información adicional que se le proporciona al modelo para mejorar su respuesta. 

Ejemplo:
```
ahora, explica a un niño de 8 años, que es una base de datos relacional con ejemplos que el entienda
```

#### Inputs
Es información adicional que se le proporciona al modelo para que realice comparaciones y mejorar su respuesta. Esto se da cuando se le proporciona un ejemplo al modelo para que a partir de este mejore su respuesta. Se porporciona mas detalle.

Ejemplo:
```
explicale al niño, la diferencia entre la base de datos relacional y las tablas de un archivo excel
```


```
explicalo nuevamente cambiando la palabra carpeta por caja de carton, porque el niño no usa carpetas
```

#### Outputs
Se refiere cuando se le solicita al modelo, que la respuesta la de en una estructura deseada, como por ejemplo que de una tabla de comparación, o que proporcione divisiones por categoria a través de bullets numéricos o no numéricos. Este es opcional y se da cuando se brinda mas detalle al modelo para que mejore su respuesta.

```
nuevamente, explicale la diferencia entre ambas tecnologias pero ahora con una historia de piratas donde se enfrenten a dinosarios y tiburones que tienen piernas de humano y pueden respirar tanto en la superficie como en el mar
```

[ver conversacion 🗺](https://chat.openai.com/share/1f4a1d79-c8eb-4174-bfe2-ad525e2aa9b4)


# Técnicas básicas de prompt engineering
* Zero-shot y One-shot Prompting
* Chain-of-Thought Prompting
* Optimizar resultados con estructuras de texto específicas
* Mejorar resultados iterando


El propósito de usar *Chain-of-thought* con LLM como ChatGPT, es generar texto estructurado y coherente a partir de una línea de pensamiento como ejemplo

La principal ventaja del *zero-shot* prompting es que no requiere datos de entrenamiento adicionales

La *iteración* en prompt engineering es una técnica para orientar al modelo a dar mejores respuestas con base al feedback de sus respuestas anteriores

La principal diferencia entre *few-shot* prompting y *one-prompting* es que *few-shot* prompting puede obtener una precisión mayor con unos cuantos ejemplos de entrenamiento. *One-shot* prompting puede ser menos preciso debido a que utiliza solo un ejemplo de entramiento.

# Técnicas avanzadas de prompt engineering
* Role play
* knowledge Generation / Knowledge Integration
* Hiper parámetros de ChatGPT

## Role play
## Knowledge Generation / Knowledge Integration
Son técnicas usadas para mejorar los modelos de lenguaje y que incluye la capacidad de generar y/o incorporar conocimiento o información para ayudar al modelo a generar respuestas mucho mas precisas.

### Knowledge Generation
¿Que me puedes decir del concepto de Knowledge Generation aplicado en prompts?

🤖 ¡Hola! En el contexto de la inteligencia artificial y los modelos de lenguaje como GPT-3.5, el concepto de "Knowledge Generation" (Generación de Conocimiento) *se refiere a la capacidad del modelo para generar información nueva y relevante en función de los datos y el contexto proporcionados en el prompt.*

🤖 Cuando aplicas el concepto de Knowledge Generation en prompts, *estás aprovechando la capacidad del modelo para comprender el contexto y generar respuestas que no solo se basan en la información existente en sus datos de entrenamiento, sino que también incorporan una capacidad para razonar, inferir y, en ciertos casos, generar contenido nuevo.*

🤖 En la práctica, al utilizar prompts específicos, puedes solicitar al modelo que genere información o respuestas que vayan más allá de la información que ha sido directamente alimentada durante su entrenamiento. Esto permite que el modelo sea más versátil y capaz de ofrecer respuestas únicas y contextualmente relevantes en una amplia gama de situaciones.

🤖 👉 Es importante señalar que, aunque los modelos de lenguaje como GPT-3.5 pueden generar conocimiento nuevo hasta cierto punto, no tienen una comprensión real del mundo y pueden producir respuestas que no son necesariamente precisas o verídicas. Por lo tanto, es fundamental interpretar y validar la información generada por estos modelos en función de la precisión y la coherencia con el conocimiento establecido.


### Knowledge Integration
Es la capacidad del modelo para integrar conocimiento que no conoce, con los datos que sí entiende, para poder generar conocimiento sobre temas particulares que no se encontraban en sus datos de entrenamiento, con el objetivo de ampliar su conocimiento sobre el tema y proporcionar respuestas más detalladas y precisas. A diferencia del Knowledge Generation, en este caso somos nosotros quienes le damos a conocer la nueva información a través de los prompts, para que luego pueda seguir instrucciones usando dicha información. ㅤ En el siguiente ejemplo, le preguntamos a GPT-3 sobre GPT-4, modelo que hasta la fecha de corte de su conocimiento, no existía. ㅤ

📥 Prompt: “¿Qué es GPT-4?” ❌ Respuesta: GPT-4 es una hipotética versión futura de la familia de modelos de lenguaje GPT (Generative Pre-trained Transformer) de OpenAI. Actualmente, el modelo más avanzado de esta familia es GPT-3, lanzado en 2020. GPT-4 sería una versión mejorada de GPT-3, con un mayor número de parámetros y una capacidad aún mayor para generar texto coherente y humano-like. Sin embargo, no se sabe cuándo será lanzado o cuáles serán sus características específicas.

ㅤ Ahora, a través de una instrucción, vamos a integrarle información reciente de OpenAI sobre GPT-4, para que la integre a sus conocimientos previos y pueda generarnos respuesta mucho más precisa, ahora conociendo detalles sobre GPT-4 que anteriormente no conocía. ㅤ

📥 Prompt: Integra la siguiente información con tu conocimiento en modelos de AI. ㅤ Información: GPT-4 es un gran modelo multimodal (que acepta entradas de imagen y texto, y emite salidas de texto) que exhibe un rendimiento a nivel humano en varios puntos de referencia académicos y profesionales. Por ejemplo, aprueba un examen de barra simulado con una puntuación de alrededor del 10 % superior de los examinados; por el contrario, la puntuación de GPT-3.5 se situó en torno al 10 % inferior. En una conversación informal, la distinción entre GPT-3.5 y GPT-4 puede ser sutil. La diferencia surge cuando la complejidad de la tarea alcanza un umbral suficiente: GPT-4 es más confiable, creativo y capaz de manejar instrucciones mucho más matizadas que GPT-3.5. ㅤ Para comprender la diferencia entre los dos modelos, se probó en una variedad de puntos de referencia, incluida la simulación de exámenes que fueron diseñados originalmente para humanos. Se procedió usando las pruebas disponibles públicamente más recientes (en el caso de las preguntas de respuesta libre de las Olimpiadas y AP) o comprando las ediciones 2022-2023 de los exámenes de práctica. No se realizó ningún entrenamiento específico para estos exámenes. El modelo detectó una minoría de los problemas en los exámenes durante el entrenamiento.” 🧠 Respuesta: (…) ㅤ 📥 Prompt: “¿Qué es GPT-4?” ✅ Respuesta: GPT-4 es un modelo de lenguaje de inteligencia artificial que acepta entradas de imagen y texto, y emite salidas de texto, y se caracteriza por ser un gran modelo multimodal que exhibe un rendimiento a nivel humano en varios puntos de referencia académicos y profesionales. GPT-4 ha superado a su predecesor, GPT-3.5, en términos de confiabilidad, creatividad y capacidad para manejar instrucciones más matizadas. Además, se ha probado en una variedad de puntos de referencia, incluyendo la simulación de exámenes diseñados originalmente para humanos, en los cuales ha obtenido resultados sobresalientes.

## Hiper parámetros de ChatGPT

# Casos de uso de ChatGPT
