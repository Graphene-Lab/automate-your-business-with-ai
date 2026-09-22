# Capítulo 30 — TI y liderazgo

## En palabras simples

TI y liderazgo son dos mitades de un mismo trabajo: mantener el negocio funcionando y dirigirlo en la dirección correcta. TI mantiene los sistemas, los datos y la red funcionando y seguros. El liderazgo convierte todo eso en decisiones —dónde invertir, qué arreglar primero, qué riesgo tomar—. La IA ayuda a ambas mitades. Responde las preguntas rutinarias de TI, vigila amenazas, construye los reportes, y expone las opciones para que un líder elija bien.

Piensa en TI como la fontanería y la seguridad de un edificio, y el liderazgo como las personas que deciden a dónde va el edificio después. Cuando la fontanería gotea, todos lo sienten. Cuando la puerta de seguridad se queda abierta, todos están expuestos. Y cuando los líderes tienen que decidir sin una imagen clara, adivinan. La IA parchea las fugas más rápido, vigila las puertas, y da a los líderes una imagen clara para decidir.

Este capítulo cubre cuatro trabajos: soporte interno (ayudar al personal con su tecnología), ciberseguridad (defender contra ataques), reportes de gestión (convertir datos en una imagen clara), y soporte a la decisión (exponer las opciones para un líder). Cada uno es un lugar donde un pequeño negocio puede funcionar más fluido, mantenerse más seguro, y decidir mejor.

Una idea honesta primero: la IA en TI y liderazgo es un *copiloto*, no el *capitán*. Responde, vigila, resume y sugiere. Una persona sigue tomando la decisión —si apagar un sistema, en qué proveedor confiar, qué riesgo aceptar—. Cuanto mayor la decisión, más importa el juicio humano. El método para juzgar si nada de esto da frutos vive en el [Capítulo 16 — Objetivos, Costes y Retorno de la Inversión](ch16-goals-costs-and-return-on-investment.md); este capítulo te muestra qué automatizar y cómo. Para ver dónde se sientan TI y liderazgo en el mapa de impacto y esfuerzo de todo tu negocio, mira el [Capítulo 12 — Dónde puede ayudar la IA a tu negocio](ch12-where-ai-can-help-your-business.md).

## Un poco de historia

**Años 80 y 90: el help desk.** El soporte de TI empezó como el help desk —un número de teléfono que el personal llamaba cuando algo se rompía—. Una persona registraba el problema, arreglaba lo que podía, y escalaba el resto. Funcionaba, pero era lento, y las mismas preguntas simples —contraseñas olvidadas, problemas de impresora— se comían la mayor parte del día.

**Años 90 y 2000: paneles e inteligencia de negocio.** Las empresas empezaron a tirar datos a paneles y herramientas de inteligencia de negocio —software que convierte números crudos en gráficos y resúmenes—. Por primera vez, un gerente podía ver ventas, costes y rendimiento en una pantalla. Pero construir esos reportes seguía necesitando un analista, y solo podías ver lo que el reporte estaba construido para mostrar.

**Años 2000: monitorización de seguridad automatizada.** A medida que crecieron los ataques, TI añadió herramientas de seguridad automatizadas —cortafuegos, detección de intrusos y sistemas de alerta que vigilan la red por actividad sospechosa—. Estas atrapaban más de lo que un humano podía, pero también producían una inundación de alertas, la mayoría inofensivas, y un analista cansado tenía que separar la amenaza real del ruido.

**Años 2010: el aprendizaje automático lee la amenaza.** El aprendizaje automático —software que aprende patrones de muchos ejemplos— cambió la seguridad. En vez de hacer coincidir firmas de ataque conocidas, la IA aprendió cómo se veía lo "normal" en la red y marcó lo inusual. Atravesó el ruido de alertas al detectar las pocas señales que realmente importaban.

