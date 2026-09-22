# Capítulo 3 — Las palabras de la IA, sin palabras rebuscadas

## En palabras simples

La mayoría de las malas decisiones sobre IA no las causa una mala tecnología. Las causan palabras que nadie se detuvo a definir.

Un proveedor dice: «nuestra plataforma de IA se integra con tus sistemas mediante una API de bajo código y usa un gran modelo de lenguaje». Todos asienten. Nadie pregunta qué significa nada de eso. Seis meses después, el proyecto está fuera de presupuesto, los datos están en algún lugar inesperado, y nadie puede decir quién es dueño de qué.

Las palabras son la interfaz. Si tu equipo no comparte el mismo significado para «modelo», «entrenamiento» e «integración», no puede tomar buenas decisiones sobre ninguna de ellas. No puedes comparar dos proveedores. No puedes redactar un contrato. No puedes darte cuenta cuando algo va mal.

Este capítulo es un glosario de trabajo, no un diccionario. Cada palabra recibe un significado sencillo, una analogía cotidiana y la única pregunta que debes hacer cuando la oigas.

Una regla recorre todo. **Una explicación real siempre contiene un verbo y un objeto.** No «funciona con IA», sino «lee tus facturas y pone el total en tu archivo de contabilidad». Si alguien no puede darte un verbo y un objeto, no te ha dicho nada.

### 3.1 Dato, información, conocimiento

Tres palabras que la gente usa como si fueran lo mismo. Son tres pasos distintos, y la diferencia importa cuando planificas.

**Dato** es un hecho en bruto, sin significado asignado. Una columna de números. Una carpeta de PDF. Una lista de fechas. Un dato por sí solo no te dice nada. El número 47 es un dato.

**Información** es un dato con contexto. «La factura 47 era de 1.200 € y se pagó tarde». Ahora el número significa algo. La información es un dato colocado en algún sitio.

**Conocimiento** es información más una comprensión de qué hacer con ella. «Cuando este cliente paga tarde, suele ser porque su propio cliente paga tarde, así que le insistimos con suavidad y al final siempre paga». Eso es conocimiento. Vive en la cabeza de una persona, y costó años construirlo.

Piensa en un archivador. El dato es el papel. La información es el papel en una carpeta etiquetada. El conocimiento es saber qué carpetas importan el lunes por la mañana y cuáles pueden esperar hasta marzo.

**Por qué te importa.** La IA trabaja con datos. No adquiere automáticamente tu conocimiento. Puedes darle a un sistema diez mil facturas y aprenderá patrones en ellas. No aprenderá por qué tu cliente más grande siempre paga tarde a propósito, porque eso es conocimiento que tiene una sola persona que nunca lo ha escrito.

Antes de cualquier proyecto de IA, pregunta: **¿cuánto de lo que hace funcionar esta tarea está escrito como dato, y cuánto vive en la cabeza de alguien?** La distancia entre esos dos números es el tamaño de tu problema real. Cerrarla suele ser más difícil, y más valioso, que la parte de IA.

**Pregunta al proveedor:** «¿Qué datos necesitan de nosotros, en qué formato y cuántos?»

### 3.2 Algoritmo, modelo, entrenamiento

**Algoritmo.** Una receta. Un conjunto claro y ordenado de pasos que resuelve un problema. Hacer café es un algoritmo. La división larga es un algoritmo. Un algoritmo no necesita un ordenador; solo necesita pasos. La palabra viene del nombre del matemático del siglo IX al-Juarismi, cuyo trabajo sobre el cálculo paso a paso se tradujo al latín y acabó darnos la palabra.

**Modelo.** En el habla cotidiana de la IA, un modelo es lo que obtienes al final del entrenamiento: un conjunto de ajustes aprendidos que puedes usar para responder casos nuevos. Piensa en él como un empleado entrenado. No tienes que volver a enseñarle cada mañana. El conocimiento está en él.

