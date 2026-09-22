# Capítulo 32 — Una práctica profesional

*Este capítulo es un compuesto representativo. No es una firma real. Combina los patrones comunes que vemos en pequeñas firmas de abogados y contabilidad que adoptan IA. Todos los números son ilustrativos —muestran la forma de la decisión, no una promesa. Reemplázalos con los tuyos.*

## Contexto

Imagina un pequeño bufete de derecho mercantil. Lo llamaremos **Marlowe Legal**. Tiene doce abogados y un puñado de personal de apoyo. No es el tipo de firma que litiga ante jueces. Hace papeleo: contratos, arrendamientos, acuerdos societarios, asesoría de cumplimiento. Los clientes son otras empresas.

El trabajo de tal firma es, en su núcleo, leer y escribir. Un cliente envía un contrato largo y pregunta: "¿Es seguro firmar esto?" Un cliente nuevo llama y necesita que abran su asunto. Hay que redactar un arrendamiento estándar desde la plantilla de la firma. A fin de mes, cada abogado anota los minutos que gastó y envía una factura.

Durante años, todo esto se hizo a mano. Un abogado júnior lee un contrato de doscientas páginas y escribe un resumen. Una recepcionista atiende la llamada del cliente nuevo y rellena un formulario. Un abogado sénior teclea las mismas cláusulas en cada arrendamiento. Por la noche, todos intentan recordar en qué trabajaron para poder facturarlo. La firma es rentable y respetada. Pero gasta una gran cantidad de tiempo caro y formado en trabajo que es repetitivo.

Una práctica profesional es diferente de una tienda o una fábrica en una forma crucial. Todo lo que toca es **confidencial**. El contrato de un cliente, un plan de fusión, un expediente de disputa —estos están protegidos por el secreto profesional, la regla de que un cliente puede hablar libremente con su abogado sin que se revele el contenido. Este solo hecho cambia cómo puede usarse la IA, y es el hilo que recorre todo este capítulo.

## El problema

Los problemas de la firma son las mismas cuatro fugas que en todas partes, pero con un giro profesional.

**La revisión de documentos es lenta y costosa.** Cuando un cliente pide a la firma revisar un contrato, un abogado júnior lee cada página y escribe notas sobre cláusulas arriesgadas. Para un gran trato, esto toma días. El cliente paga por esos días. El trabajo es cuidadoso pero repetitivo —los mismos tipos de cláusulas arriesgadas aparecen una y otra vez, y la firma ya sabe qué buscar—. Solo que lleva mucho tiempo mirar.

**La admisión de clientes es inconsistente.** Cuando llama un cliente nuevo, la información capturada depende de quién conteste. Unos obtienen un panorama completo; otros pasan por alto un detalle que importa más tarde. Hechos importantes se caen por el hueco, y el abogado tiene que perseguirlos después.

**La redacción se repite a sí misma.** La firma tiene plantillas, pero cada arrendamiento o acuerdo nuevo sigue necesitando un abogado para ensamblar las cláusulas estándar y ajustarlas. Es fiable pero lento, y es exactamente el tipo de trabajo que no necesita el juicio de un sénior.

**La facturación tiene fugas.** Los abogados facturan por hora, pero son malos registrando cada minuto. Una llamada de diez minutos aquí, un correo rápido allá —estos a menudo quedan sin escribir. A fin de mes, la firma "da de baja" horas que realmente trabajó pero nunca facturó. En doce abogados, esta fuga es grande. Un estudio de firmas legales ha puesto el tiempo típico sin facturar en el rango de varios porcentajes de todas las horas trabajadas; trátalo como una cifra direccional, no precisa. El punto se mantiene: la fuga es real.

La restricción que se sienta sobre las cuatro es la confidencialidad. Cualquier herramienta que lea el contrato de un cliente debe ser una herramienta en la que la firma pueda confiar para no filtrar ese contrato. Esto no es una preocupación menor. Es la primera pregunta, antes que cualquier otra.

## La solución

Marlowe Legal ataca las cuatro fugas en orden de seguridad, no solo de tamaño. La regla es simple: empieza donde un error es barato y los datos no son sensibles, y avanza hacia el trabajo sensible solo cuando las herramientas son de fiar.

**Revisión de documentos que lee primero, luego decide el abogado.** La firma usa un asistente de IA que lee un contrato y produce un resumen de primera pasada: qué hace el acuerdo, qué cláusulas son inusuales, y cuáles se desvían de las posiciones estándar de la propia firma. El abogado júnior ya no lee en frío. Lee las notas de la IA y luego verifica contra el documento real. La IA hace una lista corta de las cláusulas arriesgadas; el abogado hace el juicio legal. Este es el mismo patrón de "la máquina redacta, el humano revisa" que muestra el caso de Elanco en el [Capítulo 25 — Administración y Finanzas](ch25-administration-and-finance.md).

