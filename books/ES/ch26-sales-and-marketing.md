# Capítulo 26 — Ventas y marketing

## En palabras simples

Las ventas y el marketing son donde la IA puede ayudarte a encontrar más clientes, hablar con ellos mejor y gastar menos tiempo adivinando. El trabajo aquí está lleno de pequeñas tareas repetidas: clasificar qué contactos merecen una llamada, escribir correos, responder las mismas preguntas en tu sitio web, e intentar entender qué quieren tus clientes. La IA es buena en todas ellas.

La idea central es la *personalización a escala*. Un buen vendedor recuerda a cada cliente, adapta el mensaje y hace seguimiento en el momento justo. Un equipo pequeño no puede hacer eso con miles de personas. La IA sí. Puede mirar cada contacto y adivinar qué probable es que compre, escribir un correo que suene como si estuviera escrito para esa persona, responder la pregunta de un visitante a las 2 de la madrugada, y detectar qué clientes están a punto de irse.

Este capítulo cubre cuatro trabajos: puntuar contactos (adivinar quién es más probable que compre), escribir correos y contenido, gestionar chatbots y asistentes, y analizar clientes para entender qué quieren y quién está en riesgo de irse.

Una advertencia honesta antes de empezar: la IA es un potente amplificador. Hará que un buen mensaje llegue a más gente, y hará que un mal mensaje llegue a más gente también. También puede empujarte al spam —enviar demasiado, demasiado a menudo, a gente que no lo pidió. El objetivo no es ametrallarlo todo; es llegar a la persona correcta con el mensaje correcto en el momento correcto. El método para juzgar si todo esto da dinero vive en el [Capítulo 16 — Objetivos, costos y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md); este capítulo te muestra qué automatizar y cómo.

## Un poco de historia

**Años 1990: marketing masivo y la lista de correo.** La automatización de marketing empezó con simples listas de correo. Un negocio podía enviar un mensaje a miles de personas a la vez. Era barato y amplio, pero tosco —todos recibían el mismo mensaje, encajara con ellos o no. Esta fue la era de "rociar y rezar."

**Años 2000: el CRM y el embudo.** Llegó el software de Gestión de Relaciones con Clientes (CRM) —una base de datos de cada cliente y cada interacción—. Los marketers empezaron a pensar en un "embudo": muchas personas entran por arriba, menos llegan a una compra por abajo. El CRM dejaba rastrear dónde estaba cada persona en el embudo y hacer seguimiento. Los datos entraron en el cuadro.

**Años 2010: segmentación y personalización.** Con más datos, los marketers aprendieron a dividir su audiencia en grupos (segmentos) y enviar a cada grupo un mensaje distinto. "La gente que compró X también compró Y." La personalización hizo los mensajes más relevantes y más eficaces. Pero seguía siendo sobre todo basada en reglas: si un cliente hacía esto, envía aquello.

**Finales de los 2010: el aprendizaje automático puntúa contactos.** El aprendizaje automático —software que aprende patrones de muchos ejemplos— empezó a puntuar contactos. En vez de que una persona adivinara a quién llamar primero, el modelo miraba cientos de señales (tamaño de la empresa, qué páginas visitaron, cómo te encontraron) y ordenaba los contactos por lo probables que eran de comprar. Los equipos de ventas dejaron de perder tiempo en contactos fríos.

**Años 2020: la IA generativa escribe y chatea.** Los grandes modelos de lenguaje —IA entrenada con enormes cantidades de texto— ahora pueden escribir correos, textos publicitarios y descripciones de producto que suenan humanos. Los chatbots construidos sobre la misma tecnología pueden mantener una conversación real, responder preguntas y guiar a un cliente a través de una compra. El chatbot pasó de una frustrante lista de botones a algo que realmente entiende lo que escribiste.

**Ahora: agentes que trabajan todo el recorrido.** El paso más nuevo es el agente —IA que lleva una tarea a través de varios pasos. Un agente de cara al cliente puede responder una pregunta, comprobar stock y guiar una compra. Un agente interno puede tomar una solicitud de soporte y crear el ticket. El ejemplo de mobilezone más abajo usa exactamente esto: dos agentes, uno para clientes y otro para el equipo interno.

El arco: de un mensaje para todos, a embudos rastreados, a segmentos, a contactos puntuados, a IA que escribe y chatea. Cada paso hizo el marketing más personal y menos un juego de adivinar.

## Curiosidad

### 26.5 El chatbot que se convirtió en dos agentes