La palabra se usa de dos maneras, y mezclarlas causa confusión. En el sentido antiguo, un modelo es una descripción escrita de cómo funciona algo, como un modelo financiero en una hoja de cálculo. En el sentido moderno de la IA, un modelo es un archivo lleno de números que se ajustaron hasta que las respuestas salieron bien. Cuando alguien dice «el modelo» hoy, normalmente se refiere a lo segundo.

**Entrenamiento.** El proceso de pasar de la nada a un modelo. Muestra ejemplos. Deja que el sistema adivine. Compara con la respuesta correcta. Ajusta. Repite muchas veces. El Capítulo 2 explicó el mecanismo. Lo que importa aquí es el significado empresarial: **el entrenamiento es un paso que pagas una vez, y su calidad fija el techo de todo lo que viene después.** Un modelo entrenado con ejemplos malos no se arregla con una interfaz mejor. Solo se puede reentrenar, lo que significa pagar otra vez.

Tres preguntas que aclaran casi cualquier conversación:

1. **¿Cuál es la entrada?** ¿Qué entra?
2. **¿Cuál es la salida?** ¿Qué sale?
3. **¿Con qué se entrenó?** ¿Qué ejemplos, de cuándo, cuántos?

Si un proveedor no puede responder la pregunta tres, no estás comprando un modelo. Estás comprando una promesa.

### 3.3 IA generativa, LLM, prompt

**IA generativa** es la IA que produce contenido nuevo en lugar de solo ordenar o puntuar. El Capítulo 2 la definió. Aquí está el vocabulario que la rodea.

**LLM — gran modelo de lenguaje.** «Grande» significa que tiene muchísimos ajustes, medidos en miles de millones. Esos ajustes se llaman **parámetros**. Un modelo de 13.000 millones de parámetros contiene 13.000.000.000 de números. «Lenguaje» significa que se entrenó con texto. «Modelo» significa que es el resultado utilizable del entrenamiento.

Así que un LLM es un conjunto de números muy grande, ajustado al leer una cantidad enorme de texto, hasta que se volvió bueno en continuar texto. Eso es todo. No es una base de datos de hechos. Es una máquina de continuar texto.

**Prompt.** El texto que le das al modelo. Tu pregunta, tu instrucción, tu petición. Eso es todo lo que es un prompt.

La palabra importa más de lo que parece, porque lo que recibes depende en gran medida del prompt. Un prompt vago da una respuesta vaga. Un prompt con contexto, un ejemplo y un formato claro da una mucho mejor. Aprender a escribir buenos prompts es una habilidad empresarial real, y se aprende bien en cerca de una semana.

Un prompt es como un encargo que le das a un redactor freelance. Un mal encargo —«escribe algo sobre nuestro producto»— saca algo inútil. Un buen encargo —«escribe 150 palabras para pequeños comerciantes, en español sencillo, con este tono, y deja fuera los precios»— saca algo que puedes usar. El redactor es el mismo. Solo cambió el encargo.

**Alucinación.** Cuando un modelo afirma algo falso de forma segura. La palabra es imperfecta, porque el modelo no alucina en ningún sentido médico. Está continuando texto de una manera que suena bien, sin un almacén aparte de hechos contra el que comprobar. Por eso la IA generativa necesita verificación para todo lo que importe.

**Ventana de contexto.** Cuánto texto puede considerar el modelo a la vez. Piensa en ello como un escritorio. Todo lo que quieras que mire debe caber en el escritorio. El texto que no cabe simplemente no está. Los escritorios modernos son grandes, pero no infinitos, y un escritorio abarrotado funciona peor que uno ordenado.

**Pregunta al proveedor:** «¿Qué modelo usan, quién lo hizo, y a dónde van mi prompt y mis datos cuando los envío?»

### 3.4 RPA, no-code, low-code

Estas tres palabras se venden como si fueran IA. Normalmente no lo son.

**RPA — Automatización Robótica de Procesos.** Software que copia lo que hace una persona en un ordenador: abrir este sistema, copiar este campo, pegarlo en aquel sistema, pulsar Guardar. Funciona imitando acciones de ratón y teclado, o usando las mismas pantallas que usa una persona. El término se empezó a usar a principios de los años 2000.

