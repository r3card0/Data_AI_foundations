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
🍅 ¿Que me puedes decir del concepto de Knowledge Generation aplicado en prompts?

🤖 ¡Hola! En el contexto de la inteligencia artificial y los modelos de lenguaje como GPT-3.5, el concepto de "Knowledge Generation" (Generación de Conocimiento) *se refiere a la capacidad del modelo para generar información nueva y relevante en función de los datos y el contexto proporcionados en el prompt.*

🤖 Cuando aplicas el concepto de Knowledge Generation en prompts, *estás aprovechando la capacidad del modelo para comprender el contexto y generar respuestas que no solo se basan en la información existente en sus datos de entrenamiento, sino que también incorporan una capacidad para razonar, inferir y, en ciertos casos, generar contenido nuevo.*

🤖 En la práctica, al utilizar prompts específicos, puedes solicitar al modelo que genere información o respuestas que vayan más allá de la información que ha sido directamente alimentada durante su entrenamiento. Esto permite que el modelo sea más versátil y capaz de ofrecer respuestas únicas y contextualmente relevantes en una amplia gama de situaciones.

🤖 👉 Es importante señalar que, aunque los modelos de lenguaje como GPT-3.5 pueden generar conocimiento nuevo hasta cierto punto, no tienen una comprensión real del mundo y pueden producir respuestas que no son necesariamente precisas o verídicas. Por lo tanto, es fundamental interpretar y validar la información generada por estos modelos en función de la precisión y la coherencia con el conocimiento establecido.

Un buen ejemplo es la capacidad del LLMs de crear historias. En base a un contexto que se proporciona en el prompt, el modelo crea una historia.

🍅 Crea una historia donde haya dos personajes principales, un unicornio con poderes magicos, que hable y que cague dulces y un tiranosaurio rex que habla, le gusta mucho jugar videojuegos y sea un poco travieso. Ambos personajes no miden mas de 1.5m y siempre estan juntos viviendo aventuras en un mundo donde hay bosques magicos y piratas de alta mar.

🤖 *En un mundo mágico lleno de bosques encantados y océanos misteriosos, vivían dos amigos inusuales: Sparkle, un pequeño unicornio con poderes mágicos y la habilidad única de cagar dulces, y Rex, un tiranosaurio rex parlante aficionado a los videojuegos y un tanto travieso. A pesar de sus diferencias, ambos medían no más de 1.5 metros y compartían una amistad única y especial.*

🤖 *Un día, mientras exploraban un bosque mágico lleno de criaturas fascinantes y árboles centenarios, Sparkle y Rex se encontraron con un mapa antiguo que sugería la existencia de un tesoro escondido en una isla lejana. Emocionados por la perspectiva de una nueva aventura, decidieron zarpar hacia los mares desconocidos y enfrentarse a los piratas que custodiaban el tesoro.*

*A lo largo de su viaje, Sparkle usaba sus poderes mágicos para iluminar el camino y proteger a sus amigos, mientras que Rex pasaba las noches jugando videojuegos en la cubierta del barco, siempre buscando mejorar sus habilidades. Aunque travieso, Rex demostró ser un aliado valioso cuando se enfrentaron a desafíos en alta mar, utilizando su astucia para resolver problemas y derrotar a los piratas enemigos.*

*Durante una tormenta intensa, el barco quedó atrapado en una isla misteriosa. Mientras exploraban la isla en busca de pistas sobre el tesoro, Sparkle y Rex se encontraron con seres mágicos y desafíos que pusieron a prueba su amistad. Trabajaron juntos, superando obstáculos y resolviendo enigmas hasta llegar al lugar indicado en el mapa.*

*Finalmente, encontraron el tesoro escondido, un cofre lleno de gemas resplandecientes y objetos mágicos. Al abrirlo, liberaron una energía mágica que transformó la isla en un lugar aún más maravilloso. Los amigos regresaron a casa con sus tesoros y recuerdos inolvidables de su aventura.*

*A partir de ese día, Sparkle y Rex continuaron viviendo emocionantes experiencias, explorando bosques mágicos, enfrentándose a piratas y disfrutando de los videojuegos bajo la luz de la luna. Su amistad única demostró que, sin importar cuán diferentes sean dos seres, la verdadera magia se encuentra en la conexión y la diversidad de la amistad.*


### Knowledge Integration
🍅 Explica la técnica de Knowledge Integration

🤖 La "Knowledge Integration" (Integración de Conocimiento) es una técnica que se refiere a la *capacidad de un modelo o sistema para combinar y utilizar de manera coherente información de **diversas fuentes o áreas de conocimiento***. En el contexto de la inteligencia artificial y los modelos de lenguaje, como GPT-3.5, ***la Knowledge Integration implica la habilidad de asimilar datos de diferentes dominios y generar respuestas que integren de manera efectiva esa información diversa.***

