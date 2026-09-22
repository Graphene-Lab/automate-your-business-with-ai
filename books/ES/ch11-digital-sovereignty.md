# Capítulo 11 — Soberanía digital: el derecho a controlar tu IA

## En palabras simples

Soberanía, en su sentido más antiguo, significa el derecho a gobernarse a uno mismo sin que otro te diga qué hacer. La soberanía digital toma esa idea y la aplica a tu vida digital: el derecho a controlar tus propios datos, tu propio software y las máquinas que los ejecutan.

Aplicada a la IA, la soberanía digital responde tres preguntas llanas sobre cada herramienta de IA que usas.

- **¿Dónde están mis datos?** ¿Qué país, los servidores de qué empresa, bajo qué ley?
- **¿Quién puede acceder a ellos?** ¿El personal del proveedor, subcontratistas, o un gobierno extranjero?
- **¿Cómo se procesan?** ¿En un modelo que no puedo ver, o en un sistema que puedo inspeccionar y cambiar?

Si no puedes responder esas tres preguntas, no tienes soberanía sobre esa parte de tu negocio. Has tomado prestada la de otro, y puedes perderla cuando él cambie de opinión.

Esto no es lo mismo que el autoalojamiento, aunque se solapan. El autoalojamiento, tratado en el [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md), es una forma de ganar control. La soberanía digital es el objetivo más amplio: control sobre de dónde vienen tus capacidades digitales y quién lleva la correa. Puedes perseguirla con tus propios servidores, con software abierto, con contratos, o con una mezcla.

Una analogía útil es la comida. Puedes comprar platos preparados de una fábrica que nunca ves, y la mayoría de los días eso está bien. Pero si tienes una alergia, o simplemente quieres saber qué hay en tu comida, empiezas a interesarte por la receta y la cocina. La soberanía digital es interesarse por la receta y la cocina de tu IA —no por miedo, sino porque lo que está en juego son tus datos, tus clientes y tu futuro—.

El patrón opuesto, los servicios de terceros sin gestionar y la IA en la sombra, está en el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md). Los deberes legales sobre los datos personales están en el [Capítulo 10](ch10-privacy-and-gdpr.md). Este capítulo trata de la decisión estratégica: cuánto de tu IA quieres controlar de verdad.

## Un poco de historia

**Años 2000 a 2010: la conveniencia borra la pregunta.** A medida que las empresas se mudaron a la nube, casi nadie preguntó a dónde iban los datos. Las herramientas eran buenas y baratas. El control no era un criterio de compra.

**2013: Snowden cambia el ánimo.** Las revelaciones sobre la vigilancia masiva hicieron que gobiernos y empresas se dieran cuenta de que los datos almacenados en otro país podían ser alcanzados por las autoridades de ese país. La pregunta «dónde están mis datos» se convirtió en una pregunta de seguridad, no solo de privacidad.

**2018: el RGPD hace que la ubicación importe legalmente.** La ley de privacidad de Europa dio a las personas derechos sobre sus datos e hizo a las empresas responsables de dónde estaban y cómo se manejaban. La residencia de datos —mantener los datos dentro de una región— se convirtió en un requisito real, no un eslogan.

**2019 a 2022: aparece la «nube soberana».** Los proveedores de nube empezaron a ofrecer opciones soberanas: datos guardados en un país concreto, operados bajo ley local, a veces con socios locales. La soberanía se convirtió en una característica de producto.

**2022 a 2023: los modelos de pesos abiertos abren un nuevo camino.** Cuando modelos de IA potentes se volvieron descargables y ejecutables por cualquiera, una empresa pudo, por primera vez, ejecutar un modelo capaz enteramente bajo sus propias condiciones. La soberanía ya no era solo una promesa de un proveedor de nube; se convirtió en algo que podías construir.

**2024 a 2025: la soberanía se vuelve estrategia nacional y corporativa.** Países y bloques empezaron a tratar la capacidad de IA como estratégica. Europa lanzó proyectos financiados para construir sus propios modelos abiertos, para que la IA europea no dependiera por completo de proveedores extranjeros. La sección Curiosidad trata de uno de ellos.

