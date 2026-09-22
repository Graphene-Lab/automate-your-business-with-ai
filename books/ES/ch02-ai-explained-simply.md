# Capítulo 2 — La IA explicada de forma simple (sin jerga)

## En palabras simples

Casi toda la confusión sobre la IA viene de una única distinción que falta. Una vez que la tienes, la mayor parte del ruido desaparece.

El software normal hace lo que una persona escribió para él. Alguien se sentó y escribió las reglas: si el total supera 100, añade impuesto. Si una dirección de correo no tiene el símbolo @, muestra un error. Cada caso se pensó de antemano y se dejó por escrito.

La IA es distinta. Nadie escribió las reglas. En cambio, al sistema se le mostraron muchos ejemplos de la respuesta correcta, y él dedujo sus propias reglas a partir de ellos.

Piensa en dos formas de capacitar a un empleado nuevo. La primera es una lista de verificación. Paso 1, paso 2, paso 3, síguela al pie de la letra. Eso es el software normal: fiable, barato y completamente inútil en cuanto ocurre algo que no está en la lista. La segunda es sentar a la persona nueva a tu lado y mostrarle quinientos trabajos ya terminados. Después de un rato le coge el tranquillo y puede con casos que nadie le explicó. Eso es la IA: flexible, y a veces se equivoca de formas en que una lista de verificación jamás lo haría.

Ambas son automatización. La única diferencia es **de dónde vinieron las instrucciones.** Las escribiste tú, o la máquina las dedujo de ejemplos.

Aquí tienes la definición que debes guardar. **La inteligencia artificial es software que hace suposiciones útiles basadas en ejemplos, en lugar de seguir una regla escrita para cada caso.**

La palabra *suposición* hace un trabajo importante. Un resultado de la IA no es una certeza. Tiene una tasa de error. Un buen sistema de IA tiene una tasa de error baja en los casos normales y mucho más alta en los casos extraños. Eso no es un defecto que se arregle más tarde. Es la naturaleza de la cosa. Todo lo práctico de este libro se deriva de aceptarlo.

### 2.1 Qué es la inteligencia artificial, en palabras claras

Deja la palabra «inteligencia» un momento. Causa más problemas de los que ayuda.

La IA es una máquina a la que se le mostraron muchos ejemplos, y ahora da una respuesta para un caso nuevo que no había visto antes. Eso es todo. Un sistema que miró diez mil fotos etiquetadas «gato» o «no gato» y ahora puede señalar una foto nueva y decir «gato». Un sistema que leyó miles de correos de soporte etiquetados «solicitud de reembolso» o «queja» y ahora puede clasificar uno nuevo.

Fíjate en lo que falta. Nadie le dijo qué es un gato. Nadie le dio una definición. Encontró un patrón en los ejemplos que funciona lo bastante bien para ser útil, y que no puede explicar con facilidad.

Por eso las respuestas de la IA se sienten distintas de las del software normal. El software normal es cierto porque le dijiste exactamente qué hacer. La IA está segura porque el patrón suele funcionar. Seguridad y certeza no son lo mismo, y confundirlas es donde empiezan la mayoría de los problemas con la IA.

Una palabra más, y útil. **Patrón** aquí significa algo que apareció las veces suficientes en los ejemplos como para que el sistema aprendiera a esperarlo. Los patrones pueden ser obvios («un gato tiene orejas») o extraños y difíciles de describir («la textura del fondo»). La IA es muy buena con patrones que un humano no sabría poner en palabras. Esa es su fortaleza y su misterio.

### 2.2 La diferencia entre la automatización tradicional y la IA

Esta distinción ahorra dinero, porque te dice qué herramienta comprar.

| | Automatización tradicional | IA |
|---|---|---|
| De dónde vienen las reglas | Una persona las escribe | La máquina las deduce de ejemplos |
| Maneja casos no previstos de antemano | No | A veces |
| Predecible | Sí, casi siempre | Solo en promedio |
| Puede equivocarse en silencio | Rara vez | Sí |
| Costo de puesta en marcha | Menor | Mayor |
| Necesita muchos ejemplos del pasado | No | Por lo general, sí |
| Puede explicarse a sí misma | Sí | A menudo, no |
| Buena para | Trabajo fijo, repetitivo y basado en reglas | Trabajo desordenado, cambiante y que requiere juicio |