Cuando mobilezone, un minorista suizo de telecomunicaciones, reemplazó su viejo chatbot, no construyó un bot mejor. Construyó dos agentes distintos para dos trabajos distintos: uno de cara a los clientes, otro de cara a su propio personal. Esa división es la idea interesante. La misma tecnología de IA sirvió a dos audiencias de dos maneras muy distintas —una guía de compras amigable en el sitio web, y un ayudante de tickets dentro de la empresa—. La historia, con los números reales, está más abajo.

## Un ejemplo real de negocio

**mobilezone: dos agentes de Copilot, uno para clientes y otro para TI.**

mobilezone es un minorista suizo de telecomunicaciones con más de 125 tiendas físicas, que vende teléfonos, planes y dispositivos conectados. Tenía dos problemas separados. Del lado del cliente, su viejo chatbot del sitio web era rígido y frustrante —solo podía seguir una lista fija y a menudo fallaba al responder preguntas reales. Dentro de la empresa, el personal tenía que rellenar formularios engorrosos para reportar problemas de TI, lo que ralentizaba a todos.

Según un caso de cliente publicado por Microsoft, mobilezone reconstruyó ambos lados usando Microsoft Copilot Studio —una herramienta para construir agentes de IA conversacionales— junto con Dynamics 365 (su CRM) y la Power Platform (las herramientas de automatización de bajo código de Microsoft). Construyó dos agentes:

- **Mia —el agente de cara al cliente.** Mia es un asistente multilingüe en el sitio web. Responde preguntas de gran volumen de clientes, ayuda a los visitantes a encontrar el producto o plan adecuado, y los guía a través de una compra. Como entiende el lenguaje natural, maneja las preguntas que el viejo bot de lista no podía.
- **Supporto —el agente interno de TI.** Supporto es un ayudante para el propio personal de mobilezone. En vez de rellenar un formulario rígido, un empleado le dice a Supporto qué está roto en palabras simples, y el agente crea el ticket de TI automáticamente.

Los resultados reportados: los agentes ahora gestionan **más de 1.600 chats al mes**, y el agente interno de TI **recortó el tiempo de resolución de TI en cerca de un 50%**. Igualmente importante, los agentes redujeron la carga del centro de contacto externo de mobilezone (el soporte telefónico subcontratado), y el agente de clientes mejoró la conversión en línea guiando a los compradores a través del descubrimiento de productos.

Dos lecciones destacan. Primera, la misma tecnología sirvió a dos trabajos muy distintos —ventas externas y soporte interno—, lo que muestra lo flexibles que son estos agentes. Segunda, mobilezone no reemplazó humanos; movió las conversaciones fáciles y repetitivas al agente para que su gente pudiera enfocarse en las más difíciles. Esa es la promesa realista: la IA maneja el volumen, los humanos manejan el valor.

Una nota sobre la fuente: las cifras de arriba vienen de la historia de cliente de Microsoft sobre mobilezone. Trátalas como los resultados reportados por mobilezone; tus propios números dependerán de tu volumen y configuración.

## Cómo hacerlo

### 26.1 Puntuación de contactos

Un *contacto* (lead) es una persona o empresa que ha mostrado algo de interés —rellenó un formulario, descargó algo, o hizo una pregunta—. No tienes tiempo para llamar a cada contacto con el mismo esfuerzo. La puntuación de contactos significa ordenar los contactos por lo probables que son de comprar, para que tu equipo llame a los más calientes primero.

**Cómo puntúa la IA a un contacto.** Un modelo de aprendizaje automático mira muchas señales a la vez: el tamaño de la empresa del contacto, el cargo de la persona, qué páginas visitó, cuántas veces volvió, si abrió tus correos, y cómo te encontró. A partir de acuerdos pasados que se cerraron, el modelo aprende qué señales van juntas con una venta, y puntúa cada nuevo contacto en consecuencia.

**Por qué supera a adivinar.** Una persona puntuando contactos por corazonada es lenta y sesgada —tiende a favorecer los contactos que "se sienten" amigables, no los que realmente convierten. La IA puntúa de forma consistente y rápida, y puede sopesar cientos de señales que una persona no puede sostener en su cabeza.

**Empieza simple.** No necesitas un modelo perfecto el primer día. Empieza con unas pocas señales claras —tamaño de empresa, rol, y qué descargaron— y puntúa contactos a mano en tu CRM. A medida que recolectes más acuerdos cerrados, un modelo real puede aprender de ellos y mejorar.