RPA no es IA. No tiene aprendizaje ni adivinanza. Sigue una secuencia grabada exactamente. Es fiable y frágil a la vez. La analogía es una macro en una hoja de cálculo: hace los mismos pasos cada vez, rápido, y se rompe si cambia el diseño.

**Cuándo RPA es lo correcto:** la tarea es fija, de mucho volumen, y las pantallas no cambian. Copiar datos de pedidos de un correo a tu sistema de pedidos cien veces al día es un trabajo clásico de RPA. Es barato y funciona.

**Cuándo RPA es lo incorrecto:** cualquier cosa que varíe. Si la entrada no está siempre en el mismo sitio, RPA se romperá, y lo hará a menudo.

Un patrón común y sensato: **la IA lee y entiende la entrada desordenada; RPA hace el tecleo aburrido.** La IA maneja la variación. El RPA maneja la repetición.

**No-code (sin código).** Herramientas donde construyes una automatización haciendo clic, arrastrando y eligiendo de un menú, sin escribir código de programación. Buenas para flujos de trabajo simples y claros. Rápidas de empezar.

**Low-code (bajo código).** Similar, pero puedes escribir un poco de código cuando el menú no ofrece lo que necesitas. Más flexible, un poco más técnico.

Ambos son realmente útiles, y ambos tienen un coste oculto: es fácil empezar y difícil terminar. Un flujo no-code que crece a veinte pasos, tres sistemas y cuatro personas editándolo se vuelve difícil de entender y peligroso de cambiar. Hay un patrón bien conocido en el que una empresa construye docenas de pequeñas automatizaciones no-code, nadie puede mapearlas todas, y al final alguien tiene que reconstruirlo todo.

**Pregunta al proveedor:** «¿Esto de verdad aprende algo, o sigue una secuencia fija? Si cambia una pantalla, qué se rompe y quién lo arregla?»

### 3.5 Nube, API, integración

**Nube.** El ordenador de otro. Esa es la definición honesta. Tus archivos y software se ejecutan en máquinas de un gran centro de datos que otra empresa posee y mantiene, y pagas por uso a través de internet.

La nube tiene ventajas reales: ningún hardware que comprar, capacidad que puedes ampliar en minutos, mantenimiento automático. También tiene una consecuencia permanente: **tus datos están en máquinas de otro, en un país que quizá no elegiste, bajo un contrato que probablemente no leíste.** El [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md) trata de ejecutar las cosas tú mismo, y el [Capítulo 11](ch11-digital-sovereignty.md) trata de control y soberanía.

**API — interfaz de programación de aplicaciones.** Una forma definida de que un software pida a otro que haga algo.

Piensa en la cocina de un restaurante. No puedes entrar y cocinar tu propia comida. Vas a una ventanilla y pides de un menú fijo. La cocina te dice exactamente qué puedes pedir y cómo. Esa ventanilla es la API: permite al mundo exterior usar la cocina sin romperla.

En la práctica, tu sitio web pregunta a la API de la empresa de envíos «¿cuánto costará enviar este paquete a Madrid?» y recibe un número en segundos. Nadie llama a nadie por teléfono.

Dos cosas que saber. Primera, si el producto de un proveedor no tiene API, no puedes conectarlo tú mismo a nada, y dependes de ese proveedor para siempre. Segunda, cada llamada a una API significa que los datos cruzan una frontera. Cada una es una pequeña puerta. Algunas puertas están cerradas con llave y registradas. Otras no.

**Integración.** Conectar sistemas para que los datos se muevan entre ellos sin que una persona los lleve. Aquí es donde la mayoría de los proyectos gastan de verdad su tiempo y dinero, y los proveedores raramente dicen a qué nivel se refieren:

1. **Archivos.** Exportar una hoja de cálculo, subirla a algún sitio. Simple, lento, propenso a errores.
2. **API.** Una conexión en vivo. Rápida, fiable, necesita trabajo de configuración.
3. **Nativa.** Integrada en la misma plataforma. Lo mejor, pero te ata a esa plataforma.

**Pregunta al proveedor:** «¿A qué sistemas se conectan hoy, por qué método, quién hace la configuración, y qué pasa con la conexión si nos vamos?»