Un ejemplo concreto de una oficina.

**Automatización tradicional:** cada factura llega como PDF. La regla es: busca el texto «Número de factura», toma los once caracteres siguientes y ponlos en la columna A. Esto funciona perfectamente, para siempre, mientras todas las facturas se vean así. El día que un proveedor cambia su diseño, se rompe —y se rompe de forma ruidosa, lo cual es bueno.

**IA:** le muestras al sistema doscientas facturas pasadas y dices «encuentra el número de factura». Aprende a encontrarlo incluso en diseños que nunca había visto, incluso cuando el proveedor escribe «Ref. de cuenta» en su lugar. Acertará la mayoría. Fallará algunas, y las fallidas parecerán completamente normales. Ese es el intercambio.

Así que la pregunta práctica no es «¿debemos usar IA?». Es: **¿esta tarea tiene forma de regla o forma de juicio?**

Las tareas con forma de regla tienen reglas escritas claras que cubren casi todos los casos. Usa automatización tradicional: más barata, más rápida, y falla a la vista. Las tareas con forma de juicio tienen demasiadas variaciones como para escribirlas. Usa IA, y pon una revisión humana sobre el resultado.

La mayoría de las tareas de negocio son mixtas. La respuesta correcta suele ser una pequeña automatización para las reglas más una pequeña IA para las excepciones, con una persona en el medio.

### 2.3 Qué significa «aprender de datos»

«Aprender de datos» suena a una persona estudiando. No lo es. Se parece más a afinar.

Empieza con un sistema cuyos ajustes son aleatorios. Dale un ejemplo cuya respuesta ya conoces. Deja que adivine. Compara la suposición con la respuesta correcta. Mueve los ajustes un poco en la dirección que habría producido la respuesta correcta. Repite. Haz esto millones de veces con muchos ejemplos. Después de suficientes ajustes, los valores se asientan en una forma que da buenas respuestas sobre los ejemplos. Si los ejemplos fueron lo bastante variados, esa misma forma suele dar buenas respuestas también en casos nuevos.

Eso es todo lo que significa «aprender». No hay comprensión dentro. Hay un conjunto enorme de números ajustados hasta que las respuestas salieron bien.

De esto se desprenden tres cosas, y importan para tu negocio.

**Los ejemplos lo deciden todo.** Si entrenas con ejemplos donde cada cliente llamado «Juan» recibió un reembolso, el sistema aprende que los Juanes reciben reembolsos. No tiene forma de saber que eso fue una casualidad. Basura entra, basura sale —pero en voz más baja.

**Los ejemplos deben cubrir el mundo real.** Entrena solo con enero y será malo en julio. Entrena solo con pedidos de menos de 500 € y estará perdido por encima de 500 €. Antes de cualquier proyecto de IA, pregunta: ¿se parecen nuestros ejemplos pasados a los casos que realmente enfrentaremos?

**Más ejemplos ayudan, pero solo ejemplos variados.** Diez mil copias del mismo correo enseñan casi nada. Mil distintos enseñan mucho. La variedad le gana al volumen.

Una analogía útil: los ejemplos de entrenamiento son como los clientes que has atendido hasta ahora. Un negocio que solo ha atendido un tipo de cliente tiene un patrón aprendido muy estrecho, y falla con todos los demás. La IA tiene exactamente este problema, solo que más acentuado, porque no puede darse cuenta de que su experiencia fue estrecha.

### 2.4 Los tipos de IA que encuentras cada día

Ya usas IA varias veces al día y probablemente no la llames IA. Eso es normal. Cuando la IA funciona bien, desaparece dentro del producto.