**Admisión que hace las preguntas correctas cada vez.** Un asistente de admisión estructurado —un formulario guiado en el sitio web, o un chatbot que hace un conjunto fijo de preguntas— captura los mismos hechos para cada cliente nuevo. No se pasa nada por alto porque una persona olvidó preguntar. La información estructurada fluye directo al expediente del caso. El lado de chatbot de esto es la misma tecnología tratada en el [Capítulo 26 — Ventas y márketing](ch26-sales-and-marketing.md) y el [Capítulo 27 — Atención y Soporte al Cliente](ch27-customer-care-and-support.md).

**Asistencia de redacción para las partes estándar.** Para documentos rutinarios, un asistente de redacción con IA ensambla las cláusulas estándar y propone la redacción. El abogado revisa y ajusta. El abogado sénior deja de teclear texto estándar y empieza a revisar borradores en su lugar.

**Facturación que captura el tiempo mientras ocurre.** En vez de reconstruir el día por la noche, la firma usa una herramienta que convierte la actividad —correos enviados, documentos abiertos, entradas de calendario— en un borrador de asiento de tiempo con una narrativa sugerida. El abogado revisa y confirma. La fuga se estrecha porque el punto de partida es un borrador casi completo, no una página en blanco.

En cada caso, el humano se mantiene al mando. En una profesión donde una respuesta equivocada daña a un cliente real, la IA es un ayudante de primera pasada, nunca el que decide.

## Las herramientas

Las herramientas son corrientes, pero la forma en que se despliegan está moldeada por la confidencialidad.

- **Un asistente de revisión de documentos** que lee contratos y marca cláusulas contra una lista de comprobación que la firma escribe ella misma. Esta es la misma clase de herramienta de lectura de documentos que maneja facturas en el [Capítulo 25](ch25-administration-and-finance.md), apuntada a texto legal.
- **Un chatbot de admisión o formulario guiado** en el sitio web de la firma que hace un conjunto fijo de preguntas y escribe las respuestas en el sistema de gestión de casos.
- **Un asistente de redacción** para cláusulas y acuerdos estándar, conectado a las plantillas de la firma.
- **Un asistente de captura de tiempo y facturación** que redacta asientos de tiempo desde la actividad del día.

Cómo elegir estas herramientas sin deslumbrarte con una demo se trata en el [Capítulo 17 — Elegir herramientas sin ser engañado](ch17-choosing-tools-without-being-fooled.md). Cómo conectarlas al software de gestión de casos existente de la firma está en el [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).

**La pregunta de confidencialidad va primero.** Un chatbot general en el que pegas un contrato de cliente puede almacenar ese contrato, entrenar con él, o exponerlo. Para un bufete, eso puede romper el secreto profesional y el deber con el cliente. La firma debe usar herramientas que mantengan privados los datos del cliente —o un servicio de grado empresarial con un contrato claro de no-entrenamiento y no-compartición, o un modelo ejecutado en las propias máquinas de la firma—. El autoalojamiento se explica en el [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md). El peligro de que el personal pegue en silencio datos de clientes en herramientas públicas —IA en la sombra— es el tema del [Capítulo 9 — Servicios de terceros e IA en la sombra](ch09-third-party-services-and-shadow-ai.md). Y como los expedientes de clientes contienen datos personales, las reglas de privacidad del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md) se aplican por completo.

## Los costes

Aquí hay un presupuesto ilustrativo del primer año para una firma como Marlowe. Estos son números inventados para mostrar la forma. Usa los tuyos.

**Costes directos.**
- Asistente de revisión de documentos (grado empresarial, con contrato de confidencialidad): unos €12.000 al año.
- Chatbot de admisión: unos €3.600 al año.
- Asistente de redacción: unos €4.800 al año.
- Asistente de captura de tiempo y facturación: unos €4.800 al año.
- Configuración e integración con el sistema de gestión de casos: unos €9.000 únicos.
- Formación de los abogados y el personal: unos €4.000 únicos.

Total del primer año: aproximadamente **€38.200**. En años estables después, las suscripciones recurrentes llegan a unos **€25.200**.

**Costes indirectos.**
- Los abogados gastan tiempo revisando cada borrador de la IA. Este es el coste de la red de seguridad, y debe quedarse.
- La caída de aprendizaje mientras todos se adaptan.
- El coste de un error si se confía en un borrador sin comprobar —en una profesión, esto puede ser mucho mayor que la suscripción—. Presupuesta para revisión cuidadosa, no para esperanza.
- Tiempo dedicado a examinar cada herramienta por confidencialidad y cumplimiento antes de usarla.

El método completo para contar estos costes y convertir los ahorros en una cifra de retorno está en el [Capítulo 16 — Objetivos, Costes y Retorno de la Inversión](ch16-goals-costs-and-return-on-investment.md).

## Los resultados

Tras un año, medido contra una línea base que la firma registró antes de empezar, el resultado ilustrativo se ve así. Tus números diferirán. Estos muestran cómo puede verse un buen ajuste.