## Un poco de historia

Las palabras son más antiguas que la tecnología, y saberlo ayuda.

**Algoritmo** viene de al-Juarismi, un matemático persa del siglo IX cuyos libros describían el cálculo paso a paso. La palabra tiene más de mil años más que el ordenador. **Dato** viene del latín «cosas dadas» —hechos en el sentido llano, mucho antes de significar algo almacenado—. **Red neuronal** viene de los años 1940, de los primeros intentos de describir una célula cerebral como un pequeño interruptor de encendido/apagado; la frase se quedó aunque los sistemas modernos se parezcan poco a los cerebros reales. **Aprendizaje automático** lo nombró en 1959 Arthur Samuel, un investigador estadounidense que trabajaba en un programa de damas. **Gran modelo de lenguaje** entró en uso común alrededor de 2018, cuando aparecieron modelos entrenados con texto a escala web. **Prompt** se toma prestado de la informática antigua, donde significaba el lugar donde tecleas; ahora significa la instrucción que das a un modelo, que es un trabajo mucho mayor que teclear. **RPA** apareció a principios de los 2000 para describir software que imita a un humano ante una pantalla, y **low-code** y **no-code** entraron en el vocabulario empresarial alrededor de 2014.

La lección del vocabulario es simple. Casi ninguna de estas palabras la inventaron las personas que construyeron la tecnología. Fueron tomadas prestadas, estiradas y luego vendidas. Por eso se sienten vagas. Son vagas. Tu trabajo es fijar cada una antes de firmar nada.

## Curiosidad

### 3.6 Un modelo entrenado solo con datos de los años 1930 escribió Python — ¿cómo es posible?

En abril de 2026 un pequeño equipo de investigación publicó un modelo de lenguaje inusual. Se llamaba **talkie**, y toda su gracia estaba en lo que no sabía.

El equipo —Nick Levine, David Duvenaud de la Universidad de Toronto, y Alec Radford— entrenó un modelo de 13.000 millones de parámetros solo con texto en inglés publicado antes de 1931. Unos 260.000 millones de tokens de él. Un **token** es un trozo pequeño de texto, más o menos una palabra o parte de una palabra. Las fuentes fueron libros digitalizados, periódicos, revistas, revistas científicas, patentes y jurisprudencia.

No entró nada de después de 1930. Ni ordenadores. Ni internet. Y crucialmente, ningún lenguaje de programación, porque Python no se creó hasta finales de los años 1980.

Luego probaron si podía escribir Python.

**El resultado.** Podía, un poco. El equipo dio al modelo una prueba estándar de programación llamada HumanEval, con un giro: cada problema venía con unas pocas funciones de ejemplo mostradas en la propia pregunta. El modelo nunca había visto Python en el entrenamiento. Pero podía mirar los ejemplos delante de él y copiar la estructura.

Los resultados fueron honestos y modestos. El modelo vintage quedó muy por debajo de los modelos modernos. Cada respuesta correcta que produjo era un programa simple de una línea, como sumar dos números, o un pequeño cambio a uno de los ejemplos que se le mostraron. Como dijo el equipo, aún queda un largo camino antes de que esta capacidad sea notable.

Pero un ejemplo fue genuinamente llamativo. Mostrada una función que codificaba un cifrado por rotación —un código donde cada letra se desplaza una cantidad fija—, el modelo produjo la función de decodificación cambiando un solo carácter, convirtiendo una suma en una resta. Nunca había visto Python. Nunca había visto un ordenador. Dedujo, por la forma del ejemplo delante de él, que decodificar es lo inverso de codificar.

**¿Cómo es posible?** La respuesta es un comportamiento llamado **aprendizaje en contexto**: captar un patrón de los ejemplos colocados directamente en la pregunta, en lugar del entrenamiento.

Aquí está la versión sencilla. Para leer texto bien, un modelo tiene que volverse extremadamente bueno en notar estructura. Qué palabra sigue a cuál. Qué se abre y qué se cierra. Qué es una definición y qué es un ejemplo. Qué es una causa y qué es un efecto. Aprende todo esto de libros y periódicos corrientes.