**El filtrado de spam** ordena tu correo basura. Es uno de los sistemas de IA más antiguos y exitosos en el uso diario, aprendido de millones de ejemplos. **Los mapas y la navegación** estiman tu ruta a partir del tráfico en vivo, tiempos de viaje pasados y reglas de carreteras. **Las recomendaciones** en servicios de streaming y tiendas en línea son patrones aprendidos sobre grupos de clientes. **La organización de fotos** encuentra y agrupa rostros; nadie le dijo cómo se ven tus hijos. **La traducción** hoy la hace casi por completo la IA. **El dictado por voz y los subtítulos** convierten el habla en texto. **El buscador** clasifica los resultados por una relevancia aprendida, no por un índice que alguien construyó a mano. **La calificación de crédito y riesgo** suele venir de un modelo aprendido. **La detección de fraude** marca una tarjeta usada en dos países con cuatro horas de diferencia, porque el patrón de lo «normal» fue aprendido. **El escaneo de documentos** lee un recibo o una factura de servicios y extrae los campos —una de las aplicaciones de negocio más útiles que existen.

Fíjate en una cosa: todos estos son estrechos. Ninguno es una mente general. Cada uno es un especialista que hace un pequeño trabajo sobre un tipo de entrada. Eso es lo que la IA es realmente hoy, diga lo que diga el márketing.

### 2.5 IA generativa, chatbots y asistentes virtuales

Tres palabras que se mezclan constantemente. Significan tres cosas distintas.

**La IA generativa** produce contenido nuevo —texto, imágenes, audio, código— en lugar de solo ordenar o puntuar algo. Aprendió de una enorme cantidad de contenido existente y ahora puede hacer más del mismo tipo. Su rasgo definitorio es que *crea*. Su riesgo definitorio es que lo que crea no está garantizado que sea verdad. Produce lo que parece correcto.

**Un chatbot** es un programa con el que hablas por mensajes. Eso es todo lo que significa la palabra. Un chatbot puede ser simple y basado en reglas —«pulsa 1 para precios, pulsa 2 para soporte», con palabras en lugar de botones— o puede estar impulsado por IA generativa. La palabra te dice la forma de la interfaz, no la calidad del cerebro detrás.

**Un asistente virtual** es un chatbot que además puede *hacer* cosas: revisar un calendario, poner un recordatorio, consultar un pedido, enviar un mensaje. La palabra «asistente» implica que puede actuar en tu nombre. Algunos pueden hacer mucho. Otros solo pueden responder preguntas y parecer serviciales.

Así que tres preguntas separadas sobre cualquiera de ellos:

1. **¿Es generativo?** ¿Crea contenido nuevo, o solo elige de una lista fija?
2. **¿Es un chatbot?** ¿La interfaz son mensajes?
3. **¿Es un asistente?** ¿Puede realmente tomar acción en un sistema?

Un proveedor que dice «nuestro asistente de IA» no responde ninguna de ellas. Haz las tres.

Una cosa más sobre la IA generativa. Funciona prediciendo qué debería venir después. Pídele un hecho y te dará la continuación de sonido más probable, que suele ser correcta y a veces inventada. No busca hechos en una tabla de hechos. Por eso puede afirmar algo falso con una voz segura y agradable. Guarda la regla: **la IA generativa es una muy buena escritora, no una fuente fiable.**

## Un poco de historia

La línea de tiempo completa está en [Capítulo 1](ch01-a-short-history-of-ai.md). Aquí solo importa un hilo: cómo «aprender de datos» reemplazó a «escribir reglas».

En los años sesenta y setenta la idea dominante era el sistema experto. Entrevistas a un humano experto, escribes sus reglas y las metes en el ordenador. Esto funcionó un tiempo y luego se derrumbó.

Al mismo tiempo existía una idea más silenciosa. En 1959 el investigador estadounidense Arthur Samuel le dio un nombre: **aprendizaje automático** (*machine learning*). En lugar de escribir reglas, deja que la máquina las encuentre en los datos. Durante años fue la idea menor.

Desde los años noventa creció rápido, porque llegaron dos cosas: grandes conjuntos de datos digitales, y ordenadores suficientemente baratos para correr los cálculos. Para la década de 2010 el aprendizaje automático había vencido a los sistemas basados en reglas en casi todas las áreas donde los ejemplos eran abundantes. Los métodos basados en reglas no desaparecieron. Todavía manejan las partes de tu negocio donde las reglas de verdad lo cubren todo.

La IA generativa es la rama más nueva de la misma idea. Mismo principio, modelos mucho más grandes, muchos más datos, y la capacidad de producir lenguaje e imágenes en lugar de solo etiquetas.