El arco es claro. La conveniencia nos hizo dejar de preguntar quién controla nuestras herramientas. Una serie de conmociones nos hizo preguntar de nuevo. Ahora el control es una decisión de diseño que puedes tomar deliberadamente.

## Curiosidad

### 11.6 Construir tu propio asistente, y un continente haciendo lo mismo

**Un patrón representativo (ilustrativo).** Considera una firma profesional mediana —digamos una consultora de ingeniería o un despacho de abogados— que necesita un asistente de IA interno para responder preguntas sobre sus propios documentos: informes pasados, normas, contratos y notas. Los datos son confidenciales y no pueden salir del edificio.

En lugar de enviar esos datos a un servicio público de IA, la firma hace algo distinto. Descarga un modelo de pesos abiertos —un modelo cuyos archivos entrenados se publican para que cualquiera los ejecute— y lo ejecuta en sus propios servidores. Conecta el modelo a sus documentos mediante recuperación, así que el asistente responde desde los archivos propios de la firma en lugar de desde el internet abierto. Ninguna pregunta sale de la red. Ningún proveedor lee el trabajo. La firma elige el modelo, controla los datos, y puede cambiar o reemplazar el sistema cuando quiera.

Este patrón es real y cada vez más común, pero la firma específica aquí es un compuesto, no una empresa con nombre, porque las organizaciones que hacen esto raramente lo anuncian —todo el sentido es que el trabajo se mantenga privado—. Lo que importa es que el patrón existe y funciona hoy con herramientas abiertas estándar, exactamente como describe el [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md).

**Una versión real y con nombre a escala nacional.** El mismo instinto está impulsando ahora a países enteros. En Europa, dos proyectos financiados apuntan a construir modelos de IA abiertos y soberanos para que el continente no dependa de proveedores extranjeros.

**OpenEuroLLM** es un consorcio europeo de veinte socios que comenzó a trabajar el 1 de febrero de 2025, financiado bajo el Programa Europa Digital de la UE con unos 55 millones de euros. Lo coordina Jan Hajic de la Universidad Carolina y lo codelidera Peter Sarlin de AMD Silo AI. Su objetivo declarado es la autonomía estratégica de Europa en IA —construir capacidad que Europa controle—.

Junto a él, el proyecto **EuroLLM**, respaldado por Horizonte Europa, el Consejo Europeo de Investigación y la organización de supercomputación EuroHPC, produjo **EuroLLM-22B**, un gran modelo de lenguaje totalmente abierto construido para los 24 idiomas oficiales de la UE. Fue entrenado en superordenadores europeos —el sistema MareNostrum 5— y publicado como código abierto en Hugging Face, así que cualquiera puede descargarlo, inspeccionarlo y ejecutarlo. El trabajo se apoya en la iniciativa «AI Factories» de EuroHPC, que agrupa capacidad de supercomputación en toda Europa; una convocatoria asignó tres millones de horas de GPU en el Leonardo Booster del CINECA en Italia para construir datos de entrenamiento abiertos.

¿Por qué contar esta historia aquí? Porque muestra que «construye el tuyo, mantenlo abierto, mantenlo bajo tu control» no es un hobby paranoico. Ahora es estrategia oficial al nivel de las naciones. La misma lógica que lleva a un país a construir su propio modelo abierto lleva a una firma pequeña a ejecutar un modelo abierto en su propio servidor. La escala difiere; el principio es idéntico.

## Un ejemplo empresarial real

### La clínica que no podía enviar sus datos a ninguna parte

Una clínica médica privada quiere usar IA para resumir notas de pacientes y redactar correspondencia rutinaria. Los datos son datos de salud —el tipo más protegido por la ley, como explica el [Capítulo 10](ch10-privacy-and-gdpr.md)—. Enviarlos a un servicio de IA de terceros plantea graves problemas legales y éticos, y la clínica no está cómoda con ello independientemente de la ley.

