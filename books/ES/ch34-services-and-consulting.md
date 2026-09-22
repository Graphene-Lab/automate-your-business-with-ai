# Capítulo 34 — Servicios y consultoría

*Este capítulo es un compuesto representativo. No es una firma real. Combina los patrones comunes que vemos en firmas de consultoría y servicios profesionales que adoptan IA. Todos los números son ilustrativos —muestran la forma de la decisión, no una promesa. Reemplázalos con los tuyos.*

## Contexto

Imagina una firma de consultoría mediana. La llamaremos **Northbeam Advisory**. Tiene unos veinticinco consultores y un pequeño equipo de apoyo. No vende un producto. Vende experiencia y tiempo. Un cliente —normalmente otra empresa— tiene un problema, y Northbeam envía gente a resolverlo: un proyecto de estrategia aquí, una revisión de operaciones allá, un estudio de datos en otro sitio.

Cada proyecto sigue el mismo camino aproximado. Primero llega el **pitch**: una propuesta que dice qué entiende la firma, qué hará, y cuánto costará. Si el cliente acepta, el equipo hace el trabajo. Durante el trabajo, el cliente recibe **reportes de estado** regulares. Al final, hay un entregable final y una factura. Entre todo esto se sienta una montaña de coordinación: encontrar a las personas correctas para el trabajo, agendar reuniones, escribir lo que se dijo, y llevar la cuenta de quién está libre cuándo.

Durante años, todo esto funcionó con personas. Un socio escribe una propuesta abriendo una vieja y reescribiéndola. Un consultor resuelve un problema que la firma resolvió hace tres años, pero nadie recuerda dónde, así que lo resuelven desde cero. Un jefe de proyecto construye cada reporte de estado a mano, copiando números de un archivo a una diapositiva. Alguien pasa medio día haciendo coincidir los calendarios de los consultores con las necesidades del proyecto. La firma tiene éxito. Pero gasta una gran cantidad de tiempo caro y formado en trabajo que es repetitivo, y sigue perdiendo conocimiento que ya pagó una vez.

Una firma de consultoría es como una práctica profesional en una forma importante. Todo lo que toca es **confidencial**. La estrategia de un cliente, un modelo de costes, un plan de fusión —estos se comparten de buena fe. Ese solo hecho da forma a cómo puede usarse la IA aquí, igual que en un bufete. Es el hilo que recorre este capítulo.

## El problema

Las fugas de la firma son fáciles de nombrar.

**Las propuestas son lentas.** Cada pitch nuevo empieza cerca de una página en blanco. La firma ha escrito cientos de propuestas y tiene buen material en ellas, pero encontrar el ejemplo pasado correcto, el caso de estudio correcto, la estructura de precios correcta, lleva tiempo. Un socio podría pasar dos días enteros en una propuesta que es sobre todo reensamblaje. Las propuestas lentas también significan oportunidades perdidas —algunos tratos se pierden simplemente porque la respuesta llegó demasiado tarde—.

**El conocimiento se va por la puerta.** Cuando un consultor se va, el saber en su cabeza se va con él. Un método que refinó, una manía de un cliente que aprendió, una solución que elaboró —a menos que alguien lo escribiera, se ha ido—. Así que la firma paga por resolver los mismos problemas una y otra vez. Esta es la fuga más cara, porque es invisible.

**Los reportes son manuales.** Un reporte de estado es mayormente igual cada semana: qué avanzó, qué está tarde, qué sigue. Pero una persona lo ensambla a mano cada vez, sacando números de archivos de proyecto y escribiendo el mismo tipo de narrativa. Es fiable y es aburrido, y se come horas que podrían ser facturables.

**Gasto de coordinación.** Hacer coincidir las habilidades del consultor correcto con un proyecto, comprobar quién está libre, agendar reuniones, y escribir las notas después es un impuesto constante. Las reuniones ocurren, pero nadie quiere escribir las actas, así que las decisiones se vuelven borrosas y alguien tiene que rehacer la conversación más tarde.