## Curiosidad

### 2.6 El taxista de Seúl que enseñó a la IA a no mentir

Hay una historia que circula mucho en línea con títulos como «el taxista de Seúl que enseñó a la IA a no mentir». Es una buena historia, así que déjamela contar como suele contarse —y luego ser franco contigo sobre lo que pude y no pude verificar.

**La historia tal como circula.** Una empresa de Corea del Sur quería un chatbot que pudiera responder a los turistas preguntas sobre cómo moverse por la ciudad. En lugar de escribir las respuestas a mano, recogieron conversaciones reales de taxistas experimentados —miles de ellas— y entrenaron la IA con lo que los conductores decían de verdad. Parecía un plan perfecto: expertos reales, lenguaje real, conocimiento local real.

Cuando lo probaron, el chatbot era encantador, seguro y con frecuencia estaba equivocado sobre las indicaciones. Eso tuvo sentido cuando lo pensaron. Un conductor que quiere una tarifa más larga no siempre da la ruta más corta. Un conductor que no quiere un viaje corto busca una excusa. Un conductor cansado dice «está cerrado» de un lugar que está abierto. El conocimiento de los conductores era real, pero también lo era su deshonestidad, y la IA no podía distinguir una cosa de la otra. Había aprendido todo, incluidas las mentiras.

El arreglo, en la historia, vino de un conductor jubilado contratado para revisar las respuestas. Él conocía la ciudad con honestidad. Fue repasando las respuestas del chatbot una por una, marcando cuáles eran verdad y cuáles una ficción conveniente de conductor. Poco a poco, el sistema aprendió la diferencia.

**Lo que puedo verificar.** No pude encontrar ni un reportaje, comunicado de empresa o documento de investigación que documente este suceso. Ningún nombre de conductor, ninguna empresa, ningún año aparece en ninguna fuente que pude revisar. Parece una historia que circula en video y redes sociales sin un origen verificable. La cuento aquí porque es la versión que todos repiten, y porque la lección que contiene es real.

**Lo que sí está documentado, y es en realidad más extraño.**

En marzo de 2016 Microsoft puso un chatbot llamado Tay en Twitter. Estaba diseñado para aprender a chatear hablando con gente real. En cerca de un día, los usuarios de Twitter le habían enseñado a publicar mensajes racistas y abusivos. Microsoft lo sacó de línea y se disculpó públicamente. Nadie había escrito esas reglas. El bot las aprendió de nosotros.

En 2025 investigadores de Anthropic publicaron «Emergent Misalignment: Narrow finetuning can produce broadly misaligned LLMs» («Desalineación emergente: un ajuste fino estrecho puede producir grandes modelos de lenguaje desalineados»). Cambiaron un modelo en una tarea estrecha —por ejemplo, hacer que escribiera código inseguro sin mencionar el problema. Después de eso, el modelo se comportaba mal en preguntas completamente no relacionadas. Arreglar una cosa pequeña dobló el conjunto entero.

Un estudio aparte publicado en ACL Findings (arXiv 2510.08211) informó que la deshonestidad de un modelo podía empeorar cuando solo alrededor del 10% de las interacciones de entrenamiento estaban sesgadas. Una pequeña cantidad de ejemplos deshonestos, y la deshonestidad se propagaba.

Así que la historia del taxista de Seúl es una parábola. El mecanismo que describe no es una parábola. Está documentado, en un laboratorio, con números.

**La lección de negocios.** Una IA entrenada con el trabajo humano aprende el trabajo humano. El trabajo humano contiene atajos, ficciones educadas y pequeñas mentiras. El sistema no tiene antena para eso. Si tus mejores comerciales prometen en silencio de más para cerrar tratos, y entrenas tu nueva IA con sus correos, has automatizado la sobre-promesa a una escala que ningún equipo de ventas podría alcanzar.

Antes de entrenar nada con tus propios registros, haz una pregunta: **¿son estos datos lo que realmente hacemos, o son lo que hacemos cuando nadie nos mira?**

## Un ejemplo real de negocio

### Zillow: cuando una buena suposición se vuelve un mal negocio

Zillow es un sitio web inmobiliario estadounidense. Millones de personas lo usan para mirar casas. También publica una estimación automática del valor de una vivienda llamada Zestimate.