🤖 Cuando se aplica la técnica de Knowledge Integration, el modelo no solo se basa en la información proporcionada en el prompt, sino que también utiliza su conocimiento previo y la comprensión del contexto para generar respuestas más completas y coherentes. Esto permite al modelo integrar información de diversas disciplinas y proporcionar respuestas más informadas y contextualmente ricas.

🤖 Un ejemplo de Knowledge Integration en la práctica podría ser:

**Prompt:**
```
Describe los impactos ambientales y las implicaciones económicas de la introducción de energía renovable a gran escala en la industria manufacturera.
```

🤖 En este caso, el modelo debería integrar conocimientos sobre energía renovable, impactos ambientales, economía y manufactura para ofrecer una respuesta completa y bien informada. La capacidad para integrar información de estas diferentes áreas de conocimiento permitiría al modelo generar una respuesta que vaya más allá de la información específica proporcionada en el prompt.

🤖 👉 Es importante señalar que, aunque los modelos de lenguaje pueden realizar tareas de Knowledge Integration hasta cierto punto, su capacidad para comprender el contexto y proporcionar respuestas precisas depende en gran medida de la calidad y diversidad de los datos con los que han sido entrenados. Además, siempre es necesario validar la información generada utilizando fuentes confiables y conocimientos establecidos para garantizar la precisión y coherencia.

🧠 Knowledge Integration es la técnica  que integra el conocimiento de varios dominios para resolver un problema.

🍅 como ejemplo de la tecnica de Knowledge integration, quiero combinar el conocimiento de dos dominios, el primero el de petrofisica basica y el segundo de Python, entonces, crea una clase que cuente con una funcion que calcule la porosidad primaria de una formacion

🤖 Claro, puedo proporcionarte un ejemplo simple de integración de conocimientos combinando el dominio de petrofísica básica y el lenguaje de programación Python. Aquí tienes una clase que incluye una función para calcular la porosidad primaria de una formación:

```python
class PetrofisicaCalculadora:
    def __init__(self, densidad_matriz, densidad_fluido, densidad_grano):
        self.densidad_matriz = densidad_matriz
        self.densidad_fluido = densidad_fluido
        self.densidad_grano = densidad_grano

    def calcular_porosidad_primaria(self):
        try:
            # Fórmula de porosidad primaria
            porosidad_primaria = (
                (self.densidad_matriz - self.densidad_fluido) /
                (self.densidad_matriz - self.densidad_grano)
            ) * 100

            return porosidad_primaria

        except ZeroDivisionError:
            print("Error: La densidad de la matriz y la densidad del grano deben ser distintas.")

# Ejemplo de uso
if __name__ == "__main__":
    # Crear una instancia de la clase PetrofisicaCalculadora
    calculadora = PetrofisicaCalculadora(densidad_matriz=2.65, densidad_fluido=1.0, densidad_grano=2.71)

    # Calcular y mostrar la porosidad primaria
    porosidad_resultado = calculadora.calcular_porosidad_primaria()
    print(f"La porosidad primaria es: {porosidad_resultado:.2f}%")
```

🤖 En este ejemplo, la clase `PetrofisicaCalculadora` tiene un método llamado `calcular_porosidad_primaria`. Este método utiliza la fórmula de porosidad primaria, una medida común en petrofísica, que involucra las densidades de la matriz, el fluido y el grano de la formación.

🤖 Este ejemplo combina conocimientos de petrofísica básica (la fórmula de porosidad primaria) con el uso de Python para crear una clase que puede realizar este cálculo. Es un simple ejemplo de cómo se podría integrar conocimiento de diferentes dominios para realizar tareas específicas.

## Hiper parámetros de ChatGPT

🍅 Explica el concepto de hyper parametros a un niño de 8 años

🤖 ¡Hola de nuevo! Claro, intentemos con un enfoque diferente:

🤖 Imagina que estás enseñando a un robot a dibujar, pero este robot tiene una varita mágica que puedes ajustar de diferentes maneras. Cuando ajustas la varita mágica, le estás diciendo al robot cómo debería dibujar de una manera especial. Es como si le dieras reglas especiales para que sus dibujos sean los mejores.

🤖 Estos ajustes mágicos son como los "hiperparámetros" para el robot. Si alguna vez piensas, "Quiero que el robot haga dibujos aún más increíbles", puedes cambiar algunos de estos ajustes mágicos para que el robot dibuje de una manera diferente. Tal vez quieras que sus líneas sean más suaves o que use colores más brillantes.

🤖 En la inteligencia artificial, cuando enseñamos a las computadoras a hacer cosas, también les damos reglas especiales para que aprendan. Esos ajustes mágicos son los "hiperparámetros". Pueden ser como decirle a la computadora cuánto debe aprender de los datos, o cuánto debe enfocarse en detalles específicos.

🤖 En resumen, los "hiperparámetros" son como los ajustes mágicos que les decimos a las computadoras para que hagan un trabajo realmente bueno en lo que están aprendiendo. Es como darle al robot las instrucciones perfectas para que haga los mejores dibujos. ¿Cómo suena ahora?