La estructura, resulta, se transfiere. Un modelo que se ha vuelto muy bueno en notar «este bloque se abre aquí, se cierra allá, y este valor fluye hacia aquel» puede aplicar esa misma habilidad a un bloque de Python que nunca ha visto. No está usando conocimiento de Python. Está usando conocimiento de estructura sobre material de Python.

Por eso pudo invertir la función del cifrado. No estaba programando. Era seguimiento de patrones aplicado a un asunto que no existía en sus datos de entrenamiento.

**Por qué lo hicieron los investigadores.** La razón es práctica e ingeniosa: un modelo entrenado solo con texto anterior a 1931 no puede haber memorizado el examen. Los modelos modernos se entrenan con la web moderna, que contiene las respuestas a la mayoría de las preguntas de examen públicas. Eso se llama **contaminación de datos**, y hace que las pruebas modernas no sean fiables. Un modelo puede puntuar bien porque vio la respuesta antes, no porque sepa razonar. Talkie es limpio por construcción. Lo que haga, lo hizo de verdad.

**Los límites honestos.** El equipo también informó de que talkie funcionó peor en general que su «gemelo moderno» —un modelo idéntico entrenado con datos web modernos—, incluso después de corregir el hecho de que las preguntas modernas confunden a un modelo de los años 1930. Atribuyeron parte de la distancia al ruido del OCR: en 1930 nada era digital, así que cada página tuvo que escanearse y transcribirse, lo que introduce errores que el texto nativo digital no tiene. Dijeron que, como esfuerzo de investigación amateur, nunca esperaron cerrar la distancia del todo. Sí estimaron que el corpus histórico podría crecer a muy por encima de un billón de tokens, suficiente para un modelo más o menos comparable al ChatGPT original.

**La lección empresarial.** Dos cosas.

Primera, estos modelos son seguidores de estructura más que recopiladores de hechos. Eso explica tanto su poder como su falta de fiabilidad. La estructura se transfiere bien. La verdad no viene con ella.

Segunda, **la contaminación de datos es un problema real en las afirmaciones de los proveedores.** Cuando un proveedor dice «nuestro modelo puntúa 94% en esta prueba», pregunta si la prueba estaba en los datos de entrenamiento. Esto no es un detalle técnico menor. Es la diferencia entre una capacidad medida y una respuesta memorizada. Pregúntalo en cada reunión con un proveedor.

## Un ejemplo empresarial real

### Cuando las palabras son el producto: el «lavado de IA»

En septiembre de 2024 la Comisión Federal de Comercio de Estados Unidos (FTC) anunció una operación de cumplimiento de la ley que llamó **Operation AI Comply**. El objetivo eran empresas que hacían afirmaciones exageradas o engañosas sobre lo que sus productos podían hacer con inteligencia artificial. El propio nombre de la FTC para la práctica es **lavado de IA** (AI washing).

El patrón que describieron los reguladores es simple, y vale la pena reconocerlo, porque así empiezan las malas compras de IA.

Una empresa tiene un producto corriente. Quizá una herramienta de agenda, o una herramienta de automatización de marketing, o un chatbot hecho de una lista fija de respuestas. La empresa añade «impulsado por IA» al marketing. Nada en el producto cambia. El precio sube. Las ventas suben.

La posición de la FTC es que esto es un problema de protección al consumidor, no técnico. Si afirmas una capacidad que no tienes, eso es una afirmación engañosa, y la etiqueta «IA» no te protege de ello.

**Por qué este es un ejemplo empresarial y no solo legal.** Porque la misma trampa funciona en ambas direcciones. Los proveedores usan las palabras a la ligera para vender. Los compradores usan las palabras a la ligera para justificar un presupuesto internamente. Un gestor que no puede explicar qué hace la tecnología escribe «automatización impulsada por IA» en una propuesta, consigue aprobado el presupuesto, y luego tiene que hacer funcionar algo que nadie definió.

La operación del regulador te sirve como lista de comprobación al revés. Antes de comprar, pregunta:

1. **¿Qué afirmación concreta se está haciendo?** Escríbela en una frase con un verbo y un objeto.
2. **¿Cómo sabríamos si esa afirmación fuera falsa?** Si nadie puede nombrar una prueba, la afirmación es decoración.
3. **¿Está la afirmación en el contrato?** El lenguaje de marketing no es un compromiso. Si una capacidad importa, debe escribirse con un número y una fecha.
4. **¿Quién responde si no rinde?** Nombra a una persona, no a una empresa.

Un proveedor honesto responde a las cuatro con comodidad. Un proveedor que está haciendo lavado se vuelve vago. La vaguedad como respuesta a preguntas concretas es en sí misma la respuesta.

## Cómo hacerlo

### La prueba de las palabras simples

Usa esto siempre que aparezca un término técnico en una reunión.

**Paso 1: Detente en la palabra.** No la dejes pasar porque suene importante.

**Paso 2: Pide una frase con un verbo y un objeto.** No «usa un gran modelo de lenguaje», sino «lee nuestros correos de soporte y redacta una respuesta». Si el hablante no puede producir una, la palabra aún no tiene contenido.

**Paso 3: Pregunta qué entra y qué sale.** Todo sistema real tiene una entrada y una salida. Escribe ambas.

**Paso 4: Pregunta qué lo rompe.** Toda tecnología tiene un modo de fallo. Un proveedor honesto nombra el suyo.

**Paso 5: Escribe tu propia definición en una línea y léela en voz alta.** Si un colega listo no pudiera entenderla, la definición no está terminada.

### Tu tabla de traducción de trabajo

| Palabra que oyes | Significado sencillo | Qué preguntar |
|---|---|---|
| Impulsado por IA | Usa algún componente aprendido, quizá diminuto | ¿Qué parte, exactamente? |
| Modelo | Un archivo de ajustes aprendidos que responde casos nuevos | ¿Entrenado con qué, cuándo, cuánto? |
| Entrenamiento | Ajustar ajustes contra ejemplos hasta que las respuestas coinciden | ¿Quién lo hizo, y quién lo comprobó? |
| LLM | Un sistema de continuación de texto muy grande | ¿Cuál, hecho por quién, ejecutándose dónde? |
| Prompt | La instrucción que das al modelo | ¿Podemos escribir y reutilizar los nuestros? |
| Alucinación | Una afirmación segura que es falsa | ¿Cómo la detectan y corrigen? |
| RPA | Software que imita a una persona haciendo clic en pantallas | ¿Qué se rompe cuando cambia la pantalla? |
| No-code | Construir haciendo clic, sin programar | ¿Qué no puede hacer? |
| Low-code | Sobre todo clics, algo de programación permitida | ¿Quién lo mantiene aquí? |
| Nube | Se ejecuta en ordenadores de otros | ¿Qué país, de quién el contrato, qué datos salen? |
| API | Una ventanilla definida para que un sistema use otro | ¿Existe? ¿Podemos usarla nosotros mismos? |
| Integración | Los datos se mueven entre sistemas sin una persona | ¿Qué método, quién lo configura, qué si nos vamos? |
| Token | Un trozo pequeño de texto | ¿Cuántos por uso típico, y cuánto cuesta eso? |
| Ventana de contexto | Cuánto texto puede mirar el modelo a la vez | ¿Qué pasa cuando nuestro documento es demasiado grande? |

### Construye un glosario compartido para tu empresa

Haz esto una vez y mantenlo vivo.

1. Empieza una sola página. Cada término que surja en una discusión sobre IA va a ella.
2. Cada entrada tiene tres líneas: el significado sencillo, lo que significa *en nuestro negocio*, y una pregunta que aún no podemos responder.
3. Una persona con nombre propio es dueña de la página. No un comité.
4. Antes de cualquier reunión con un proveedor, lee la página. Durante la reunión, añade a ella.
5. Retira las entradas que nunca uses. Mantenla por debajo de dos páginas.