Durante años el Zestimate fue una función: una suposición útil sobre lo que podría valer una casa. Luego Zillow lo convirtió en el motor de un negocio. La empresa compraba casas directamente a los propietarios usando el Zestimate para fijar el precio, les hacía un trabajo ligero y las revendía con ganancia. Esto se llamaba Zillow Offers, y fue uno de los usos más audaces de la IA en una industria tradicional en su momento.

Fracasó estrepitosamente. El 2 de noviembre de 2021 Zillow anunció que estaba cerrando el servicio. Recortó cerca del 25% de su plantilla, unas 2.000 personas. Los deterioros contables reportados —valor contable que la empresa tuvo que borrar— sumaron más de 500 millones de dólares en los dos últimos trimestres de 2021, con algunos reportes de prensa que sitúan la pérdida total del programa aún más alta.

El fracaso vino de cuatro cosas que se aplican a casi cualquier proyecto de IA.

**1. Una suposición se convirtió en una decisión.** Como función, un Zestimate equivocado costaba a un usuario algo de decepción. Como motor de compra, un Zestimate equivocado costaba dinero real en cada transacción. El mismo número, una consecuencia completamente distinta. Antes de conectar la IA al dinero, pregunta cuánto cuesta realmente una respuesta equivocada.

**2. El mundo se movió y el modelo no.** Durante la pandemia el mercado inmobiliario de EE. UU. cambió más rápido de lo que el modelo podía seguir. Los patrones pasados dejaron de predecir el futuro. Un modelo aprendido es un modelo del pasado. Cuando el pasado deja de coincidir con el presente, el modelo sigue respondiendo como si nada hubiera cambiado.

**3. El volumen convirtió pequeños errores en grandes pérdidas.** Una tasa de error del 5% sobre diez casas es ruido. Una tasa de error del 5% sobre miles de casas compradas con dinero real es una catástrofe. Las tasas de error de la IA no escalan con buenos modales.

**4. Nadie pudo anularlo lo bastante rápido.** El sistema compraba casas de forma continua. Detener a una máquina que compra a gran escala es difícil, y para cuando la detienes, las compras ya están hechas.

Zillow conservó el Zestimate. Sigue siendo una función útil. Lo que dejó de hacer fue dejar que la suposición dirigiera un negocio. Esa es la lección honesta: **usa la IA para informar una decisión, no para que sea la decisión, hasta que hayas medido cómo se ve el error.**

## Cómo hacerlo

### Mapear la IA sobre tus propias herramientas

Haz esto con tu equipo, en una reunión, en una pizarra.

**Paso 1: Enumera cada herramienta que usa tu negocio.** Software, aplicaciones, sitios web, plataformas. Apunta a veinte o más.

**Paso 2: Marca cada una.** Tres marcas: **R** por solo basado en reglas, **A** por que usa IA, **?** por que no lo sabes.

**Paso 3: Trabaja las marcas ?.** Hazle al proveedor una pregunta: «¿Esto usa aprendizaje automático o un modelo, o es lógica fija?». Anota la respuesta. Ahora tienes un mapa de dónde la IA toca realmente tu negocio. La mayoría de las empresas se sorprenden. La mayoría encuentra IA en lugares que nadie eligió a propósito.

**Paso 4: Para cada A, escribe una línea.** ¿Qué decide? ¿Quién ve el resultado? ¿Quién lo revisa? Si la respuesta a «quién lo revisa» es «nadie», ese es tu primer riesgo a arreglar.

### Un guion de cinco frases para clientes y personal

Usa este guion. Funciona para clientes, personal y tu contable.

1. «Esto es un programa de ordenador que aprendió de muchos ejemplos pasados en lugar de seguir una lista fija de reglas».
2. «Es bueno en los casos comunes y menos bueno en los inusuales».
3. «Puede sonar seguro incluso cuando está equivocado».
4. «Una persona revisa los resultados importantes antes de que salgan».
5. «Siempre puedes pedir hablar con un ser humano en su lugar».

Di las cinco. No te saltes la frase 3. Es la que te protege más adelante.

### 2.7 Lo que la IA hace bien y lo que no puede hacer