**Alimenta el bucle.** El modelo mejora cuando le dices qué contactos realmente se volvieron clientes. Asegúrate de que tu CRM registre el resultado de cada acuerdo, para que la puntuación aprenda de resultados reales, no de suposiciones.

**No te fíes demasiado de la puntuación.** Una puntuación es una pista, no un veredicto. Una puntuación alta significa "llama pronto," no "venta garantizada." Una puntuación baja puede seguir siendo un buen cliente que el modelo aún no ha aprendido. Usa la puntuación para fijar prioridad, no para ignorar personas.

### 26.2 Correo y contenido

Escribir correos, textos publicitarios y descripciones de producto lleva horas. La IA generativa —IA que produce texto— puede redactarlos rápido, y una persona puede editarlos para que suenen bien.

**Redacta, no envíes.** Usa la IA para producir un primer borrador, y luego edítalo. La IA es excelente poniendo palabras en la página rápido y pésima sabiendo tu voz exacta, tu marca y los sentimientos de tu cliente sin guía. El borrador está al 70% ahí; tu edición es el último 30% que lo hace tuyo.

**Personaliza a escala.** La IA puede tomar una plantilla y adaptarla para muchas personas: insertar el nombre del destinatario, referirse a lo que miraron, adaptar la oferta a su segmento. Esta es la idea de personalización a escala de antes —un mensaje que se siente escrito para una persona, enviado a miles.

**Adapta el canal.** Un correo, una publicación social y una página de producto necesitan distintas longitudes y tonos. Di a la IA el canal y el objetivo, y edita en consecuencia. Un correo largo no funciona como tuit; un tuit no funciona como página de aterrizaje.

**Conserva la voz humana.** El texto de IA puede sonar plano, genérico o demasiado ansioso. Lee cada borrador en voz alta. Si no suena a algo que tú dirías, reescríbelo. Tus clientes notan cuando un mensaje es genérico.

**Nunca dejes que la IA envíe sin revisión.** Un correo de IA sin revisar puede contener un precio erróneo, un nombre equivocado, o una línea inapropiada. Ten siempre a un humano leyéndolo antes de que salga. Esta es la misma regla que en finanzas: la IA redacta, el humano aprueba.

**Vigila el volumen.** La IA hace fácil enviar más correos de los que deberías. Más no es mejor. Enviar demasiado a gente que no lo pidió es spam, y quema tu lista y tu reputación. Envía menos, pero haz que cada uno cuente.

### 26.3 Chatbots y asistentes

Un chatbot es un programa que habla con un cliente en tu sitio web o app. Los chatbots modernos, construidos sobre grandes modelos de lenguaje, entienden lo que una persona escribe y responden en lenguaje simple —un gran salto desde las viejas listas de "pulse 1 para ventas."

**Qué hace un buen chatbot.** Responde preguntas comunes al instante (precio, horario, envíos, devoluciones), guía a un visitante al producto correcto, captura datos de contacto para un seguimiento, y pasa a un humano cuando no puede ayudar. El traspaso es crítico: un chatbot que nunca pasa a alguien frustra a la gente y pierde ventas.

**Diseña el traspaso primero.** Antes de construir el bot, decide cuándo debe pasar la conversación a una persona. Cuando el bot no está seguro, cuando el cliente pide un humano, cuando el tema es delicado —pasa. Un bot que conoce sus límites es confiable; uno que farolea, no.

**Entrénalo con tus preguntas reales.** Dale al bot las preguntas que los clientes realmente hacen, con las respuestas que quieres. Cuanto más sepa tus productos y políticas específicos, más útil es. Un bot genérico da respuestas genéricas que frustran.

**Deja que hable muchos idiomas.** Una de las mayores victorias de un chatbot moderno es el soporte multilingüe. Puede responder a un cliente en su propio idioma sin que contrates traductores. Esto es exactamente lo que hace Mia de mobilezone.

**Mide qué gestiona y qué falla.** Rastrea cuántas conversaciones resuelve el bot por su cuenta, cuántas pasa, y qué no pudo responder. Los fallos son oro —te dicen qué enseñarle después. (Las mismas ideas de chatbot, aplicadas al soporte en vez de a las ventas, se tratan en el [Capítulo 27 — Atención y soporte al cliente](ch27-customer-care-and-support.md).)

### 26.4 Análisis de clientes

El análisis de clientes significa usar datos para entender quiénes son tus clientes, qué quieren, y quién está a punto de irse. La IA es fuerte aquí porque puede ver patrones a través de miles de clientes que ninguna persona podría detectar a mano.