Así que la clínica elige el control. Ejecuta un modelo abierto en su propio servidor, dentro de su propia red, detrás de su propio cortafuegos. El modelo lee solo las notas de la clínica y responde solo al personal de la clínica. Nada cruza internet hacia un proveedor. La clínica puede decir con verdad a pacientes, reguladores y a su propia conciencia: estos datos nunca salieron de nuestro edificio.

El coste es real. La clínica tuvo que comprar hardware y encontrar a alguien para mantenerlo. El modelo es bueno pero no el mejor absoluto disponible. Algunas tareas aún necesitan un humano. Pero la clínica ganó la única cosa que no podía comprar a ningún proveedor: certeza sobre a dónde van sus datos más sensibles.

Ahora compara la clínica con una firma que no pensó en esto y pegó datos de pacientes en un chatbot gratuito. La diferencia no es inteligencia. Es que una firma hizo las tres preguntas de soberanía primero, y la otra nunca lo hizo.

## Cómo hacerlo

### 11.1 Qué es la soberanía digital: una definición simple

La soberanía digital es la capacidad de controlar tus propios recursos y decisiones digitales, en lugar de depender de los de otro.

Desglosada, tiene tres capas.

**Soberanía de datos.** Controlas dónde se almacenan tus datos, quién puede acceder a ellos, y bajo qué ley caen. Puedes moverlos o borrarlos.

**Soberanía operativa.** Controlas los sistemas que procesan tus datos. Puedes ejecutarlos, cambiarlos y mantenerlos funcionando incluso si un proveedor desaparece.

**Soberanía estratégica.** Controlas tu propio rumbo. Tu futuro no queda rehén del precio de un proveedor, de las reglas de un gobierno extranjero, o de las decisiones de negocio de un suministrador.

La soberanía no es todo o nada. Es un dial, no un interruptor. Puedes ser muy soberano sobre un proceso y casi nada soberano sobre otro. El objetivo es decidir, a propósito, dónde quieres el dial puesto para cada parte de tu negocio, en lugar de derivar hacia lo más conveniente.

Lo opuesto a la soberanía es la dependencia que no elegiste —un estado en el que un cambio en los planes de otro fuerza un cambio en los tuyos—.

### 11.2 Por qué importa para las empresas: saber dónde están los datos, quién accede, cómo se procesan

La soberanía importa porque las tres preguntas tienen consecuencias reales.

**Dónde están los datos.** Los datos almacenados en otro país caen bajo las leyes de ese país. Una autoridad extranjera puede poder obligar al acceso. La ubicación del centro de datos de un proveedor no es un detalle menor; fija el terreno legal sobre el que se sostienen tus datos.

**Quién accede a ellos.** Un servicio de terceros puede permitir que su propio personal, sus equipos de soporte y sus subcontratistas alcancen tus datos, en países que nunca aceptaste. Puede que nunca veas una lista de ellos. Soberanía significa que sabes, o controlas, ese acceso.

**Cómo se procesan.** Si el procesamiento ocurre dentro de un sistema cerrado que no puedes inspeccionar, no puedes verificar qué hace con tus datos ni si es justo. Si tú ejecutas el sistema, puedes mirar dentro.

Esto importa por tres razones prácticas. **Cumplimiento:** leyes como el RGPD exigen que conozcas y controles el manejo de datos. **Seguridad:** cada parte extra con acceso es una oportunidad extra de brecha. **Continuidad de negocio:** si un proveedor falla, sube precios, o queda cortado por sanciones, la soberanía es la diferencia entre un contratiempo y una crisis.

La soberanía no es una ideología. Es gestión de riesgo para la parte de tu negocio que funciona con datos.

### 11.3 Modelos propietarios frente a modelos de código abierto: qué cambia de verdad

La elección entre un modelo propietario y un modelo de código abierto cambia varias cosas a la vez.