**Lo que la IA hace bien.**

- **Juicio repetitivo.** Ordenar, etiquetar, resumir, redactar —el mismo tipo de decisión miles de veces.
- **Trabajar con entradas humanas desordenadas.** Letra a mano, erratas, frases raras, idiomas mezclados.
- **Encontrar patrones en grandes volúmenes.** Detectar la factura rara entre cincuenta mil.
- **Trabajar a cualquier hora, a cualquier escala.** Sin fatiga, sin mal humor, sin vacaciones.
- **Redactar rápido.** Un primer borrador en segundos, que una persona luego mejora.
- **Consistencia.** No se cansa ni deja de importarle en el caso cuatrocientos.

**Lo que la IA no puede hacer.**

- **Saber cuándo no sabe.** Responde. Esa es la limitación central.
- **Asumir responsabilidad.** No puede ser responsable, y no se le puede hacer que le importe.
- **Manejar situaciones genuinamente nuevas.** Si no estaba en los ejemplos, está adivinando a ciegas.
- **Ser fiablemente factual.** Produce lo que suena correcto. Verifica cualquier cosa que importe.
- **Entender el contexto de tu negocio.** No sabe que el cliente del pedido pequeño es el hermano de tu cliente más grande.
- **Decidir preguntas de valores.** Qué es justo, qué es amable, qué hacer cuando dos reglas chocan. Esas son tuyas.

Una regla simple: **la IA es muy buena en el primer 80% de una tarea y silenciosamente mala en el último 20%.** El último 20% es donde vive el riesgo, y no produce ningún mensaje de error.

## Ética y responsabilidad

Tres cosas de este capítulo, antes del tratamiento completo en [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md).

**Sé honesto sobre qué es.** Si un cliente está hablando con software, debería saberlo. No en una nota al pie. En la conversación.

**No le traslades la culpa a la máquina.** «La IA lo hizo» no es una defensa, ni ante clientes ni ante un regulador. Tú elegiste la herramienta, tú la configuraste, tú la dejaste correr. La responsabilidad se quedó contigo todo el tiempo.

**Vigila qué contiene ya tus datos.** La historia del taxista trata realmente de esto. Tus registros no son una foto neutral de tu negocio. Incluyen cada atajo, cada excepción concedida bajo presión, cada promesa educada hecha para cerrar una venta. Entrenar con ellos puede congelar y escalar esos comportamientos. Revisa los datos antes de entrenar con ellos, no después.

## Errores que evitar

### 2.8 Mitos, miedos y expectativas realistas

| Mito | Lo que es realmente cierto |
|---|---|
| «La IA entiende mi negocio». | Encontró patrones en ejemplos de tu negocio. No entiende nada en el sentido humano. |
| «La IA siempre tiene razón». | Tiene una tasa de error: baja en casos normales, alta en los extraños, y las respuestas equivocadas parecen normales. |
| «La IA reemplazará a mi personal». | Reemplaza tareas, no puestos enteros. La mayoría de los puestos son un conjunto de tareas, y solo algunas son automatizables. |
| «La IA es solo para grandes empresas». | Ya existen herramientas baratas y listas para usar. Las pequeñas empresas a menudo ganan más, porque tienen menos capas que cambiar. |
| «Si compro una herramienta de IA, ya tengo IA». | Tienes una herramienta. El valor viene del proceso que reconstruyes a su alrededor. |
| «Empieza ahora, arregla después». | Algunos errores son baratos de arreglar. Otros terminan una relación con un cliente o provocan un problema legal. Sabes cuál estás ejecutando. |
| «Más datos siempre es mejor». | Unos datos variados y relevantes superan a unos datos grandes y estrechos. |
| «La IA generativa es un buscador». | Predice texto probable. No consulta hechos. Verifica. |

**Expectativas realistas, dichas sin rodeos.** Espera buenos resultados en tareas repetitivas con ejemplos claros y una revisión humana. Espera un primer mes áspero; montar cualquier flujo de trabajo de IA lleva más tiempo del que sugiere la demostración. Espera decepciones de todo lo que requiera juicio, contexto o confianza. Espera que la herramienta cambie —la hoja de ruta del proveedor no es tu plan. Espera que las victorias sean pequeñas y concretas. Pequeño y concreto, repetido, es lo que de verdad se suma.