**Segmenta tus clientes.** La IA puede agrupar clientes por comportamiento: compradores frecuentes, grandes gastadores, compradores estacionales, clientes en riesgo. Cada grupo necesita un mensaje distinto. Esto es la segmentación, y la IA la hace más rápido y con más precisión que las reglas manuales.

**Detecta el abandono antes de que ocurra.** *Abandono* (churn) significa que un cliente deja de comprar. La IA puede mirar señales —menos visitas, pedidos más pequeños, menos implicación— y marcar clientes que probablemente se vayan pronto. Eso te da tiempo para recuperarlos con una oferta o una llamada personal, en vez de enterarte después de que se fueron.

**Encuentra la siguiente mejor oferta.** La IA puede mirar qué compró un cliente y sugerir qué es probable que quiera después. "Compró un teléfono, probablemente necesita una funda y un seguro." Esta es la idea del motor de recomendaciones, y eleva el valor de cada cliente.

**Lee lo que dicen los clientes.** La IA puede leer reseñas, comentarios de encuestas y chats de soporte y extraer los temas principales: qué les encanta, qué les molesta, qué piden. En vez de leer mil comentarios uno por uno, obtienes un resumen de los grandes temas. Esto convierte el comentario bruto en algo sobre lo que puedes actuar.

**No trates a las personas como puntos de datos.** El análisis es una herramienta para servir mejor a los clientes, no para manipularlos. Usa lo que aprendes para mejorar su experiencia, no para explotar sus debilidades. La línea entre personalización y manipulación es real, y debes mantenerte en el lado correcto.

## Ética y responsabilidad

Las ventas y el marketing tocan la atención y la confianza de las personas directamente, así que la línea ética importa.

**No hagas spam.** La IA hace fácil enviar demasiado. Enviar mensajes a gente que no los pidió, o más de lo que acordaron, es spam. Respeta el consentimiento y la frecuencia. Una lista corta de gente que quiere tus mensajes vence a una lista enorme que ametrallas.

**Sé honesto en el texto escrito por IA.** La IA puede escribir una afirmación que suena verdad pero no lo es. Comprueba cada afirmación factual —precio, funciones, resultados— antes de que se envíe. Nunca dejes que la IA invente un beneficio que no puedas entregar.

**Divulga cuando es un bot.** En muchos lugares, y como buena práctica, un cliente debe saber que está hablando con un chatbot y no con una persona. Haz que el traspaso a un humano sea fácil y claro.

**Respeta la privacidad.** El análisis de clientes usa datos personales. Sigue las reglas para manejarlos —lo básico está en el [Capítulo 10 — Privacidad y GDPR](ch10-privacy-and-gdpr.md). Recoge solo lo que necesitas, di a la gente qué recoges, y mantenlo seguro.

**No manipules.** La personalización debe ayudar a la gente a encontrar lo que quiere, no empujarlos a una compra de la que se arrepentirán. Evita los patrones oscuros —trucos que presionan a las personas. Construye confianza, no una trampa.

**Mantén un humano en el bucle.** La IA redacta el correo, el anuncio, la respuesta. Un humano lo revisa antes de que llegue a un cliente. Esta sola regla previene la mayor parte del daño.

## Errores a evitar

**Hacer spam con IA.** Usar el poder de la herramienta para enviar más de lo que la gente quiere. Envía menos, haz que cuente.

**Enviar texto de IA sin revisar.** Un precio erróneo o una afirmación falsa en un correo escrito por IA daña la confianza. Revisa siempre.

**Un chatbot que nunca pasa a un humano.** Un bot que farolea en vez de pasar a un humano frustra a los clientes y pierde ventas. Diseña el traspaso primero.

**Texto genérico y plano.** Texto de IA que suena como el de todos los demás. Edítalo para tu voz o será ignorado.

**Fiarse demasiado de la puntuación de contactos.** Tratar una puntuación como un veredicto en vez de una pista. Úsala para fijar prioridad, no para ignorar personas.

**Basura entra, basura sale en el análisis.** Si tus datos del CRM están desordenados, los segmentos y las marcas de abandono están mal. Limpia tus datos primero.

**Tratar a los clientes como puntos de datos.** Usar el análisis para manipular en vez de servir. Mantente en el lado ético.

**Sin divulgación de los bots.** Dejar que un chatbot finja ser humano. Sé claro.

**Ignorar las reglas de privacidad.** Usar datos personales sin consentimiento o seguridad. Sigue lo básico del GDPR.

