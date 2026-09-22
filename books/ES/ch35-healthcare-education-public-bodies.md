# Capítulo 35 — Salud, educación y organismos públicos

*Este capítulo es un caso representativo compuesto. No es una organización real. Reúne los patrones comunes que vemos en clínicas pequeñas, escuelas y oficinas públicas que adoptan la IA para la administración. Todas las cifras son ilustrativas: muestran la forma de la decisión, no una promesa. Reemplázalas por las tuyas. Las reglas para los datos regulados están en [Capítulo 10 — Privacidad y GDPR](ch10-privacy-and-gdpr.md) y [Capítulo 5 — Reglas y responsabilidad legal](ch05-rules-and-legal-responsibility.md); este capítulo muestra cómo esas reglas se aplican en la práctica.*

## Contexto

Imagina una pequeña clínica médica comunitaria. La llamaremos **Clínica Familiar Riverside**. Tiene cuatro médicos de cabecera, dos enfermeras y una recepción con tres personas de administración. Atiende a unos pocos miles de pacientes en un pueblo.

El día de la clínica se maneja desde la recepción. El teléfono suena sin parar. La gente llama para pedir una cita, para moverla, para preguntar qué llevar, para consultar sobre una derivación, para saber cuándo estará un resultado. Las tres personas de administración pasan la mayor parte del día al teléfono y con papel. Las cartas de derivación llegan por correo y hay que leerlas, archivarlas y enviarlas al médico correcto. Hay que revisar los formularios antes de atender a un paciente. Mientras tanto, los médicos terminan cada consulta y luego dedican tiempo a redactar las notas, una tarea que se acumula hasta que parte de ella se hace tarde por la noche.

Ahora imagina otros dos lugares con la misma forma. Una **escuela primaria** donde la oficina responde todos los días las mismas preguntas de los padres, gestiona el papeleo de admisiones y se las arregla con los horarios. Una **oficina del ayuntamiento** donde el personal tramita solicitudes de los ciudadanos: un permiso, una solicitud de prestación, un registro, cada una un montón de formularios y documentos que hay que leer, revisar y hacer avanzar.

Tres lugares distintos. El mismo patrón: un equipo pequeño sepultado bajo la programación de citas, los documentos y las preguntas repetidas, mientras las personas formadas —médicos, maestros, trabajadores sociales— dedican tiempo al papeleo en lugar del trabajo para el que se prepararon.

Lo que hace especiales a estos tres lugares es el dato. Una clínica guarda **datos de salud**. Una escuela guarda datos sobre niños. Una oficina pública guarda datos sobre ciudadanos y sus derechos a prestaciones. No son registros corrientes. Están entre los tipos de datos personales más protegidos. Ese solo hecho impone un listón más alto para todo lo que se hace en este capítulo.

## El problema

Las filtraciones son las de siempre, pero el costo de equivocarse es mayor.

**Recepción desbordada.** La cola telefónica es el cuello de botella de la clínica. El personal pasa horas en preguntas repetidas —horario, qué llevar, cómo reprogramar— mientras las llamadas realmente urgentes esperan. Las esperas largas frustran a los pacientes y agotan al personal.

**Ausencias a las citas.** Cuando un paciente olvida una cita, el turno se desperdicia y otra persona podría haberlo tenido. En una clínica concurrida, una alta tasa de ausencias significa que pacientes reales esperan más tiempo para recibir atención.

**Carga de documentación.** Después de cada consulta, el médico escribe notas. Es necesario y es pesado. Los profesionales de la salud en todas partes reportan que dedican una gran parte del día a los registros y no a los pacientes. Es un factor conocido de estrés y agotamiento. El trabajo es minucioso, pero repetitivo.

**Manejo de documentos.** Las cartas de derivación, los formularios y los resultados llegan en muchos formatos. Alguien debe leer cada uno, extraer los datos clave, archivarlo y enviarlo a la persona correcta. Si se pasa por alto un documento, un paciente espera.

