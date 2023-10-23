# Como escribir prompts en ChatGPT
Un prompt es una pregunta que se le hace a ChatGPT

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

# Casos de uso de ChatGPT