- **Revisión de documentos acelerada.** La primera pasada del abogado júnior sobre un contrato largo bajó de días a horas, porque empezó desde el resumen de la IA y verificó en vez de leer en frío.
- **La admisión se volvió completa.** Cada cliente nuevo proporciona ahora el mismo conjunto de hechos. Menos huecos que perseguir después.
- **La redacción se volvió más rápida.** Los documentos rutinarios tomaron una fracción del tiempo, porque el abogado revisó un borrador en vez de ensamblar texto estándar.
- **La fuga de facturación se estrechó.** Como el tiempo se capturaba mientras ocurría, menos horas trabajadas quedaron sin escribir. La firma facturó más de lo que realmente hizo.

La advertencia honesta: nada de esto fue instantáneo. El asistente de revisión de documentos dio resúmenes imperfectos al principio y necesitó que se ajustara la lista de comprobación de la firma. La herramienta de facturación produjo borradores que los abogados tuvieron que corregir antes de confiar. Las ganancias se incrementaron durante semanas, como predice la advertencia de la curva de aprendizaje en el [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). La firma midió los números reales tras la rampa, no durante ella.

## Lecciones aprendidas

**La confidencialidad es la primera restricción, no una ocurrencia tardía.** En una práctica profesional, la pregunta nunca es solo "¿funciona esta herramienta?" Es "¿se puede confiar en esta herramienta con el expediente privado de un cliente?" Responde eso antes que nada. Usa herramientas de grado empresarial con un contrato claro de no-entrenamiento, o autoalójate. Ver [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md) y [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).

**La IA redacta; el profesional asesora.** El valor de un abogado es el juicio y la responsabilidad. La IA hace listas cortas y redacta; el abogado decide y firma. Nunca dejes que un borrador se vuelva asesoría sin una mente humana sobre él.

**Cuidado con la respuesta equivocada con confianza.** Estas herramientas pueden producir texto que suena correcto y está mal —una cláusula que no existe, una cita que está inventada—. En una profesión, una referencia fabricada es un desastre. Verifica cada cita y cada afirmación legal contra la fuente real. El problema de fiabilidad se trata en el [Capítulo 2](ch02-ai-explained-simply.md), y el deber de ser honesto sobre lo que la IA puede y no puede hacer está en el [Capítulo 4 — IA ética: hacer lo correcto](ch04-ethical-ai-doing-the-right-thing.md).

**Empieza con el trabajo seguro.** Marlowe empezó con redacción interna y admisión —bajo riesgo, aún no los expedientes de clientes más sensibles—. Se movió hacia la revisión de contratos solo una vez que las herramientas fueron de fiar. Esta es la regla de "primero la alta facilidad" del [Capítulo 12](ch12-where-ai-can-help-your-business.md).

**La facturación con IA debe revisarse, en ambos sentidos.** Una herramienta de captura de tiempo puede registrar de menos, pero también puede registrar de más o etiquetar mal. Sobrefacturar a un cliente por una suposición de la IA es un problema ético y legal. El abogado revisa cada asiento. Las reglas sobre conducta profesional y los deberes de la Ley de IA de la UE están en el [Capítulo 5 — Reglas y responsabilidad legal](ch05-rules-and-legal-responsibility.md).

**Un dato personal sigue siendo un dato personal.** Los expedientes de clientes guardan nombres, direcciones, detalles financieros. Los deberes de privacidad del [Capítulo 10](ch10-privacy-and-gdpr.md) se aplican a cada uno de ellos, sin importar cómo se comercialice la herramienta.

**Mide con honestidad y espera la rampa.** Registra la línea base antes de empezar. Juzga el proyecto tras la curva de aprendizaje, no durante ella.

La lección de la práctica profesional es la misma que la de cada sector, con una barandilla extra: encuentra el trabajo repetitivo, deja que la IA redacte y marque, guarda un humano en el juicio, y mide con honestidad —y en una profesión, nunca dejes que la herramienta toque el expediente confidencial de un cliente hasta que estés seguro de que es seguro hacerlo—.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Redacta un contrato de servicios

![Un acuerdo de servicios redactado, listo para revisar](../../assets/examples/service-contract.png)
*Un acuerdo de servicios redactado, listo para revisar*

**Qué preguntas:** `Redacta un contrato de servicios entre mi estudio y un cliente para un proyecto de sitio web de 3 meses por 6.000 euros, con un depósito del 50%.`

El agente produce un contrato claro con las partes, el alcance del trabajo, el calendario de pagos y la cronología. Es un punto de partida que puedes revisar y ajustar —no asesoría legal, sino un borrador sólido que te ahorra horas de trabajo de página en blanco—.

*Consejo: Adjunta tu contrato viejo y pídele que siga el mismo estilo y cláusulas.*

<!-- END agentbridge-examples -->