**Preguntas repetidas de ciudadanos y padres.** En la escuela y en la oficina del ayuntamiento, las mismas preguntas llegan una y otra vez, en muchos idiomas, y la respuesta siempre es la misma. Responderlas es sencillo, pero consume la oficina.

Por encima de todo esto está la regla de que estos datos son de **categoría especial**. Según el GDPR, los datos de salud y los datos sobre niños reciben una protección extra. La Ley de IA de la UE añade más: los sistemas usados en dispositivos médicos o de formas que afectan los derechos de las personas se consideran de mayor riesgo y conllevan obligaciones más pesadas. Los detalles están en el [Capítulo 10](ch10-privacy-and-gdpr.md) y el [Capítulo 5](ch05-rules-and-legal-responsibility.md). La idea aquí es simple: en estos entornos, la privacidad y el cumplimiento no son una casilla que marcar al final. Definen cada decisión desde el principio.

## La solución

Riverside ataca la carga administrativa según el orden de seguridad. La regla es la misma que en un bufete de abogados: empieza donde un error es barato y el dato es menos sensible, y avanza hacia el trabajo delicado solo cuando las herramientas son confiables. Y en una clínica, el trabajo más delicado —el criterio clínico— nunca se automatiza.

**Agendamiento y recordatorios con IA.** Un chatbot en el sitio web y un sistema telefónico gestionan las reservas rutinarias: pedir, mover, cancelar. Responden al instante las preguntas repetidas. Los recordatorios automáticos se envían antes de cada cita, lo que reduce las ausencias. El personal de recepción queda libre para las llamadas que necesitan un humano: un paciente preocupado, un caso complejo. La tecnología del chatbot es la misma que en el [Capítulo 27 — Atención y soporte al cliente](ch27-customer-care-and-support.md).

**Documentación ambiental que redacta, y el médico firma.** Para una consulta, una herramienta escucha la conversación (con el consentimiento claro del paciente) y redacta después la nota clínica. El médico la revisa, corrige lo que esté mal y la firma. El médico es totalmente responsable de la nota; la herramienta solo quita el tecleo. Es el mismo patrón de "la máquina redacta, el humano revisa" que muestra el caso Elanco en el [Capítulo 25 — Administración y finanzas](ch25-administration-and-finance.md). La herramienta no diagnostica. Anota lo que se dijo para que el médico pueda comprobarlo.

**Enrutamiento de documentos.** Una herramienta lee las cartas de derivación y los formularios que llegan, extrae los datos clave —el paciente, la solicitud, la urgencia— y los archiva y enruta. Una persona sigue revisando el montón, pero la clasificación ya está hecha, así que nada queda sin leer.

**Un asistente de preguntas para ciudadanos y padres.** En la escuela y en la oficina del ayuntamiento, un chatbot responde las preguntas repetidas en lenguaje sencillo y en varios idiomas, a cualquier hora. Un padre que pregunta "¿qué documentos necesito para la admisión?" o un ciudadano que pregunta "¿cómo solicito este permiso?" obtiene una respuesta inmediata. El personal de la oficina atiende solo las preguntas que el bot no puede.

Fíjate en la línea que nunca se mueve. La IA reserva, recuerda, redacta, extrae y responde. Un médico firma la nota clínica. Un trabajador social decide sobre una solicitud. Un maestro toma la decisión educativa. En estos entornos, la IA toca la administración que rodea la decisión, nunca la decisión en sí.

## Las herramientas

Las herramientas son corrientes, pero se despliegan bajo un conjunto de reglas mucho más estricto.

- **Un sistema de agendamiento y recordatorios** con un chatbot y gestión telefónica para las reservas rutinarias.
- **Una herramienta de documentación ambiental** que redacta las notas de consulta a partir de una conversación grabada, para que el profesional la revise y la firme.
- **Una herramienta de extracción de documentos** que lee cartas y formularios y los enruta.
- **Un chatbot de preguntas** para padres y ciudadanos, que funciona en varios idiomas.

Cómo elegir estas herramientas sin dejarse deslumbrar por una demostración se explica en el [Capítulo 17 — Elegir herramientas sin dejarse engañar](ch17-choosing-tools-without-being-fooled.md). Cómo conectarlas al sistema de pacientes de la clínica o al sistema de expedientes de la oficina está en el [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).