🍅 Dame un ejemplo del uso de hyper parametros en un prompt

🤖 ¡Claro! Imagina que tienes una varita mágica y quieres enseñarle a una computadora a adivinar el número que estás pensando. Ahora, la varita mágica tiene algunos ajustes especiales llamados "hiperparámetros". Aquí hay un ejemplo de cómo podrías usarlos en un "prompt":

**Prompt:**
```
Piensa en un número del 1 al 100. Quiero que la computadora adivine ese número, pero quiero que lo haga de la mejor manera posible. Ajusta los hiperparámetros para optimizar la precisión de la adivinanza. Puedes cambiar cosas como la cantidad de intentos, la velocidad de aprendizaje y la cantidad de pistas que la computadora puede utilizar.
```

🤖 En este prompt, estás dando instrucciones a la computadora sobre cómo debería ajustar sus hiperparámetros para mejorar su capacidad para adivinar el número que estás pensando. Puedes imaginarte que la computadora ajusta la "configuración" interna (hiperparámetros) para mejorar su rendimiento en la tarea específica de adivinanza.

🤖 Esta es solo una manera de pensar en ello, y en el mundo real, los hiperparámetros pueden ser ajustados para tareas más complejas, como entrenar modelos de aprendizaje automático para reconocer imágenes, traducir idiomas o cualquier otra tarea específica que quieras que la computadora realice de la mejor manera posible.

🤖 Otra manera. Vamos a imaginar que tienes una varita mágica que te ayuda a enseñar a un robot a jugar un juego. Ahora, la varita tiene algunos ajustes especiales llamados "hiperparámetros" que puedes cambiar para que el robot sea un jugador aún mejor.

**Prompt:**
```
Enséñale al robot a jugar al juego de adivinanzas. Queremos que sea muy bueno y que aprenda rápido. Ajusta los hiperparámetros de la varita mágica para lograrlo.
```

En este ejemplo:

1. **Tasa de Aprendizaje:** Puedes ajustar la tasa de aprendizaje para decirle al robot cuánto debe aprender de cada intento. Un valor alto hará que aprenda más rápido, pero también podría olvidar algunas cosas. Un valor bajo hará que aprenda más lentamente, pero podría recordar mejor.

2. **Número de Intentos:** Puedes ajustar cuántos intentos le das al robot para aprender. Un número alto le dará más oportunidades de aprender, pero también podría tardar más tiempo. Un número bajo hará que aprenda más rápido, pero con menos oportunidades.

3. **Foco en Detalles o Conceptos Generales:** Puedes ajustar si quieres que el robot preste mucha atención a detalles pequeños o si debe concentrarse en entender conceptos más grandes del juego.

Cambiar estos ajustes sería como girar los "hiperparámetros" en la varita mágica para decirle al robot cómo queremos que aprenda. Así, al ajustar estos hiperparámetros, ayudamos al robot a volverse un jugador de adivinanzas muy hábil. ¡Es como darle instrucciones mágicas para que aprenda de la mejor manera posible!

#### Hyper paramatros de temperatura y top_p
🤖 Los hiperparámetros de temperatura (temperature) y top-p son específicos del modelo de lenguaje GPT (Generative Pre-trained Transformer) y están relacionados con la generación de texto. Estos hiperparámetros se utilizan para ajustar la diversidad y la creatividad de las respuestas generadas por el modelo.

1. **Temperatura (Temperature):**
   - **Baja Temperatura (valor cercano a 0):** Hace que el modelo sea más determinista y tienda a generar respuestas más predecibles y centradas en las elecciones más probables.
   - **Alta Temperatura (valor mayor a 1):** Aumenta la aleatoriedad y la diversidad en las respuestas generadas, ya que permite que se exploren opciones menos probables.

   En términos sencillos, la temperatura controla cuánto "caos" o aleatoriedad quieres en las respuestas del modelo. Una temperatura baja tiende a producir respuestas más conservadoras y coherentes, mientras que una temperatura alta puede dar lugar a respuestas más sorprendentes y variadas.

2. **Top-p (también conocido como Nucleus Sampling):**
   - **Top-p = 1.0:** Selecciona siempre la palabra más probable, similar a la generación con temperatura baja.
   - **Top-p < 1.0:** Limita la selección a un subconjunto de las palabras más probables, excluyendo palabras menos probables.

   🤖 El hiperparámetro top-p se utiliza para controlar la probabilidad acumulativa de las palabras que se consideran para la generación de texto. Reducir top-p permite que el modelo se centre en un conjunto más estrecho de opciones, eliminando las opciones menos probables.

🤖 Estos hiperparámetros son útiles cuando se quiere ajustar el equilibrio entre la coherencia y la creatividad en la generación de texto. La elección de valores específicos dependerá del escenario de uso y de la naturaleza deseada de las respuestas generadas. Experimentar con diferentes valores de temperatura y top-p puede ayudar a obtener el tipo de salida que mejor se adapte a tus necesidades.

# Casos de uso de ChatGPT