**Años 2020: los grandes modelos de lenguaje responden y asesoran.** Los grandes modelos de lenguaje —IA entrenada con enormes cantidades de texto— ahora pueden responder la pregunta de TI de un empleado en lenguaje claro, resumir un incidente de seguridad, construir un reporte de gestión desde datos crudos, y exponer las opciones y compensaciones para la decisión de un líder. Este es el paso más nuevo: IA que lee, explica y asesora en los cuatro trabajos a la vez. El ejemplo de riesgo de proveedor de IBM más abajo muestra la misma idea aplicada a decidir qué proveedores son seguros.

El arco: de un help desk por teléfono, a paneles, a alertas automatizadas, a IA que lee la amenaza y responde la pregunta, a IA que asesora la decisión. Cada paso movió el trabajo rutinario al software y dejó a los humanos decidir y liderar.

## Curiosidad

### 30.5 El problema más antiguo del líder: decidir sin una imagen clara

Desde que hay gerentes, ha existido la misma queja: "Tengo que decidir, pero no puedo ver con claridad." Los datos están dispersos por sistemas. El reporte tarda una semana en construirse. El panel muestra el mes pasado, no hoy. Así que los líderes deciden por corazonada y esperanza.

La IA cambia eso más que casi cualquier otra cosa en este libro. Puede reunir los datos dispersos, construir la imagen bajo demanda, y responder la pregunta de un líder en palabras claras en segundos —"¿Qué línea de producto está perdiendo dinero?", "¿Dónde está nuestro efectivo el mes que viene?", "¿Qué proveedor es el mayor riesgo?"—. El líder sigue decidiendo. Pero ahora decide con una imagen clara en vez de una suposición. Esa es la revolución silenciosa en el liderazgo: no la IA tomando la decisión, sino la IA haciendo la decisión *informada*. La historia de riesgo de proveedor de IBM más abajo es exactamente esto, aplicada a una decisión difícil —¿en qué proveedores podemos confiar?—.

## Un ejemplo real de negocio

**IBM: evaluación de riesgo de terceros (proveedor) asistida por IA.**

Toda empresa que compra a proveedores externos carga *riesgo de terceros* —el riesgo de que un proveedor del que dependas resulte ser poco fiable, inseguro o incumplidor—. Comprobar cada proveedor es trabajo lento y cuidadoso. Una forma común de comprobar es un cuestionario detallado que el proveedor rellena, que luego un evaluador humano lee y puntúa. Cuando tienes cientos de proveedores, ese trabajo se vuelve un cuello de botella.

IBM Client Engineering publicó un trabajo real sobre esto, llamado "Evaluating Third Party Risk with AI." El cliente era una institución financiera que ejecutaba **más de 1.000 evaluaciones de proveedores al año**, y cada evaluación tomaba **unas 45 horas de trabajo** en completarse —leer el cuestionario, comprobar la evidencia, y puntuar el riesgo—. Eso es una enorme cantidad de tiempo cualificado gastado en la misma tarea cuidadosa, una y otra vez.

IBM usó su plataforma watsonx.ai para asistir a los evaluadores. La IA leía las respuestas del cuestionario del proveedor y la evidencia de apoyo, y ayudaba al evaluador a entender la calidad de lo que el proveedor había proporcionado, para que el humano pudiera enfocarse en el juicio en vez de leerlo todo desde cero. La estimación publicada fue **una reducción de unos 20% en el tiempo de evaluación**, lo que a lo largo de esa carga de trabajo se sumaba a **aproximadamente 10.000 horas de trabajo ahorradas** y **alrededor de $800.000 en coste de mano de obra al año**.

Una nota sobre la cifra del "50%". Puedes ver este tipo de trabajo de riesgo de proveedor de IBM citado como "una reducción de unos 50% en el tiempo." Ese número **no** es lo que reporta el caso publicado de IBM. La estimación publicada para este trabajo es de unos 20%, con los ahorros expresados como ~10.000 horas y ~$800k al año. Trata el "50%" como no verificado, y usa las cifras publicadas —~20% de reducción de tiempo, ~10.000 horas, ~$800k— como los números reales y con fuente. (Fuente: IBM Client Engineering, "Evaluating Third Party Risk with AI.")