Si quieres ver cómo estas se clasifican contra el resto de tu firma, el método de impacto y esfuerzo del [Capítulo 12 — Dónde puede ayudar la IA a tu negocio](ch12-where-ai-can-help-your-business.md) es el lugar para puntuarlas.

Sobre las cuatro se sienta la confidencialidad. Cualquier herramienta que lea la propuesta o el archivo de proyecto de un cliente debe ser una herramienta en la que la firma pueda confiar para no filtrarlo. Esa pregunta va primero.

## La solución

Northbeam ataca las cuatro fugas en orden de seguridad, no solo de tamaño. La regla es la misma que usa un bufete: empieza donde un error es barato y los datos no son los más sensibles, y avanza hacia el trabajo sensible solo cuando las herramientas son de fiar.

**Un asistente de propuestas que redacta desde la propia historia de la firma.** Cuando llega un pitch nuevo, un consultor escribe un breve resumen —el cliente, el problema, el alcance aproximado—. Un asistente de IA busca en las propuestas pasadas de la firma y saca las secciones más relevantes, luego redacta una primera versión: una comprensión del problema, un enfoque sugerido, un caso de estudio que encaja. El socio ya no empieza en frío. Edita un borrador en vez de construir desde la nada. Dos días se vuelven unas pocas horas. Este es el mismo patrón de "la máquina redacta, el humano revisa" que muestra el caso de Elanco en el [Capítulo 25 — Administración y Finanzas](ch25-administration-and-finance.md).

**Una memoria buscable para la firma.** La firma pone sus entregables, métodos y notas pasados en una búsqueda interna que los consultores pueden consultar en lenguaje claro. Esto a menudo se llama una **base de conocimiento con búsqueda de IA**. Por dentro usa una técnica llamada **generación aumentada por recuperación**, o RAG. En palabras simples: en vez de hacerle una pregunta a una IA general, el sistema primero busca en los propios documentos de la firma, luego responde usando solo lo que encontró allí. Así que cuando un consultor pregunta, "¿Cómo manejamos una revisión de riesgo de proveedor para un cliente minorista?", el sistema encuentra el proyecto pasado real y responde desde él. El conocimiento deja de irse por la puerta. La tecnología de chatbot y búsqueda detrás de esto se trata en el [Capítulo 27 — Atención y Soporte al Cliente](ch27-customer-care-and-support.md).

**Reportes que se redactan solos.** La herramienta de reporte de estado se conecta a los datos del proyecto —tareas, fechas, hitos— y redacta el reporte semanal: qué avanzó, qué se retrasó, qué sigue. El jefe de proyecto lo revisa, añade el juicio humano sobre el tono y qué enfatizar, y lo envía. La página en blanco se ha ido.

**Agendamiento y resúmenes de reuniones.** Un asistente de agendamiento hace coincidir las habilidades y disponibilidad de los consultores con las necesidades del proyecto y propone quién debería trabajar en qué. Para reuniones, una herramienta graba la llamada, redacta el acta, y lista las decisiones y elementos de acción. Una persona lo comprueba antes de que circule. Las decisiones dejan de ser borrosas porque la redacción ocurre automáticamente.

En cada caso, el humano se mantiene al mando. En consultoría, el cliente paga por juicio y responsabilidad. La IA redacta, busca y resume. El consultor decide, adapta y respalda el trabajo.

## Las herramientas

Las herramientas son corrientes, pero la forma en que se despliegan está moldeada por la confidencialidad.

- **Un asistente de propuestas** que busca en las propuestas pasadas de la firma y redacta una nueva desde un resumen.
- **Una búsqueda de conocimiento interna** (RAG) sobre los entregables y notas de la firma, para que los consultores puedan hacer preguntas en lenguaje claro y obtener respuestas fundamentadas en el trabajo propio de la firma.
- **Un asistente de reportes** que se conecta a los datos del proyecto y redacta reportes de estado.
- **Un asistente de agendamiento** para emparejar personas con proyectos, más una **herramienta de resumen de reuniones** que convierte una llamada grabada en un borrador de acta.