Un glosario compartido es una cosa pequeña con un efecto descomunal. Convierte «compramos IA» en «usamos un modelo de texto para redactar respuestas y una herramienta de reglas para archivarlas, y una persona revisa ambas».

## Ética y responsabilidad

### 3.7 Privacidad, seguridad, sesgo — la versión corta

Tres palabras que oirás constantemente. Aquí está la introducción sencilla. El tratamiento completo vive en otra parte, y deberías leer esos capítulos antes de desplegar nada que toque datos de clientes.

**Privacidad** trata de quién tiene permiso para ver y usar información personal. La pregunta práctica para cada herramienta de IA es simple: *cuando pego algo, a dónde va, quién puede leerlo, y qué guardan ellos?* No metas nunca los datos personales de un cliente en una herramienta que no has comprobado. El [Capítulo 10](ch10-privacy-and-gdpr.md) trata la ley de privacidad y el RGPD como es debido.

**Seguridad** trata de proteger los sistemas de ataques, mal uso y accidentes. La IA añade nuevas formas de ser atacado, incluido engañar a un modelo con entradas cuidadosamente redactadas y envenenar los datos de los que aprende. El [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md) trata esto por completo.

**Sesgo** es cuando un sistema trata a algunas personas peor que otras de forma sistemática, porque los ejemplos de los que aprendió fueron desiguales. Si las decisiones de contratación pasadas favorecieron a un grupo, un modelo entrenado con ellas aprenderá a favorecer a ese grupo. El sesgo no es un fallo moral de la máquina. Es un espejo puesto ante los ejemplos. El [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md) trata el sesgo, la transparencia, la explicabilidad y la responsabilidad humana como parte del marco ético completo.

Lo único que sacar de esta sección: **no puedes gestionar un riesgo que no puedes nombrar.** Aprender las palabras no es académico. Es el primer requisito para hacer las preguntas correctas.

## Errores a evitar

**Error 1: Aceptar «IA» como una función.** No es una función. Es una categoría que contiene docenas de tecnologías muy distintas. Pregunta cuál.

**Error 2: Pensar que no-code significa no pensar.** No-code elimina la programación. No elimina el diseño, el mantenimiento, ni el riesgo de un enredo inmapeable de automatizaciones.

**Error 3: Confundir RPA con IA.** Si sigue una secuencia grabada, no está aprendiendo nada. Eso puede ser exactamente lo que quieres, o exactamente lo que fallará.

**Error 4: Pensar que una API significa que estás integrado.** Una API es una posibilidad, no una conexión. Alguien aún tiene que construir y mantener la conexión.

**Error 5: No preguntar dónde está realmente la nube.** «La nube» es un centro de datos, en un país, bajo un contrato. Pregunta cuál.

**Error 6: Dejar que un proveedor defina tus términos.** Si el vocabulario del proveedor es el único vocabulario en la sala, el proveedor controla la reunión.

**Error 7: Saltarse la prueba de las palabras simples porque parece lenta.** Cinco minutos de «¿qué significa eso realmente?» son más baratos que seis meses de un proyecto que nadie puede describir.

**Error 8: Creerse una prueba sin preguntar por la contaminación.** El experimento de Talkie existe precisamente porque los resultados de pruebas modernas pueden estar inflados por respuestas que ya estaban en los datos de entrenamiento.

## Ejercicio práctico

### 3.8 Traduce una frase técnica a palabras simples

Esta es la habilidad más útil de todo este capítulo. Practícala con estas seis frases. Escribe tu respuesta antes de leer la respuesta modelo.

**Frase 1:** «Nuestra plataforma aprovecha un gran modelo de lenguaje para ofrecer procesamiento inteligente de documentos a escala.»

*Respuesta modelo:* «Lee documentos y los ordena. Usa un sistema de texto muy grande para entenderlos. Funciona con muchos a la vez, no solo con uno.»

**Frase 2:** «La solución es un bot RPA de bajo código con integración de API en la nube.»

*Respuesta modelo:* «Un robot que copia datos de una pantalla a otra. Puedes configurarlo sobre todo haciendo clic. Habla con otros sistemas por internet mediante una conexión definida. Se ejecuta en los ordenadores del proveedor.»