Dos cosas vale la pena notar. Primero, el evaluador humano se mantuvo al mando. La IA no aprobó ni rechazó un proveedor; ayudó al humano a leer más rápido y juzgar mejor. Segundo, el ahorro vino de la parte de *lectura y comprobación* del trabajo —la lectura lenta y cuidadosa en la que la IA es buena— mientras que la *decisión* sobre el proveedor se quedó con la persona. Ese es el patrón a copiar en tu propio trabajo de riesgo: deja que la IA haga la lectura, guarda al humano para el juicio.

## Cómo hacerlo

### 30.1 Soporte interno

Soporte interno significa ayudar a tu propio personal con su tecnología —la contraseña olvidada, la impresora que no funciona, el software que necesita configurarse—. Es el help desk, y está lleno de las mismas preguntas repetidas. La IA es muy buena con las preguntas repetidas.

**El asistente de help desk de TI.** Un chatbot entrenado con tu propia base de conocimiento de TI puede responder preguntas del personal al instante: "¿Cómo me conecto a la VPN?", "¿Cómo restablezco mi contraseña?", "¿Cómo instalo esta aplicación?" Esto elimina los tickets rutinarios que se comen el día de un equipo de soporte, para que el equipo pueda enfocarse en los problemas reales.

**Resuelve los simples automáticamente.** Algunos tickets necesitan una acción simple —restablecer una contraseña, desbloquear una cuenta, reinstalar una aplicación—. La IA puede hacer esto automáticamente o redactar la acción para que un humano la apruebe. El trabajo rutinario desaparece de la cola.

**Enruta los difíciles rápido.** Cuando el bot no puede resolverlo, debería pasar el ticket a la persona correcta con el contexto intacto —lo que el miembro del personal ya dijo y probó— para que el humano no empiece de cero. Un traspaso limpio es la función más importante.

**Construye desde tus propios tickets.** Saca los últimos meses de tickets de TI y encuentra las preguntas más comunes. Esas se vuelven la base de conocimiento del bot. La misma tecnología de chatbot, aplicada a clientes en vez de personal, se trata en el [Capítulo 27 — Atención y Soporte al Cliente](ch27-customer-care-and-support.md); aquí se gira hacia adentro para servir a tu propio equipo.

**Guarda un humano para el problema difícil.** La IA maneja lo rutinario; una persona maneja la caída, el bicho extraño, el incidente de seguridad. Nunca dejes que un bot sea el único camino cuando algo está genuinamente roto. El personal siempre debe poder llegar a un humano.

### 30.2 Ciberseguridad

Ciberseguridad significa defender tus sistemas, datos y red de ataques. La IA es ahora una herramienta central en ambos lados de esta lucha —los defensores la usan para detectar amenazas, y los atacantes también la usan—, así que importa que entiendas qué puede y qué no puede hacer por ti.

**La IA detecta lo inusual.** La IA aprende cómo se ve lo "normal" en tu red —tráfico normal, inicios de sesión normales, acceso normal a datos— y marca lo que está raro. Un inicio de sesión desde un país extraño a las 3 a.m., una inundación súbita de descargas de archivos, un dispositivo comportándose de forma extraña. Estas pequeñas señales, vistas a la vez en toda la red, son cómo la IA atrapa una amenaza que un humano perdería.

**Atraviesa el ruido de alertas.** Las herramientas de seguridad producen miles de alertas, la mayoría inofensivas. La IA las clasifica para que la amenaza real suba a la cima y el ruido caiga. Este es uno de sus mayores valores: no más alertas, sino *menos y mejores* alertas que un pequeño equipo puede realmente manejar.

**Responde más rápido.** Cuando la IA marca una amenaza real, también puede sugerir o tomar una primera acción rápida —aislar una máquina infectada, bloquear una dirección sospechosa— para detener la propagación mientras un humano investiga. La velocidad importa en un ataque; los primeros minutos deciden cuánto daño se hace.