**Un modelo propietario** es un producto cerrado. Lo usas a través de un servicio o una API. No puedes ver cómo funciona, no puedes ejecutarlo tú mismo, y no puedes cambiarlo. Dependes del dueño para el acceso, el precio y la continuidad. La conveniencia es alta; el control es bajo. Si el dueño cambia las condiciones o detiene el servicio, te adaptas o te detienes.

**Un modelo de código abierto o de pesos abiertos** publica su código o sus archivos entrenados para que puedas descargarlo y ejecutarlo tú mismo. Puedes inspeccionarlo, ejecutarlo en tu propio hardware, ajustarlo fino, y seguir usándolo incluso si el creador original desaparece. El control es alto; la conveniencia es menor, porque debes ejecutarlo y mantenerlo.

Lo que cambia de verdad es **quién tiene el poder y quién carga con la carga.** Lo propietario entrega el poder al proveedor y lleva la carga por ti. Lo abierto te entrega el poder y te da la carga.

Ninguno es automáticamente mejor. Lo propietario es correcto cuando quieres capacidad sin mantenimiento y los datos no son sensibles. Lo abierto es correcto cuando necesitas control, transparencia o independencia, y puedes sostener el trabajo. Muchos negocios usan ambos: propietario para la conveniencia de bajo riesgo, abierto y autogestionado para los datos y procesos que más importan.

Una precaución: «abierto» es un espectro, y la licencia importa. Algunos modelos abiertos restringen el uso comercial o cómo puedes describir tu uso. Lee la licencia antes de construir sobre ella.

### 11.4 El papel del código abierto: transparencia, control, comunidad

El código abierto es la herramienta principal de la soberanía digital, por tres razones.

**Transparencia.** Como el código o los pesos están publicados, tú o un tercero podéis leerlos y comprobar qué hace realmente el sistema. No se os pide confiar en una caja negra. Es el mismo instinto detrás de las ideas de auditoría del [Capítulo 7](ch07-trustless-trust-without-trusting.md).

**Control.** Puedes ejecutarlo donde elijas, cambiarlo para que se ajuste a tus necesidades, y conservarlo todo el tiempo que quieras. Nadie puede quitártelo ni forzarte una actualización que no pediste.

**Comunidad.** Un proyecto abierto lo mantiene mucha gente, no la hoja de ruta de una sola empresa. Los errores los encuentran personas externas. El proyecto puede sobrevivir al equipo original. No estás solo si algo se rompe.

El código abierto también baja la barrera de entrada. Una firma pequeña puede usar el mismo modelo abierto que una grande. Eso iguala el terreno de una forma que los productos propietarios no hacen.

Pero el código abierto no es gratis en el sentido real. Alguien debe instalarlo, actualizarlo, asegurararlo y darle soporte. Si no tienes a nadie para hacerlo, el código abierto puede volverse un pasivo. Una soberanía que no puedes mantener es peor que una dependencia cómoda. Usa código abierto donde tengas, o puedas contratar, la capacidad.

### 11.5 Cómo construir una infraestructura de IA soberana: los pasos concretos

Si decides ganar control, aquí hay un camino práctico.

1. **Decide qué debe ser soberano.** Enumera los datos y procesos que no pueden depender de externos —datos sensibles, flujos de trabajo centrales, trabajo regulado—. No todo necesita el tratamiento.
2. **Elige modelos abiertos.** Escoge modelos de pesos abiertos cuya licencia encaje con tu uso. Ajusta el tamaño a tu tarea, como explica el [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md).
3. **Ejecútalos en infraestructura que controles.** Eso puede ser un servidor en tu oficina, una máquina en tu propia cuenta de nube bajo tus propias llaves, o una estación de trabajo local para un comienzo pequeño.
4. **Mantén los datos locales y conectados.** Usa recuperación para que el asistente responda desde tus propios documentos sin enviarlos fuera.
5. **Controla el acceso y las llaves.** Tú tienes las credenciales. Ningún tercero tiene una puerta trasera. Registra quién hace qué.
6. **Planifica el mantenimiento.** Nombra quién instala, actualiza, asegura y hace copias de seguridad del sistema. Escribe el manual de operación.
7. **Mantén una salida de todo.** Incluso para las partes que mantengas propietarias, asegúrate de poder exportar datos y cambiar de herramientas. La soberanía incluye la capacidad de irse.
8. **Revisa el terreno legal.** Confirma la residencia de datos y los deberes del Reglamento de IA y del RGPD para la configuración, como cubren el [Capítulo 5](ch05-rules-and-legal-responsibility.md) y el [Capítulo 10](ch10-privacy-and-gdpr.md).
9. **Empieza pequeño y crece.** Prueba en piloto un flujo soberano, demuestra que funciona, y luego amplía. No reconstruyas toda la empresa de golpe.