**Frase 3:** «Usamos generación aumentada por recuperación para asentar el modelo en tu base de conocimiento.»

*Respuesta modelo:* «Antes de responder, busca las páginas relevantes de tus propios documentos y las usa como base. Esto reduce las respuestas inventadas. Solo funciona si tus documentos son buenos y están al día.»

**Frase 4:** «El modelo está ajustado fino con tus datos de dominio.»

*Respuesta modelo:* «Tomaron un modelo general existente y lo entrenaron más con tus ejemplos, así que se adapta mejor a tu negocio. Pagas por eso. También significa que tus datos fueron enviados a quien hizo el entrenamiento.»

**Frase 5:** «Nuestra IA ofrece una toma de decisiones explicable y transparente.»

*Respuesta modelo:* «Alegan que puedes ver por qué decidió lo que decidió. Pídeles que te lo muestren, en un caso real, ahora mismo. Si no pueden, la afirmación es decoración.»

**Frase 6:** «Es un sistema multiagente con orquestación.»

*Respuesta modelo:* «Varios componentes de IA trabajan en una tarea en secuencia o en paralelo, y algo los coordina. Pregunta: cuántos componentes, qué hace cada uno, y qué pasa si uno falla?»

**Ahora haz el tuyo.** Encuentra una frase de un correo de un proveedor que recibiste el mes pasado. Tradúcela con el mismo método: verbo y objeto, entrada, salida, qué se rompe. Envía tu traducción de vuelta al proveedor y pregunta si es correcta. Su reacción te dirá muchísimo.

## Lista de comprobación

### 3.9 Tu glosario mínimo

- [ ] Puedo explicar dato, información y conocimiento, y sé cuánto de mi conocimiento del negocio está escrito.
- [ ] Puedo definir algoritmo como «una receta»: un conjunto ordenado de pasos.
- [ ] Puedo definir modelo como «la cosa entrenada que usas para responder casos nuevos».
- [ ] Puedo definir entrenamiento como «ajustar ajustes contra ejemplos hasta que las respuestas coinciden».
- [ ] Sé que un LLM es un sistema de continuación de texto, no una base de datos de hechos.
- [ ] Sé que un prompt es la instrucción que doy al modelo, y que su calidad cambia el resultado.
- [ ] Sé qué es un token y más o menos cuánto cuestan los tokens por uso típico.
- [ ] Sé qué es una ventana de contexto y qué pasa cuando un documento es demasiado grande para ella.
- [ ] Sé que «alucinación» significa una afirmación falsa y segura, y que necesita verificación.
- [ ] Puedo distinguir RPA de IA, y sé que RPA es barato y frágil.
- [ ] Sé que no-code y low-code eliminan la programación, no el diseño ni el mantenimiento.
- [ ] Sé que «la nube» significa ordenadores de otros, en un país concreto, bajo un contrato concreto.
- [ ] Sé que una API es una ventanilla definida para que un sistema use otro, y siempre pregunto si existe una.
- [ ] Sé los tres niveles de integración: archivos, API, nativa.
- [ ] Uso la prueba de las palabras simples: un verbo, un objeto, una entrada, una salida y qué se rompe.
- [ ] He empezado un glosario compartido de una página con un dueño con nombre propio.
- [ ] Sé que privacidad, seguridad y sesgo tienen cada uno un capítulo completo, y los he leído o los leeré.

## Puntos clave

- La mayoría de las malas decisiones de IA vienen de palabras no definidas, no de una mala tecnología.
- Una explicación real siempre contiene un verbo y un objeto; si no puedes nombrar uno, no te han dicho nada.
- Los modelos son seguidores de estructura, no guardianes de hechos, por eso transfieren habilidades entre materias y por eso afirman falsedades con seguridad.
- El experimento de Talkie muestra que un modelo sin conocimiento de ordenadores aún puede escribir un poco de Python, y existe porque los resultados de pruebas modernas pueden estar inflados por datos contaminados.
- Fija cada término antes de firmar: qué entra, qué sale, qué lo rompe, y quién es su dueño.