**El panorama de seguridad completo es su propio tema.** Las amenazas, las defensas y los hábitos humanos que más importan se tratan en profundidad en el [Capítulo 6 — Ciberseguridad en la era de la IA](ch06-cybersecurity-in-the-ai-era.md), y el despliegue seguro en el [Capítulo 20 — Implementar la IA de forma segura](ch20-implementing-ai-securely.md). Lee esos antes de depender de la IA para tu defensa. La IA es una herramienta potente, no un escudo mágico.

**Guarda un humano para la gran decisión.** La IA puede aislar una máquina, pero una persona decide si apagar un sistema, si pagar o rechazar un rescate, si llamar a las autoridades. En un incidente real, el juicio humano es la última línea de defensa. Nunca dejes que la automatización tome las grandes decisiones de seguridad sola.

### 30.3 Reportes de gestión

Un reporte de gestión convierte datos crudos en una imagen clara que un líder puede leer y accionar —pérdidas y ganancias, ventas por producto, costes por categoría, posición de caja—. La IA cambia quién construye el reporte y qué tan rápido.

**El reporte se construye solo.** En vez de un analista tirando números a una hoja de cálculo cada semana, el reporte puede generarse en un calendario desde tus sistemas en vivo y aterrizar en la bandeja del líder. Los números siempre están al día, y nadie tiene que acordarse de hacerlo.

**Resúmenes en lenguaje claro.** La IA puede leer los números y escribir un resumen corto en palabras claras: "Los ingresos subieron 8% este mes, impulsados por el producto X; los costes subieron 3%, sobre todo en envíos." Esto convierte una tabla de cifras en una frase que un líder puede realmente leer y accionar. Es como tener un analista júnior que escribe el comentario.

**Pregunta en lenguaje claro.** Algunas herramientas dejan a un líder preguntar, "¿Qué línea de producto perdió dinero el trimestre pasado?" y obtener una respuesta sin escribir una fórmula. Esto es útil para las preguntas ad-hoc que antes significaban "lo miraré más tarde" y luego nunca pasaba. El líder obtiene la respuesta mientras la pregunta aún está fresca.

**No te saltes la lectura humana.** Un reporte automático es un punto de partida, no un documento de decisión terminado. Lee el resumen, comprueba que los números tengan sentido, y añade tu propio juicio antes de accionar o compartir. La IA puede resumir con confianza y seguir estando equivocada si los datos subyacentes están desordenados. Basura entra, basura con confianza sale.

**Mantén el formato estable.** Una vez que te asientes en un diseño de reporte, mantenlo consistente. Un formato estable es más fácil de leer mes a mes y más fácil de detectar cuando algo se ve raro. Cámbialo a propósito, no cada vez. (Las mismas ideas de construcción de reportes, aplicadas a finanzas, están en el [Capítulo 25 — Administración y Finanzas](ch25-administration-and-finance.md).)

### 30.4 Soporte a la decisión

Soporte a la decisión significa usar la IA para exponer las opciones, la evidencia y las compensaciones de una decisión, para que un líder pueda elegir bien. No toma la decisión. Hace la decisión *informada*.

**Expón las opciones.** Para una elección como "¿Deberíamos abrir una nueva región?" o "¿Qué proveedor deberíamos elegir?", la IA puede reunir los datos relevantes y presentar las opciones lado a lado, con los pros, los contras y los números detrás de cada una. El líder ve el panorama completo, no el favorito de una persona.

**Modela las compensaciones.** La IA puede mostrar qué pasa bajo distintos supuestos: "Si la demanda sube 10%, esta opción gana; si se mantiene plana, esa otra es más segura." Esto convierte una suposición en una comparación de escenarios, que es mucho más útil para una gran decisión.

**Saca a la luz lo que pasaste por alto.** La IA puede señalar un riesgo u oportunidad que un líder ocupado no vio, porque miró todo a la vez. El caso de riesgo de proveedor de IBM de arriba es exactamente esto: la IA leyendo las respuestas de cada proveedor para que el evaluador vea el riesgo con claridad antes de decidir.