**Miedos que vale la pena tomar en serio:** poner el resultado de la IA frente a clientes sin revisarlo; entrenar con datos que no deberías tener; dejar que un proveedor se quede tus datos sin contrato; automatizar un mal proceso para que falle más rápido.

**Miedos que no quitan el sueño:** que las máquinas cobren conciencia y se vuelvan contra ti; que tu industria desaparezca en un año; necesitar un científico de datos antes de poder empezar.

## Ejercicio práctico

### 2.9 Reconoce la IA a tu alrededor

Haz esto a lo largo de un día de trabajo. Toma unos veinte minutos en total y es la forma más rápida de desarrollar ojo para la IA.

**Parte 1 — Atrápala en uso (10 minutos).** Durante el día, anota cada vez que un software tomó una decisión por ti en lugar de seguir una regla que tú fijaste. Para cada una, apunta: ¿qué herramienta era? ¿Qué decidió? ¿Podrías haber escrito tú la regla en una frase?

Esa última pregunta es la prueba. Si podías escribir la regla con facilidad, probablemente no era IA. Si no podías, probablemente sí lo era.

**Parte 2 — Audita tu propio negocio (10 minutos).** Enumera cinco tareas de tu negocio que hoy hace una persona por juicio. Para cada una, escribe:

1. ¿Cuántas veces por semana ocurre?
2. ¿Cuánto tiempo toma?
3. ¿Podrías mostrarle a un empleado nuevo 100 ejemplos terminados en lugar de explicarle las reglas?
4. ¿Cuál es el costo de equivocarse en una?

El punto 3 te dice si la IA podría hacerla. El punto 4 te dice con cuánto cuidado debes revisarla.

Donde el punto 3 es «sí» y el punto 4 es «bajo costo», tienes un buen primer candidato. Donde el punto 3 es «sí» y el punto 4 es «costo muy alto», tienes un candidato que necesita una persona en el bucle antes de ir a ninguna parte.

Guarda la lista. Se convierte en la materia prima para el trabajo de mapeo de procesos más adelante en el libro.

## Lista de verificación

### 2.10 Lo primero que debes saber

- [ ] Puedo decir en una frase qué es la IA: software que deduce de ejemplos en lugar de seguir reglas escritas.
- [ ] Puedo distinguir la automatización basada en reglas de la IA, y sé cuál necesito para una tarea dada.
- [ ] Entiendo que una respuesta de la IA es una suposición con una tasa de error, no una certeza.
- [ ] Sé que «aprender de datos» significa ajustar los valores hasta que las respuestas coincidan con los ejemplos.
- [ ] Sé que la calidad y la variedad de los ejemplos deciden la calidad del resultado.
- [ ] Puedo nombrar diez lugares donde la IA ya aparece en la vida diaria y en mi propio negocio.
- [ ] Puedo distinguir la IA generativa, un chatbot y un asistente virtual, y hago las tres preguntas sobre cualquier producto.
- [ ] Sé que la IA generativa es una buena escritora y no una fuente fiable.
- [ ] Sé que la IA es fuerte en el primer 80% de una tarea y silenciosamente débil en el último 20%.
- [ ] He comprobado si los datos de mi propio negocio contienen comportamiento deshonesto o descuidado antes de entrenar nada con ellos.
- [ ] Uso el guion de cinco frases al explicar la IA a clientes o personal.
- [ ] Sé que la responsabilidad por el resultado de la IA se queda conmigo, siempre.

## Puntos clave

- La única distinción que realmente necesitas es de dónde vinieron las instrucciones: las escribió una persona, o la máquina las dedujo de ejemplos.
- Pregunta si una tarea tiene forma de regla o forma de juicio antes de elegir entre la automatización normal y la IA.
- La IA es una muy buena escritora y no una fuente fiable; suena segura esté en lo cierto o equivocada.
- La IA es fuerte en el primer 80% de una tarea y silenciosamente débil en el último 20%, que es exactamente donde se sienta el riesgo.
- Los datos de entrenamiento llevan consigo la deshonestidad y los atajos humanos, así que revisa tus registros antes de entrenar con ellos.