El objetivo no es la independencia total. Es el control deliberado sobre las partes que importan, con una línea clara entre lo que ejecutas y lo que alquilas.

## Ética y responsabilidad

La soberanía conlleva sus propios deberes éticos, y es fácil equivocarse con ellos.

**Control no es lo mismo que bondad.** Un sistema soberano puede seguir siendo sesgado, erróneo o injusto. Ejecutarlo tú mismo no lo vuelve ético. Los deberes del [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md) siguen aplicando.

**La soberanía no debe volverse secretismo.** «Nosotros lo controlamos» no es una razón para esconder cómo tratas los datos de la gente. Aún debes transparencia a clientes y reguladores. Controla el sistema; no te escondas del escrutinio.

**No uses la soberanía para esquivar la cooperación.** Algunos problemas —fraude, daño, peticiones legales— requieren trabajar con las autoridades. La soberanía trata de proteger a los inocentes, no de bloquear la supervisión legítima.

**Sé honesto sobre tus límites.** Si alegas soberanía total pero no puedes parchear, respaldar ni auditar el sistema, la afirmación es vacía y engañosa. Di qué controlas y qué no.

**Sopesa el bien colectivo.** Los modelos abiertos y la investigación compartida benefician a todos. Un mundo donde cada firma construye un silo cerrado pierde algo. El enfoque más sano es controlar lo sensible y contribuir a lo compartido.

## Errores a evitar

### 11.7 Soberanía por sí misma

El error más común es perseguir la soberanía como un ideal en lugar de una herramienta.

La soberanía cuesta dinero, tiempo y habilidades. Si la persigues en todas partes, gastas mucho en controlar cosas que nunca necesitaron control. Podrías construir un caro sistema local para datos que nunca fueron sensibles, mientras un servicio barato y contratado te habría servido bien y liberado a tu gente para trabajo real.

La prueba no es «¿puedo controlar esto?». Es «¿qué pierdo si no puedo controlar esto?». Si la respuesta es poco, no gastes en controlarlo. Guarda tu presupuesto de soberanía para los datos y procesos donde perder el control dolería de verdad —datos sensibles, trabajo regulado, y los sistemas sin los que tu negocio no puede funcionar—.

La soberanía es un medio, no un fin. Cómprala donde el riesgo justifique el coste, y sé cómodamente dependiente donde no.

Más allá de esa trampa, vigila estas:

1. **Construir una fortaleza que no puedes mantener.** Soberanía sin un mantenedor se convierte en un sistema roto y una falsa sensación de seguridad.
2. **Confundir código abierto con gratis.** Alguien debe ejecutarlo. Presupuesta para eso.
3. **Ignorar la licencia.** Abierto no siempre significa que puedas usarlo como te plazca.
4. **Suponer que local equivale a seguro.** Un servidor soberano aún necesita seguridad, como cubre el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).
5. **Cortar con todos los proveedores por principio.** Muchos proveedores se ganan su lugar. La independencia total raramente vale la pena.
6. **Sin plan de salida para las partes que mantengas alquiladas.** La soberanía incluye la capacidad de dejar a cualquier proveedor único.
7. **Sobreprometer a los clientes.** No alegues un control que no tienes.
8. **Ignorar que los modelos abiertos aún pueden filtrar.** Un modelo entrenado con datos malos aún puede exponer datos personales, como señala el [Capítulo 10](ch10-privacy-and-gdpr.md).