**Guarda la decisión con el líder.** La IA asesora; el líder decide y es dueño del resultado. Un líder que sigue ciegamente al modelo ha dejado de liderar. Usa la IA para informar tu juicio, no para reemplazarlo. La estrategia detrás de estas elecciones está en el [Capítulo 13 — Definir una simple estrategia de IA](ch13-defining-a-simple-ai-strategy.md).

**Vigila las tonterías con confianza.** La IA puede presentar una opción equivocada con total confianza. Comprueba la evidencia detrás de su consejo, especialmente para una decisión grande o inusual. Pide al modelo que muestre su razonamiento, y ponlo a prueba contra lo que sabes. Confía, pero verifica.

## Ética y responsabilidad

TI y liderazgo cargan la confianza de toda la empresa, así que la responsabilidad aquí es amplia.

**Guarda al humano en la gran decisión.** La IA asesora sobre seguridad, reportes y estrategia. Una persona toma la decisión de apagar un sistema, confiar en un proveedor, o tomar un riesgo. Cuanto mayor la decisión, más es humano suyo.

**Protege los datos que das a los modelos.** Los datos de TI y liderazgo —registros de red, finanzas, registros de proveedores— están entre los más sensibles que una empresa guarda. Mantenlos seguros y, donde importe, dentro de tu propio entorno. No des datos sensibles a herramientas de IA públicas sin comprobar las implicaciones de seguridad (ver [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md) y [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md)).

**Vigila la IA de terceros y en la sombra.** Los proveedores y el personal pueden traer herramientas de IA a la empresa sin aprobación —el riesgo de "IA en la sombra"—. Sabes qué IA está corriendo en tu red y quién la aprobó. Ese riesgo se trata en el [Capítulo 9 — Servicios de terceros e IA en la sombra](ch09-third-party-services-and-shadow-ai.md).

**Sé honesto en reportes y consejos.** Un resumen de IA puede hacer que un mal trimestre suene bien, y el consejo de IA puede estar equivocadamente seguro. Lee los números, comprueba el consejo, y reporta la verdad, especialmente cuando es incómoda. El trabajo de un líder es ver con claridad, no ser consolado.

**Ten presente el suelo legal.** Algunos usos de IA en TI y RRHH tocan las reglas de alto riesgo y transparencia de la Ley de IA de la UE. Conoce tu rol y tus deberes antes de desplegar (ver [Capítulo 5 — Reglas y responsabilidad legal](ch05-rules-and-legal-responsibility.md)). El cumplimiento es el suelo; tu propio juicio fija el estándar por encima.

**Usa la IA para fortalecer la confianza, no para controlar a la gente.** La monitorización y la analítica deberían hacer la empresa más segura y mejor gestionada, no volverse una herramienta para vigilar y presionar al personal. Úsalas para proteger y mejorar, no para vigilar como policía.

## Errores a evitar

**Un help desk solo-bot.** Personal con un problema real atrapado detrás de un bot sin camino humano. Permite siempre un traspaso a un humano.

**Confiar en una alerta de seguridad a ciegas.** Actuar sobre un falso positivo, o peor, ignorar una amenaza real porque la alerta estaba enterrada. Ajusta el sistema y guarda un investigador humano.

**Dejar que la automatización tome la gran decisión de seguridad.** Apagar, pagar o escalar sin un humano. Guarda la decisión humana en un incidente.

**Saltarse la lectura humana en los reportes.** Actuar sobre un resumen de IA sin comprobar los números. Léelo tú primero.

**Tonterías con confianza en el consejo.** Seguir consejo de IA que está mal pero bien redactado. Comprueba la evidencia detrás.

**Fe ciega en el modelo para grandes decisiones.** Un líder que deja de liderar y solo sigue el panel. El líder es dueño de la decisión.

**Dar datos sensibles a IA pública.** Registros de red, finanzas y registros de proveedores a herramientas inseguras. Comprueba seguridad y privacidad primero.