Cómo elegir estas herramientas sin deslumbrarte con una demo se trata en el [Capítulo 17 — Elegir herramientas sin ser engañado](ch17-choosing-tools-without-being-fooled.md). Cómo conectarlas a los sistemas de gestión de proyectos y documentos existentes de la firma está en el [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).

**La confidencialidad va primero.** Un chatbot general en el que pegas una propuesta de cliente puede almacenarla, entrenar con ella, o exponerla. Para una firma de consultoría, eso puede romper la confianza de un cliente y un deber contractual de secreto. La firma debe usar herramientas que mantengan privados los datos del cliente —o un servicio de grado empresarial con un contrato claro de no-entrenamiento y no-compartición, o un modelo ejecutado en las propias máquinas de la firma—. El autoalojamiento se explica en el [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md). El peligro de que el personal pegue en silencio datos de clientes en herramientas públicas —IA en la sombra— es el tema del [Capítulo 9 — Servicios de terceros e IA en la sombra](ch09-third-party-services-and-shadow-ai.md). Y como los expedientes de clientes y las listas de contactos guardan datos personales, las reglas de privacidad del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md) se aplican por completo.

## Los costes

Aquí hay un presupuesto ilustrativo del primer año para una firma como Northbeam. Estos son números inventados para mostrar la forma. Usa los tuyos.

**Costes directos.**
- Asistente de propuestas (grado empresarial, con contrato de confidencialidad): unos €12.000 al año.
- Búsqueda de conocimiento interna (plataforma RAG): unos €9.000 al año.
- Asistente de reportes: unos €4.800 al año.
- Herramientas de agendamiento y resumen de reuniones: unos €6.000 al año.
- Configuración e integración con los sistemas de gestión de proyectos y documentos: unos €12.000 únicos.
- Formación de los consultores y el personal de apoyo: unos €5.000 únicos.

Total del primer año: aproximadamente **€48.800**. En años estables después, las suscripciones recurrentes llegan a unos **€31.800**.

**Costes indirectos.**
- Los consultores gastan tiempo revisando cada borrador de la IA. Este es el coste de la red de seguridad, y debe quedarse.
- La caída de aprendizaje mientras todos se adaptan.
- El coste de curar la base de conocimiento. Una búsqueda es solo tan buena como lo que pones en ella, y alguien debe mantenerla limpia y al día.
- Tiempo dedicado a examinar cada herramienta por confidencialidad y cumplimiento antes de usarla.
- El coste de un error si se confía en un borrador sin comprobar —en consultoría, un número equivocado en un reporte de cliente puede costar mucho más que una suscripción—.

El método completo para contar estos costes y convertir los ahorros en una cifra de retorno está en el [Capítulo 16 — Objetivos, Costes y Retorno de la Inversión](ch16-goals-costs-and-return-on-investment.md). No hagas las matemáticas de cabeza. Escríbelas.

## Los resultados

Tras un año, medido contra una línea base que la firma registró antes de empezar, el resultado ilustrativo se ve así. Tus números diferirán. Estos muestran cómo puede verse un buen ajuste.

- **Las propuestas se volvieron más rápidas.** Un pitch que tomaba dos días ahora toma unas pocas horas, porque el socio edita un borrador en vez de construir desde una página en blanco. La firma también responde antes, lo que gana algunos tratos que habría perdido.
- **El conocimiento se quedó.** Cuando los consultores se iban, su saber se quedaba en la base buscable. La firma resolvía menos problemas dos veces.
- **El tiempo de reportes bajó.** El reporte de estado semanal se volvió una revisión de un borrador, no una construcción manual, liberando horas en los jefes de proyecto.
- **Las reuniones produjeron registros.** Decisiones y elementos de acción se escribían automáticamente, así que menos conversaciones tuvieron que repetirse.
- **Más tiempo facturable.** Con menos tiempo gastado en reensamblaje y búsqueda, los consultores pasaban más de su día en trabajo por el que el cliente paga.