## Ejercicio práctico

### 11.8 Define tu nivel deseado de soberanía

Tómate una hora y mapea tus usos de IA sobre un simple dial de control.

Enumera cada uso de IA en tu negocio. Para cada uno, responde tres preguntas y fija un nivel objetivo.

- **¿Cuán sensible es el dato?** Bajo (público o inofensivo), Medio (interno), Alto (confidencial de cliente, regulado o personal).
- **¿Cuán crítico es el proceso?** Bajo (gusto tenerlo), Medio (usado a diario), Alto (el negocio se detiene sin él).
- **¿Cuál es el coste de perder el control?** Bajo, Medio o Alto.

Ahora fija un objetivo para cada uno:

- **Alta sensibilidad o alta criticidad → apunta alto.** Ejecútalo tú mismo o bajo un contrato que te dé control real y una salida.
- **Baja sensibilidad y baja criticidad → apunta bajo.** Un servicio de terceros conveniente está bien; no desperdicies dinero controlándolo.
- **Mixto → apunta al medio.** Usa un proveedor pero mantén los datos exportables y el flujo de trabajo intercambiable.

Escribe una frase por uso: *«Para [uso], quiero soberanía [alta/media/baja] porque [razón].»*

El resultado es tu mapa de soberanía. Debería mostrar una mezcla deliberada, no una sola respuesta. Si todo es «alto», estás gastando de más. Si todo es «bajo», estás expuesto en las cosas que importan. Ajusta hasta que el mapa coincida con tu riesgo real.

## Lista de comprobación

### 11.9 Los pilares de la soberanía digital

Usa esto para comprobar si una configuración de IA dada te da control real.

- [ ] **Sabes dónde se almacenan los datos** —el país y el operador—.
- [ ] **Sabes quién puede acceder a ellos** —personal del proveedor, subcontratistas y cualquier alcance gubernamental—.
- [ ] **Puedes mover o borrar los datos** cuando elijas.
- [ ] **Puedes exportar tus datos** en un formato común y utilizable (sin bloqueo).
- [ ] **Sabes cómo se procesan los datos** —o tú ejecutas el procesamiento—.
- [ ] **Usas modelos abiertos donde el control importa**, y has leído sus licencias.
- [ ] **Tú tienes las llaves y credenciales** de los sistemas que importan.
- [ ] **Tienes un mantenedor con nombre** para todo lo que ejecutas tú mismo, con un manual de operación escrito.
- [ ] **Tienes un plan de salida** para cada proveedor, para que ningún proveedor único pueda tomarte como rehén.
- [ ] **Has revisado el terreno legal** —residencia de datos, RGPD y Reglamento de IA—.
- [ ] **Has fijado un nivel de soberanía deliberado** para cada uso, no un valor por defecto.
- [ ] **Puedes verificar tus propias afirmaciones** —si dices que los datos se quedan dentro, puedes probarlo—.

Si falta un pilar para un uso de alto riesgo, esa es tu prioridad a arreglar.

## Puntos clave

- La soberanía digital significa controlar dónde están tus datos, quién accede a ellos y cómo se procesan —y poder responder esas tres preguntas para cada herramienta de IA—.
- Es un dial, no un interruptor: ponlo deliberadamente alto para el trabajo sensible y crítico, y bajo donde la conveniencia es inofensiva.
- Los modelos de código abierto y de pesos abiertos te dan transparencia, control y comunidad, pero solo si tienes la capacidad de ejecutarlos y mantenerlos.
- La soberanía es un medio, no un fin; perseguirla en todas partes desperdicia dinero, así que cómprala solo donde perder el control dolería de verdad.
- La soberanía real siempre incluye una salida: mantén tus datos exportables para que ningún proveedor único pueda tener tu negocio como rehén.