**El listón de cumplimiento es toda la historia aquí.** Los datos de salud y los datos de niños no se pueden pegar en un chatbot público. Estas organizaciones deben usar herramientas que mantengan el dato protegido: un servicio de nivel empresarial con un contrato claro de no entrenamiento y no compartición y un acuerdo de tratamiento de datos, o un modelo ejecutado en sus propias máquinas o en una nube controlada y dentro de la región. El autoalojamiento se explica en el [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md). El peligro de que el personal pegue a escondidas datos sensibles en herramientas públicas —la IA en la sombra— es el tema del [Capítulo 9 — Servicios de terceros e IA en la sombra](ch09-third-party-services-and-shadow-ai.md). Mantener los datos dentro del país o la región, en lugar de en el extranjero, es la pregunta de soberanía del [Capítulo 11 — Soberanía digital](ch11-digital-sovereignty.md). Y las obligaciones legales para esta categoría de datos están en el [Capítulo 10](ch10-privacy-and-gdpr.md) y el [Capítulo 5](ch05-rules-and-legal-responsibility.md).

De ahí se derivan dos reglas prácticas. Primera, **minimización de datos**: recoge y procesa solo lo necesario. Un bot de agendamiento no necesita toda la historia médica de un paciente. Segunda, **rastro de auditoría**: cada acción que toma la IA y cada revisión humana deben quedar registrados, para que la organización pueda demostrar después quién hizo qué.

## Los costos

Aquí hay un presupuesto ilustrativo del primer año para una clínica como Riverside. Son cifras inventadas para mostrar la forma. Usa las tuyas. El trabajo de cumplimiento hace que estos entornos sean más caros de montar que una tienda.

**Costos directos.**
- Sistema de agendamiento y recordatorios: unos €6.000 al año.
- Herramienta de documentación ambiental (conforme, con acuerdo de tratamiento de datos): unos €14.400 al año.
- Extracción y enrutamiento de documentos: unos €7.200 al año.
- Chatbot de preguntas para pacientes: unos €3.600 al año.
- Configuración, integración y el trabajo de cumplimiento (evaluación de impacto en la protección de datos, verificación de proveedores, revisión de seguridad): unos €18.000 de una sola vez.
- Formación del personal: unos €5.000 de una sola vez.

Total del primer año: aproximadamente **€54.200**. En los años estables siguientes, las suscripciones recurrentes suman unos **€31.200**.

**Costos indirectos.**
- Los profesionales dedican tiempo a revisar cada nota redactada. Esta es la red de seguridad y debe quedarse.
- La carga de cumplimiento: una evaluación de impacto en la protección de datos no es gratis, y debe hacerse antes de ponerse en marcha, no después.
- La caída de aprendizaje mientras el personal e incluso los pacientes se adaptan.
- El costo de un error si se confía en un borrador sin revisarlo: en una clínica, esto puede dañar a un paciente, lo cual es mucho peor que una venta perdida.
- La supervisión continua para que las herramientas sigan cumpliendo a medida que cambian las reglas.

El método completo para contar estos costos y convertir el ahorro en una cifra de retorno está en el [Capítulo 16 — Metas, costos y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md). En un entorno regulado, suma el costo del cumplimiento al balance antes de contar cualquier ahorro.

## Los resultados

Después de un año, medido contra una línea base que la clínica registró antes de empezar, el resultado ilustrativo se ve así. Tus números serán distintos. Esto muestra cómo puede verse un buen encaje.

- **Bajaron las ausencias.** Los recordatorios automáticos llevaron a más pacientes a sus citas, así que se desperdiciaron menos turnos y se atendió a más gente.
- **Se acortó la cola telefónica.** El chatbot y la reserva por cuenta propia gestionaron las llamadas rutinarias, así que la recepción pudo concentrarse en los pacientes que necesitaban a una persona.
- **Bajó el tiempo de documentación.** Los médicos pasaron menos tiempo tecleando notas y más con los pacientes, porque partían de un borrador para revisar en lugar de una página en blanco.
- **Los documentos se movieron más rápido.** Las derivaciones y los formularios se clasificaban y enrutaban de forma automática, así que menos quedaban sin leer y menos pacientes se quedaban esperando.
- **Mejoró el acceso.** El asistente de preguntas multilingüe ayudó a padres y ciudadanos que no hablan el idioma local a obtener respuestas sin esperar un intérprete.