**IA en la sombra corriendo sin control.** Personal y proveedores usando herramientas de IA no aprobadas. Sabes qué está corriendo y quién lo aprobó.

**Automatizar un proceso roto.** Si tu soporte de TI o tus reportes son un desastre, la IA hace un desastre más rápido. Arregla el proceso primero.

**Sin línea base.** No medir el tiempo de tickets, la tasa de incidentes, o el tiempo de reporte antes, así que no puedes probar la ganancia. Mide primero (ver [Capítulo 22 — Medir resultados y ROI](ch22-measuring-results-and-roi.md)).

**Citar el número del proveedor como el tuyo.** Usar la cifra del mejor caso de un proveedor en vez de tu propio resultado medido. Usa tus propios números.

## Ejercicio práctico

### 30.7 Ejercicio: planifica una automatización de TI o liderazgo

Elige un trabajo y planifica su asistencia de IA de principio a fin, con la decisión humana incorporada.

**Paso 1 — Elige el trabajo.** Elige uno: soporte interno, ciberseguridad, reportes de gestión, o soporte a la decisión. Haz uno, no todos.

**Paso 2 — Define la meta y la métrica.** ¿Resolución de tickets más rápida? ¿Menos amenazas perdidas? ¿Reportes más rápidos? ¿Mejores decisiones? Elige un número para medir.

**Paso 3 — Mide la línea base.** ¿Cuál es ese número ahora? Tiempo medio de ticket, incidentes perdidos, días para construir un reporte, tiempo de respuesta a decisiones. Escríbelo.

**Paso 4 — Encuentra el objetivo costoso.** Identifica el punto más doloroso —el tipo de ticket que más tiempo se come, la amenaza que se escapa, el reporte que siempre llega tarde, la decisión que sigues equivocando—. Ataca ese primero.

**Paso 5 — Marca cada paso.** Para cada paso, márcalo: **la IA lo hace** (responder, marcar, resumir, exponer opciones), **el humano lo revisa** (comprobar la alerta, leer el reporte), o **el humano lo decide** (apagar el sistema, elegir el proveedor, tomar el riesgo). Cada gran decisión debe ser humana.

**Paso 6 — Comprueba los datos y la ley.** Decide qué datos necesita la IA, mantenlos seguros, y comprueba si el uso toca las reglas de alto riesgo o transparencia de la Ley de IA (ver [Capítulo 5](ch05-rules-and-legal-responsibility.md)).

**Paso 7 — Conecta los sistemas.** Decide qué sistemas necesita ver la IA —tickets, registros, finanzas, registros de proveedores— y cómo los conectarás (ver [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md)).

**Paso 8 — Lanza pequeño y mide.** Ejecútalo en un equipo, un sistema, o un reporte primero. Compara la métrica con la línea base. Escala solo lo que pruebe que funciona.

Haz un trabajo bien. El análisis de objetivo costoso del paso 4 es valioso por sí solo —te muestra dónde tu trabajo de TI y liderazgo realmente pierde más tiempo o carga más riesgo, lo cual es útil incluso antes de comprar cualquier herramienta—.

## Lista de comprobación

### 30.8 Lista de comprobación de TI y liderazgo

Antes de automatizar cualquier tarea de TI o liderazgo, comprueba esto.

- [ ] **Mediste la línea base** —tiempo de ticket, tasa de incidentes, tiempo de reporte, tiempo de respuesta a decisiones—.
- [ ] **Atacaste el punto más costoso primero**, no el más fácil.
- [ ] **Un humano toma cada gran decisión** —apagado del sistema, confianza en proveedor, aceptación de riesgo—.
- [ ] **El bot del help desk pasa a un humano** con contexto completo.
- [ ] **Las alertas de seguridad están ajustadas** para que la amenaza real suba y el ruido caiga.
- [ ] **Un humano investiga cada incidente de seguridad real.**
- [ ] **Los reportes de gestión son leídos por un humano** antes de que actúes o los compartas.
- [ ] **Compruebas la evidencia detrás del consejo de IA**, especialmente para grandes decisiones.
- [ ] **Los datos sensibles se mantienen seguros**, no enviados a servicios de IA públicos.
- [ ] **Sabes qué IA está corriendo en tu red** y quién la aprobó (sin IA en la sombra).
- [ ] **Comprobaste la Ley de IA** por cualquier deber de alto riesgo o transparencia.
- [ ] **Arreglas el proceso roto antes de automatizarlo.**
- [ ] **Reportas tus propios números medidos**, no el mejor caso del proveedor.