La advertencia honesta: nada de esto fue instantáneo. El asistente de propuestas producía borradores toscos al principio hasta que tuvo suficientes buenas propuestas pasadas para aprender el estilo de la firma. La búsqueda de conocimiento daba respuestas débiles hasta que los documentos se organizaron y etiquetaron. La herramienta de resumen de reuniones etiquetaba mal a los hablantes al principio. Las ganancias se incrementaron durante semanas, como predice la advertencia de la curva de aprendizaje en el [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). La firma midió los números reales tras la rampa, no durante ella.

## Lecciones aprendidas

**La confidencialidad es la primera restricción, no una ocurrencia tardía.** En consultoría, la pregunta nunca es solo "¿funciona esta herramienta?" Es "¿se puede confiar en esta herramienta con el expediente privado de un cliente?" Responde eso antes que nada. Usa herramientas de grado empresarial con un contrato claro de no-entrenamiento, o autoalójate. Ver [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md) y [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).

**La IA redacta; el consultor asesora.** El valor de un consultor es el juicio y la responsabilidad. La IA hace listas cortas, redacta y resume; el consultor decide y firma. Nunca dejes que un borrador se vuelva trabajo de cara al cliente sin una mente humana sobre él.

**Una base de conocimiento es un jardín, no un vertedero.** La búsqueda de IA es solo tan buena como los documentos detrás. Si echas archivos desordenados, rancios o equivocados, obtienes respuestas equivocadas con confianza. Alguien debe ser dueño de la base, mantenerla al día, y controlar quién puede ver qué. El control de acceso importa: un consultor en el proyecto de un cliente no debería poder buscar el material confidencial de otro cliente. El principio de preparación de datos está en el [Capítulo 14 — Datos: la materia prima](ch14-data-the-raw-material.md).

**Grabar reuniones necesita consentimiento.** Una herramienta de resumen de reuniones funciona grabando la llamada. Grabar una conversación es tratamiento de datos personales, y las personas deben saberlo y estar de acuerdo. Informa a los participantes antes de grabar, y sigue las reglas del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md). No grabes en silencio.

**Cuidado con la respuesta equivocada con confianza.** Estas herramientas pueden producir texto que suena correcto y está mal —un caso de estudio que nunca ocurrió, un número que no cuadra—. En consultoría, una cifra fabricada en un reporte de cliente es un desastre. Verifica cada número y cada afirmación contra la fuente real. El problema de fiabilidad se trata en el [Capítulo 2 — La IA explicada de forma simple](ch02-ai-explained-simply.md), y el deber de ser honesto sobre lo que la IA puede y no puede hacer está en el [Capítulo 4 — IA ética: hacer lo correcto](ch04-ethical-ai-doing-the-right-thing.md).

**Empieza con el trabajo seguro.** Northbeam empezó con búsqueda interna y borradores de reportes —bajo riesgo, aún no las propuestas de clientes más sensibles—. Se movió hacia la redacción de propuestas solo una vez que las herramientas fueron de fiar. Esta es la regla de "primero la alta facilidad" del [Capítulo 12](ch12-where-ai-can-help-your-business.md).

**Mide con honestidad y espera la rampa.** Registra la línea base antes de empezar. Juzga el proyecto tras la curva de aprendizaje, no durante ella. El método está en el [Capítulo 22 — Medir resultados y ROI](ch22-measuring-results-and-roi.md).

La lección de la firma de consultoría es la misma que la de cada otro sector, con una barandilla extra: encuentra el trabajo repetitivo —propuestas, búsqueda, reportes, coordinación—, deja que la IA redacte y recupere, guarda un humano en el juicio y la relación con el cliente, y mide con honestidad. Y en una firma construida sobre la confianza, nunca dejes que la herramienta toque el expediente confidencial de un cliente hasta que estés seguro de que es seguro hacerlo.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Dibuja tu área de servicio

![Un mapa de área de servicio para clientes](../../assets/examples/service-area.png)
*Un mapa de área de servicio para clientes*

**Qué preguntas:** `Muestra nuestra área de servicio en un mapa con los principales pueblos que cubrimos.`

El agente produce un mapa claro de tu cobertura que puedes poner en tu sitio web o enviar a clientes.

*Consejo: Mantenlo actualizado a medida que creces —solo pide una nueva versión—.*

<!-- END agentbridge-examples -->