La advertencia honesta: nada de esto fue instantáneo. La herramienta de documentación redactaba notas imperfectas al principio y necesitaba que cada médico corrigiera su estilo. El bot de agendamiento malinterpretaba algunas solicitudes al inicio. Las ganancias fueron subiendo con las semanas, como predice la advertencia de la curva de aprendizaje en el [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). La clínica midió los números reales después de la subida, no durante.

## Lecciones aprendidas

**Los datos regulados imponen un listón más alto, desde el primer paso.** Los datos de salud y los de niños son de categoría especial. No puedes tratarlos como la descripción de un producto. Usa herramientas conformes, firma un acuerdo de tratamiento de datos, mantén los datos dentro de la región y haz una evaluación de impacto en la protección de datos antes de ponerte en marcha. Las reglas están en el [Capítulo 10](ch10-privacy-and-gdpr.md) y el [Capítulo 5](ch05-rules-and-legal-responsibility.md).

**Nunca automatices la decisión.** Una herramienta puede redactar una nota clínica, pero un médico la firma y se hace cargo de ella. Una herramienta puede clasificar una solicitud, pero un trabajador social la decide. En estos entornos la IA trabaja en la administración que rodea la decisión y nunca toma la decisión. Esto es una regla de seguridad y, para los usos de mayor riesgo, también una legal bajo la Ley de IA de la UE.

**El consentimiento para grabar no es opcional.** La documentación ambiental graba una conversación. El paciente debe saberlo y estar de acuerdo, de forma clara y por adelantado. No grabes a escondidas. Esto es tratamiento de datos personales según el [Capítulo 10](ch10-privacy-and-gdpr.md).

**La minimización de datos te protege.** Dale a cada herramienta solo los datos que necesita. El bot de agendamiento no necesita la historia clínica completa. Cuantos menos datos sensibles toque una herramienta, menor será el daño si algo sale mal.

**Mantén un rastro de auditoría.** Registra qué hizo la IA y qué revisó el humano. En un entorno regulado, poder mostrar el registro después es tan importante como el resultado mismo.

**Cuidado con la respuesta equivocada pero segura de sí misma.** Una nota redactada que falsea lo que se dijo, o un chatbot que da una instrucción errónea, puede causar un daño real aquí. Un humano debe revisar. El problema de la fiabilidad está en el [Capítulo 2 — La IA explicada de forma sencilla](ch02-ai-explained-simply.md), y el deber de honestidad está en el [Capítulo 4 — IA ética: hacer lo correcto](ch04-ethical-ai-doing-the-right-thing.md).

**La IA puede ampliar el acceso, no solo recortar costos.** El asistente multilingüe y el chatbot siempre abierto ayudaron a personas que de otro modo tienen dificultades para llegar a la oficina. En los servicios públicos, esa equidad es un resultado que vale tanto como el dinero ahorrado.

**Mide con honestidad y espera la subida.** Registra la línea base antes de empezar. Juzga el proyecto después de la curva de aprendizaje, no durante. El método está en el [Capítulo 22 — Medir resultados y ROI](ch22-measuring-results-and-roi.md).

La lección para clínicas, escuelas y oficinas públicas es la misma que la de todos los sectores, con la barrera más estricta de todas: encuentra la carga administrativa —la programación de citas, los documentos, las preguntas repetidas—, deja que la IA redacte, clasifique y responda, mantén un humano formado en cada decisión, protege los datos sensibles como exige la ley y mide con honestidad. El premio no es solo una oficina más barata. Es más tiempo con los pacientes, los estudiantes y los ciudadanos, que es el verdadero sentido del trabajo.