Si una casilla está vacía, el riesgo —a tus sistemas, tus datos, o tus decisiones— sigue siendo tuyo. Rellénala antes de dejar que la IA se acerque a los controles.

## Puntos clave

- La IA en TI y liderazgo es un copiloto: responde preguntas de soporte, detecta amenazas, construye reportes y expone opciones, mientras un humano guarda cada gran decisión.
- El caso de riesgo de proveedor de IBM (IBM Client Engineering, "Evaluating Third Party Risk with AI") ayudó a una institución financiera con más de 1.000 evaluaciones al año a ~45 horas cada una, con una estimación publicada de ~20% de reducción de tiempo, ~10.000 horas y ~$800k ahorrados al año —la cifra de "unos 50%" no es lo que reporta la fuente publicada—.
- El ahorro viene de dejar que la IA haga la lenta lectura y comprobación mientras el humano guarda el juicio; el mismo patrón funciona en soporte, seguridad, reportes y decisiones.
- Mantén los datos sensibles seguros, sabe qué IA está corriendo en tu red, y comprueba las reglas de alto riesgo y transparencia de la Ley de IA antes de desplegar.
- Mide tu propia línea base, guarda un humano en cada gran decisión, y trata la ley como el suelo y tu propio juicio como el estándar por encima.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Notas de reunión limpias

![Actas de reunión prolijas con decisiones y acciones](../../assets/examples/meeting-minutes.png)
*Actas de reunión prolijas con decisiones y acciones*

**Qué preguntas:** `Convierte estas notas toscas en actas de reunión limpias con una lista de decisiones y elementos de acción: [pega notas]`

El agente convierte tus notas desordenadas en actas estructuradas: qué se discutió, qué se decidió, y una lista de acciones con dueños. Puedes enviarlas directo al equipo.

*Consejo: Pega tus notas tal como están —el agente ordena la secuencia y la redacción—.*

---

### Una revisión trimestral del consejo

![Una diapositiva de presentación de revisión trimestral](../../assets/examples/board-review.png)
*Una diapositiva de presentación de revisión trimestral*

**Qué preguntas:** `Construye una presentación de revisión trimestral: resultados, logros, desafíos, y plan del próximo trimestre.`

El agente ensambla la presentación de revisión con los resultados, los éxitos, los problemas y el plan —expuesto para que la reunión avance rápido—.

*Consejo: Adjunta tu hoja de KPI y el agente pone los gráficos en las diapositivas.*

---

### Ve todos tus agentes de un vistazo

![La vista de OfficeManager de tus agentes](../../assets/examples/officemanager-view.png)
*La vista de OfficeManager de tus agentes*

**Qué preguntas:** `(browser) Abre la vista de OfficeManager.`

OfficeManager muestra tus agentes en una página simple, para que puedas ver qué está corriendo y cómo están las cosas.

*Consejo: Una forma rápida de vigilar más de un asistente a la vez.*

---

### Un informe que puedes escuchar

![Un informe de audio listo para reproducir](../../assets/examples/audio-briefing.png)
*Un informe de audio listo para reproducir*

**Qué preguntas:** `Convierte el resumen de esta semana en un breve informe de audio que pueda escuchar de camino al trabajo.`

El agente convierte el resumen escrito en un claro informe de audio, así tu trayecto se vuelve tiempo útil.

*Consejo: Programa el resumen semanal y su versión en audio juntos.*

<!-- END agentbridge-examples -->