**Confundir actividad con resultados.** Contar correos enviados en vez de acuerdos cerrados. Mide resultados, no volumen.

**Saltarte la línea base.** No medir la conversión antes, así que no puedes probar la mejora. Mide primero (mira el Capítulo 22).

**Reemplazar por completo el trato humano.** Los clientes aún quieren una persona para los problemas difíciles. Mantén humanos para las conversaciones de valor.

## Ejercicio práctico

### 26.7 Ejercicio: planifica una campaña asistida por IA

Elige una campaña —un correo a clientes pasados, un chatbot en tu sitio, o una pasada de puntuación de contactos— y planifícala de principio a fin.

**Paso 1 — Elige el trabajo.** Elige uno: puntuación de contactos, una campaña de correo, un chatbot, o un análisis de clientes. Haz uno, no todos.

**Paso 2 — Define el objetivo y la métrica.** ¿Qué debe lograr esto? ¿Registros, respuestas, preguntas resueltas, clientes recuperados? Elige un número para medir.

**Paso 3 — Mide la línea base.** ¿Cuál es ese número ahora? Anótalo. Sin él no puedes probar la mejora.

**Paso 4 — Reúne los datos.** Para puntuación: tus contactos pasados y cuáles se cerraron. Para correo: tu lista con consentimiento. Para el chatbot: tus preguntas y respuestas reales de clientes. Para análisis: tus registros de clientes. Limpia los datos primero.

**Paso 5 — Construye la parte de IA.** Puntúa los contactos, redacta el correo, entrena el bot, o ejecuta la segmentación. Deja que la IA haga el trabajo pesado.

**Paso 6 — Añade la revisión humana.** Lee cada borrador. Comprueba cada afirmación factual. Decide las reglas de traspaso del chatbot. Nada se envía sin una lectura humana.

**Paso 7 — Revisa el consentimiento y la privacidad.** Confirma que tienes permiso para mensajear a esta gente y que sus datos se manejan correctamente.

**Paso 8 — Lanza en pequeño y mide.** Ejecútalo primero en un grupo pequeño. Compara la métrica con la línea base. Si funciona, escala. Si no, aprende y ajusta.

Haz una campaña bien. Las lecciones que aprendas —sobre el tono, sobre los traspasos, sobre qué responde tu cliente— se llevan a cada campaña posterior.

## Lista de verificación

### 26.8 Lista de verificación de ventas y marketing

Antes de lanzar cualquier actividad de ventas o marketing asistida por IA, revisa esto.

- [ ] **Mediste la línea base** de la única métrica que te importa.
- [ ] **Un humano revisa cada mensaje escrito por IA** antes de que llegue a un cliente.
- [ ] **Cada afirmación factual está comprobada** —precio, funciones, resultados.
- [ ] **Tienes consentimiento** para mensajear a la gente que estás mensajeando.
- [ ] **Respetas la frecuencia** —sin spam, sin exceso de envíos.
- [ ] **El chatbot tiene reglas claras de traspaso** a un humano.
- [ ] **El chatbot está entrenado con tus preguntas reales**, no genéricas.
- [ ] **Divulgas que es un bot** donde se requiere y como buena práctica.
- [ ] **Limpies tus datos** antes de puntuar, segmentar o analizar.
- [ ] **Retroalimentas los resultados** al modelo de puntuación de contactos para que aprenda.
- [ ] **Tratas la puntuación de contactos como una pista**, no un veredicto.
- [ ] **Usas el análisis para servir a los clientes**, no para manipularlos.
- [ ] **Sigues las reglas de privacidad** (lo básico del GDPR, mira el Capítulo 10).
- [ ] **Mantienes humanos para las conversaciones difíciles.**
- [ ] **Mides resultados** (acuerdos, respuestas, victorias), no solo volumen enviado.
- [ ] **Lanzas en pequeño primero** y escalas solo lo que se demuestra.

Si una casilla está vacía, estás arriesgando confianza. Rellénala antes de pulsar enviar.

## Puntos clave

- La IA ayuda a ventas y marketing personalizando a escala —puntuando contactos, adaptando mensajes, respondiendo preguntas y detectando clientes en riesgo.
- El caso de mobilezone (una historia de cliente de Microsoft) construyó dos agentes de Copilot Studio —Mia para clientes, Supporto para TI interna— gestionando más de 1.600 chats al mes y recortando el tiempo de resolución de TI en cerca de un 50%.
- La IA redacta, un humano revisa: nunca envíes un mensaje escrito por IA ni dejes que un chatbot farolee en vez de pasar a una persona.
- Los datos limpios son la base —los registros desordenados hacen que las puntuaciones de contactos, los segmentos y las marcas de abandono estén mal.
- Usa la IA para servir mejor a los clientes, no para spamearlos o manipularlos; el consentimiento y la honestidad protegen la confianza sobre la que vendes.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Convierte una idea en una propuesta

![Un documento de propuesta de proyecto estructurado](../../assets/examples/project-proposal.png)
*Un documento de propuesta de proyecto estructurado*

**Lo que pides:** `Crea una propuesta de proyecto para una pequeña tienda en línea: objetivos, qué entregamos, un calendario de 8 semanas, y un precio de 9.500 euros.`

El agente construye una propuesta con el objetivo del cliente, tu solución, los entregables, el calendario y el precio —todo en un diseño limpio que parece que llevó toda una tarde. Le llevó un minuto.

*Consejo: Añade tu logo y una frase sobre resultados pasados para que se sienta personal.*

---

### Rastrea tus ventas

![Un rastreador de ventas con ingresos por canal](../../assets/examples/sales-tracker.png)
*Un rastreador de ventas con ingresos por canal*

**Lo que pides:** `Crea un rastreador de ventas con mes, canal e ingresos, y un gráfico de ingresos por canal.`

El agente construye el rastreador y el gráfico. Añade filas a medida que avanzas, o adjunta tu lista bruta de ventas y pídele que te rellene la hoja.

*Consejo: Adjunta una exportación desordenada de tu tienda y di 'limpia esto en un rastreador' —lo hará.*

---

### Una presentación de pitch de un solo prompt

![Una diapositiva de presentación construida por el agente](../../assets/examples/pitch-deck.png)
*Una diapositiva de presentación construida por el agente*

**Lo que pides:** `Haz una presentación de pitch de 6 diapositivas para mi startup de entregas: problema, solución, mercado, modelo, tracción, petición.`

El agente diseña las diapositivas con un look limpio, una idea clara por diapositiva, y el orden correcto para un pitch. En el navegador pulsas F11 para pantalla completa y presentas.

*Consejo: ¿Necesitas un .pptx real para enviar? Usa /tools office-files y pide PowerPoint.*

---

### Una presentación de ventas para un cliente

![Una diapositiva de presentación de ventas de cara al cliente](../../assets/examples/sales-presentation.png)
*Una diapositiva de presentación de ventas de cara al cliente*

**Lo que pides:** `Crea una presentación de ventas resumiendo nuestro trabajo con Acme y proponiendo la siguiente fase.`

El agente construye una presentación enfocada: resultados hasta ahora, qué ganó el cliente, y el siguiente paso propuesto. Ajustas los números y presentas con confianza.

*Consejo: Adjunta el informe del proyecto y el agente saca los puntos destacados a las diapositivas.*

---

### Un seguimiento educado

![Un borrador de correo de seguimiento amigable](../../assets/examples/follow-up.png)
*Un borrador de correo de seguimiento amigable*

**Lo que pides:** `Escribe un breve seguimiento a un cliente que no ha respondido a nuestra cotización de la semana pasada.`

El agente escribe un toque ligero y educado que recuerda sin presión. Lo envías y mantienes la relación tibia.

*Consejo: Un seguimiento programado puede enviar estos por ti si no ha llegado una respuesta.*

---

### Un boletín de clientes

![Un borrador de boletín listo para enviar](../../assets/examples/newsletter.png)
*Un borrador de boletín listo para enviar*

**Lo que pides:** `Escribe un boletín mensual para nuestros clientes: novedades, un consejo, y un pequeño código de descuento.`

El agente escribe el boletín en tu voz con las noticias, un consejo útil y la oferta. Envíalo, o deja que prepare uno según un calendario.

*Consejo: Una tarea mensual programada puede redactar el boletín para tu revisión cada vez.*

---

### Convierte un tema en un pódcast

![Un episodio de pódcast listo para reproducir](../../assets/examples/podcast-episode.png)
*Un episodio de pódcast listo para reproducir*

**Lo que pides:** `Crea un episodio de pódcast de 5 minutos sobre por qué las pequeñas tiendas deberían pasarse en línea, en un estilo amigable de dos voces.`

El agente escribe el guion y produce un episodio de audio con dos voces, listo para publicar. Tu mensaje, en forma de audio, sin estudio.

*Consejo: Dale tus puntos clave y los da forma en una conversación natural.*

<!-- END agentbridge-examples -->
