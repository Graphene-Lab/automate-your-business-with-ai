# Capítulo 9 — Servicios de terceros e IA en la sombra

## En palabras simples

Un servicio de IA de terceros es cualquier IA que usas y que funciona en los ordenadores de otra persona. Escribes una pregunta o subes un archivo. Viaja por internet hasta sus máquinas. Su software hace el trabajo. La respuesta vuelve. Nunca ves lo que hay dentro.

Así es como la mayoría de las empresas usan la IA hoy. Es fácil, es barato para empezar y es potente. Por eso casi todo el mundo la usa.

También tiene un coste oculto. En el momento en que tu texto sale de tu edificio, pierdes el control directo sobre él. Ahora dependes de una empresa que no has diseñado, de unas reglas que no has escrito, de un servidor que no puedes inspeccionar.

La "IA en la sombra" es la segunda parte de esta historia. IA en la sombra significa que los empleados usan herramientas de IA sin que la empresa lo sepa, lo apruebe o lo supervise. Una ayudante de marketing pega una lista de clientes en un chatbot gratuito. Un contable deja caer una factura en una aplicación web para resumirla. Nadie a cargo sabe que está pasando. Los datos se han ido, y no hay registro, ni contrato, ni control.

Piénsalo como la impresora de la oficina hace veinte años. Todos la usaban. Nadie sabía que guardaba una copia de cada página. La IA en la sombra es la misma sorpresa, pero las páginas son tus listas de clientes, tus contratos y tus precios.

Este capítulo trata de dos cosas: qué le pasa realmente a tus datos cuando usas un servicio de terceros, y cómo evitar que tu propio personal cree riesgo en silencio. El patrón opuesto —hacer funcionar la IA en tus propias máquinas— se trata en el [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md). El lado legal de los datos personales es el tema central del [Capítulo 10](ch10-privacy-and-gdpr.md). La pregunta más amplia sobre controlar tus propias herramientas es el [Capítulo 11](ch11-digital-sovereignty.md).

## Un poco de historia

**Años 90 y 2000: el software sale de la estantería.** Antes comprabas un programa en un CD y lo hacías funcionar en tu propio ordenador. Luego el correo, los calendarios y el almacenamiento de archivos se mudaron a internet. Dejaste de ser dueño del software y empezaste a alquilar acceso a él.

**Años 2000 a 2015: el SaaS se vuelve normal.** "Software como Servicio" significaba pagar una cuota mensual para usar el software de otro por la web. Salesforce, Google Workspace y Microsoft 365 lo hicieron corriente. La conveniencia ganó. La mayoría de las pequeñas empresas dejaron de gestionar sus propios servidores.

**2016 a 2022: los datos se van con el software.** Una vez que tus registros de clientes, documentos y mensajes vivieron en la nube de un proveedor, los datos de tu negocio quedaron permanentemente fuera de tus muros. La mayoría lo aceptó porque las herramientas eran buenas y el precio era bajo.

**Noviembre de 2022: ChatGPT abre la puerta a todos.** Una IA potente quedó disponible en una caja web gratuita. Ya no necesitabas un contrato con un proveedor para usar IA. Solo necesitabas una dirección de correo. Este es el momento en que empezó la IA en la sombra, porque un solo empleado podía enviar ahora datos de la empresa a un modelo de frontera sin pedirle permiso a nadie.

**2023: las primeras alarmas corporativas.** Las empresas descubrieron que el personal pegaba material confidencial en chatbots públicos. El caso de Samsung, en la sección Curiosidad, es el más famoso. Varios bancos y firmas profesionales prohibieron o restringieron herramientas de IA públicas ese año.

**2023 a 2026: los proveedores añaden niveles "empresariales".** En respuesta, los proveedores de IA vendieron planes de negocio que prometían no entrenar con tus datos, mantener los datos separados y añadir controles de administración. La conveniencia se quedó; las promesas mejoraron. Pero una promesa no es lo mismo que el control, y por eso importa este capítulo.

## Curiosidad

### 9.7 La empresa de semiconductores que pegó sus secretos en ChatGPT

A principios de 2023, Samsung Electronics —una de las empresas de tecnología más grandes del planeta— descubrió que sus propios ingenieros habían puesto material confidencial en un chatbot de IA público.

La información, publicada por primera vez por el diario financiero coreano *Korea Economic Daily* en abril de 2023 y repetida ampliamente, describía tres incidentes separados dentro de la división de semiconductores. En el primero, un ingeniero pegó código fuente defectuoso de un programa usado para descargar datos de medición de una fábrica de chips, esperando que el chatbot encontrara el fallo. En el segundo, el personal subió código relacionado con equipos de semiconductores y detección de defectos. En el tercero, los empleados introdujeron transcripciones grabadas de reuniones en la herramienta para obtener resúmenes. Todo esto ocurrió en unas tres semanas desde que la división permitió por primera vez el acceso a la herramienta.

Una vez que los datos estuvieron dentro del chatbot, estaban en máquinas que Samsung no poseía. La empresa no podía recuperarlos con facilidad, y no podía estar segura de que no serían usados o vistos por otros.

La respuesta de Samsung fue directa. Prohibió las herramientas de IA generativa, incluido ChatGPT, en ordenadores, tablets, teléfonos de propiedad de la empresa y su red interna. Incumplir la regla podía llevar a medidas disciplinarias hasta el despido. Se dijo a los empleados que usaban tales herramientas en dispositivos personales que nunca enviaran información de la empresa ni datos personales que pudieran revelar la propiedad intelectual de Samsung. Una encuesta interna encontró que el 65% de los encuestados creía que los servicios de IA suponían un riesgo de seguridad. Al mismo tiempo, Samsung dijo que estaba construyendo sus propias herramientas internas de IA para traducción, resumen de documentos y desarrollo de software, y trabajando en formas de bloquear la subida de información sensible a servicios externos.

La lección no es que Samsung fuera descuidado. Es que si una empresa con miles de millones en presupuesto de seguridad fue tomada por sorpresa por un chatbot gratuito, una pequeña empresa sin equipo de seguridad tiene aún menos protección. La conveniencia es real, y también la filtración.

## Un ejemplo real de negocio

### La agencia que perdió su lista de clientes dos veces

Considera una pequeña agencia de marketing, veinte personas, sin departamento de TI. Esta es una historia compuesta, pero cada parte ocurre cada semana en firmas reales.

Primera filtración: una ejecutiva de cuentas senior quiere reescribir una propuesta rápido. Abre un chatbot de IA gratuito en su portátil y pega el borrador, que incluye el nombre no publicado de un producto de un cliente, cifras de presupuesto y datos de contacto. Consigue un párrafo más bonito. Nunca piensa a dónde fue el texto.

Segunda filtración: la misma ejecutiva, un mes después, se registra en un "asistente de escritura con IA" de pago que promete mejores resultados. Para configurarlo, lo conecta al correo y a la unidad compartida de la agencia para que "aprenda la voz de la empresa". Ahora el proveedor puede leerlo todo: cada cliente, cada contrato, cada broma interna que se convierte en una nota de estrategia.

Entonces llega el problema de la evolución. Un año después el proveedor cambia su plan. Las funciones por las que pagó se mueven a un nivel superior. El precio se duplica. El modelo detrás de la herramienta se cambia por uno más nuevo, y el estilo de escritura con el que entrenó a su equipo cambia en silencio. Quiere irse, pero todo está conectado a esa herramienta. Cambiar significa reconectar toda la agencia en otro sitio y reentrenar a todos. Eso es dependencia del proveedor, y ocurrió sin una sola mala decisión —solo una serie de decisiones convenientes.

Nada de esto requirió maldad. Requirió conveniencia y la ausencia de una regla. La solución no es temer a la IA. Es decidir, de antemano, qué datos pueden ir a dónde, y dar a la gente una buena herramienta para que no recurra a una arriesgada.

## Cómo hacerlo

### 9.1 La conveniencia de los servicios en la nube: por qué los usa todo el mundo

La IA de terceros es popular por razones honestas, y deberías nombrarlas antes de argumentar en su contra.

No hay configuración. No compras hardware, ni contratas un ingeniero, ni instalas nada. Abres una página web y empiezas. Para una pequeña empresa sin personal técnico, ese es todo el atractivo.

No hay coste inicial. La mayoría de las herramientas tienen un nivel gratuito o una cuota mensual baja. Puedes probar una idea por el precio de un café en vez de una compra de capital.

La calidad es alta. Los mejores modelos del mundo están detrás de estos servicios. Una firma de dos personas puede usar la misma capacidad que una gran corporación.

Escala al instante. ¿Necesitas hacer diez veces más trabajo hoy? Las máquinas del proveedor lo absorben. Tú no haces nada.

Por eso la IA en la nube se extendió más rápido que cualquier tecnología anterior. El punto de este capítulo no es quitarte eso. Es que la uses con los ojos abiertos, porque cada una de esas conveniencias se compra con un trozo de control que no notaste que estabas vendiendo.

### 9.2 Qué le pasa a tus datos cuando salen de la empresa

Cuando pegas texto en una IA de terceros, pueden pasar varias cosas, y normalmente no puedes ver cuáles.

Tus datos cruzan internet hasta los servidores del proveedor, a menudo en otro país. Una vez allí, se almacenan, al menos durante un tiempo, en hardware que no controlas y no puedes inspeccionar.

Puede que lo lean sistemas automatizados para un filtrado de seguridad. Puede que se registre para depuración. Personal de soporte en otro país puede poder verlo. Nada de esto es inusual; así operan los servicios grandes.

Lo más importante, puede que se use para entrenar el modelo del proveedor. "Entrenar" significa que la empresa introduce tu texto en su sistema para que el modelo aprenda de él. Si eso ocurre, un fragmento de tu texto confidencial puede dar forma a las respuestas que se dan a otros clientes. Esta es la razón más grande para tener cuidado.

Algunos planes de negocio prometen no entrenar con tus datos. Esa promesa vale algo, pero es una cláusula de contrato, no un muro. Confías en que el proveedor la cumpla en cada producto y cada país. La regla segura es simple: trata cualquier IA de terceros como si todo lo que envíes pudiera hacerse público. Si ese pensamiento es inaceptable para un archivo dado, no envíes ese archivo.

### 9.3 El problema de la transparencia: nunca sabes realmente cómo se usan tus datos

No puedes ver dentro de un servicio de IA de terceros. Este es el problema central, y no va a desaparecer.

No sabes qué modelo te respondió. Los proveedores cambian de modelo sin avisarte. No sabes dónde se almacenaron tus datos, quién podía acceder a ellos, ni cuánto tiempo se guardaron. No sabes si un subcontratista en otro país los procesó. No sabes si se usaron para entrenamiento, incluso cuando crees que no.

La política de privacidad del proveedor la escriben abogados, no ingenieros, y describe lo que pueden hacer, no lo que harán en tu caso concreto. Leerla rara vez da una respuesta clara.

Por eso la prueba práctica es tan útil. En vez de intentar entender el sistema, hazte una pregunta sobre los datos: *¿sería aceptable si esto se hiciera público mañana?* Para una entrada de blog pública, sí. Para el archivo de salarios de un cliente, no. Esa única prueba reemplaza mil preguntas que no puedes responder.

Si necesitas transparencia real, la única fuente honesta es un sistema que puedas inspeccionar —tu propia máquina, o software abierto que alguien pueda auditar. Ese es el tema del [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md) y del [Capítulo 11](ch11-digital-sovereignty.md).

### 9.4 El problema de la evolución: los modelos cambian, los contratos cambian, los precios cambian

Un servicio de terceros no es algo que compras; es una relación que sigue cambiando bajo tus pies.

El modelo cambia. La herramienta de hoy puede funcionar con un modelo distinto el próximo trimestre. Las respuestas cambian. El estilo cambia. Algo que funcionaba bien en tu flujo de trabajo puede empeorar, o simplemente ser diferente, sin aviso y sin forma de quedarse en la versión antigua.

El contrato cambia. Los términos que aceptaste al registrarte pueden actualizarse. Funciones en las que confiabas pueden moverse detrás de un plan superior. La promesa sobre los datos de entrenamiento puede reformularse.

El precio cambia. Una herramienta barata que ya has conectado a tu negocio puede subir su precio, y te enfrentas a una elección dolorosa: pagar más, o arrancar todo.

Este es el riesgo oculto de la conveniencia. Construyes sobre un terreno que otro controla, y pueden mover el terreno cuando quieran. La defensa es mantener tus datos importantes y tus flujos de trabajo centrales portables, y no dejar nunca que un solo proveedor sea el único lugar donde puede ocurrir tu trabajo.

### 9.5 Dependencia del proveedor: lo difícil que es cambiar de proveedor después

Dependencia del proveedor significa que irse de un proveedor es tan costoso, en tiempo, dinero o disrupción, que no puedes hacerlo de forma realista. Estás "atrapado".

Ocurre de tres maneras. **Dependencia de datos:** tus datos se guardan en un formato que solo ese proveedor lee bien, o no puedes exportarlos limpiamente. **Dependencia de flujo de trabajo:** tu proceso diario está construido alrededor de esa herramienta, así que cambiar significa reentrenar a todos y rehacer plantillas. **Dependencia de integración:** la herramienta está conectada a tu correo, tu CRM, tus archivos, y sacarla rompe todos esos enlaces.

La dependencia le da poder al proveedor sobre ti. Saben que irse es difícil, lo que debilita tu posición cuando suben precios o cambian términos.

Para seguir libre, exige tres cosas desde el principio. Primero, tus datos deben ser exportables en un formato sencillo y común. Segundo, guarda tus datos centrales en algún lugar que controles, y deja que el proveedor trabaje sobre una copia. Tercero, diseña tu flujo de trabajo de modo que la IA sea un paso, no toda la máquina, para poder intercambiar el paso. El objetivo no es evitar proveedores. Es poder irte de uno en una semana, no en un año.

### 9.6 IA en la sombra: cuando los empleados usan herramientas no autorizadas

La IA en la sombra es el riesgo que no puedes ver, porque lo crea tu propio personal de confianza.

Ocurre porque las buenas herramientas oficiales tardan en aprobarse, mientras que las herramientas gratuitas arriesgadas son instantáneas. Un empleado bajo presión de tiempo pega un correo de un cliente en un chatbot gratuito para redactar una respuesta. Nadie lo detiene, porque nadie lo sabe.

Por qué es peligroso: los datos se van sin contrato, sin revisión y sin registro. No puedes decírselo al cliente, no puedes encontrar los datos después, y no puedes probar qué pasó. Si la herramienta entrena con esos datos, tu información confidencial puede acabar dando forma a un modelo público.

Cómo detectarla: cargos inusuales en tarjetas corporativas por suscripciones de IA; quejas del personal de que las herramientas aprobadas son demasiado lentas; mejoras "mágicas" súbitas en los resultados que ninguna herramienta aprobada explica.

Cómo detenerla: no solo prohibas. Una prohibición sin una buena alternativa solo empuja el comportamiento a la clandestinidad. Dale a la gente una herramienta aprobada que sea rápida y suficientemente buena, y la usarán. Luego deja clara la regla, entrena sobre ella y supervisa de forma ligera. El lado completo de la política está en la sección 9.8 y en las plantillas de política de IA de la empresa en los apéndices del libro.

### 9.8 Cómo mitigar los riesgos: diligencia debida, contratos y política interna

Reducir el riesgo con tres capas. Haz las tres.

**Capa 1: Diligencia debida — comprueba antes de comprar.**
Antes de adoptar cualquier proveedor de IA, haz las preguntas difíciles. ¿Dónde se almacenan los datos, y en qué países? ¿Entrenan con datos de clientes, y pueden garantizar por escrito que no lo harán? ¿Quién puede acceder a ellos, incluidos los subcontratistas? ¿Cuánto tiempo se guardan, y cómo se borran? ¿Están cifrados en tránsito y en reposo? ¿Qué certificaciones tienen? Consigue las respuestas por escrito, no en una llamada de ventas. Un proveedor que no puede responder con claridad te está diciendo algo. Una versión puntuada de estas preguntas está en la tarjeta de diligencia debida de proveedores en los apéndices.

**Capa 2: Contratos — pon las promesas sobre el papel.**
Una garantía verbal no vale nada. En el contrato, exige: sin entrenamiento con tus datos; residencia de datos en un país que aceptes; el derecho a exportar todos tus datos en un formato utilizable; el derecho al borrado; el deber de avisarte sobre brechas y sobre cambios importantes de modelo o de términos; y límites en los subcontratistas. Si el proveedor no firma esto, esa es tu respuesta.

**Capa 3: Política interna — di a tu gente las reglas.**
Escribe una política de IA corta y clara. Di qué herramientas están aprobadas. Di qué datos nunca pueden entrar en ninguna IA externa —datos personales de clientes, registros financieros, contratos, código fuente, contraseñas—. Da al personal una herramienta aprobada y rápida para que no recurra a una arriesgada. Entrena a todos con la regla en una sesión corta. Revisa la lista de herramientas aprobadas cada trimestre. Una plantilla está en los apéndices.

El orden importa. Comprueba primero, contrata segundo, política tercero. La mayoría de las empresas se saltan las dos primeras y se preguntan por qué quedaron expuestas.

## Ética y responsabilidad

La IA de terceros plantea un deber que debes a dos grupos: las personas cuyos datos guardas, y tu propio personal.

**A tus clientes y empleados.** Cuando un cliente te da datos personales, confía en que los protejas. Enviar esos datos a una IA de terceros que no has verificado puede romper esa confianza, incluso si no pasa nada malo. Eres responsable de a dónde van sus datos. Los deberes legales se exponen en el [Capítulo 10](ch10-privacy-and-gdpr.md); el principio ético es simple —no pongas la información privada de alguien en un lugar donde no pondrías la tuya—.

**A tu personal, sobre la IA en la sombra.** Ten cuidado de no convertir la protección en vigilancia. Si supervisas el uso de IA, dile a la gente qué supervisas y por qué. Una regla clara más una buena herramienta es justo. La vigilancia secreta de personal de confianza daña la moral y la confianza. Apunta a barandillas de protección, no a un estado policial.

**Sé honesto sobre lo que no controlas.** Si un cliente pregunta si sus datos entrenan un modelo externo, deberías poder responder con la verdad. Si no lo sabes, dilo, y arreglalo. Afirmar una seguridad exagerada es peor que admitir un hueco.

## Errores a evitar

1. **Leer la demo, no el flujo de datos.** Una demo elegante no te dice nada sobre a dónde van tus datos. Haz primero las preguntas de almacenamiento y entrenamiento.
2. **Confiar en un "no entrenamos con tus datos" verbal.** Si no está en el contrato, no existe.
3. **Conectar una herramienta a toda tu unidad.** "Aprender nuestra voz" a menudo significa "leerlo todo". Dale a la herramienta lo mínimo que necesita.
4. **Prohibir la IA en la sombra sin alternativa.** Una prohibición sin una buena herramienta aprobada solo esconde el comportamiento.
5. **Sin política escrita.** Si la regla no está escrita y entrenada, no es una regla.
6. **Ignorar la pregunta del país.** Los datos almacenados bajo un sistema legal distinto pueden ser accedidos de forma distinta. Sabes dónde están.
7. **Suponer que un plan de pago equivale a seguridad.** Un plan de consumo de pago no es lo mismo que un plan empresarial contratado con los términos correctos.
8. **Sin plan de exportación.** Si no puedes sacar tus datos, estás atrapado desde el primer día.
9. **Tratar la política de privacidad como una garantía.** Enumera lo que pueden hacer, no lo que harán por ti.
10. **Olvidar al humano.** La filtración casi siempre empieza con una persona bajo presión de tiempo. Arregla la presión y da un camino seguro.

## Ejercicio práctico

### 9.9 Analiza tus proveedores de IA actuales

Toma una hora y haz esto con cada herramienta de IA que tu empresa usa hoy, incluidas las que el personal usa en silencio.

Haz una tabla. Una fila por herramienta. Columnas:

- **Nombre de la herramienta** y quién se registró en ella.
- **Qué datos entran.** Sé específico: correos de clientes, facturas, contratos, código, texto público.
- **Dónde se almacena,** si lo sabes. Si es desconocido, escribe "desconocido".
- **¿Entrenan con nuestros datos?** Sí / No / Desconocido.
- **¿Hay un contrato,** o solo una aceptación al hacer clic?
- **¿Podemos exportar nuestros datos?** Sí / No / Desconocido.
- **Nivel de riesgo** para los datos que realmente pones en ella: Bajo / Medio / Alto.

Ahora lee las filas de riesgo Alto. Para cada una, pregúntate: ¿sería aceptable si estos datos se hicieran públicos? Si no, tienes tres opciones —dejar de poner esos datos en ella, pasar a un proveedor que firme los términos correctos, o mover esa tarea a una herramienta que controles (ver [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md))—.

Por último, pregunta por ahí. Envía un mensaje honesto a tu equipo: "¿Qué herramientas de IA usáis para el trabajo de las que no hemos hablado?" Las respuestas son tu lista real de IA en la sombra. No castigues la honestidad; arregla los huecos que revela.

## Lista de comprobación

### 9.10 Preguntas que hacer a cada proveedor de IA

Antes de poner cualquier dato real en un servicio de IA de terceros, consigue una respuesta escrita a cada una de estas.

- [ ] **¿Dónde se almacena físicamente nuestros datos,** y en qué países?
- [ ] **¿Entrenan sus modelos con nuestros datos?** ¿Pueden comprometerse a decir "no" en el contrato?
- [ ] **¿Quién puede acceder a nuestros datos,** incluidos empleados y subcontratistas, y desde dónde?
- [ ] **¿Cuánto tiempo guardan nuestros datos,** y cómo conseguimos que se borren?
- [ ] **¿Están cifrados nuestros datos** tanto en tránsito como almacenados?
- [ ] **¿Podemos exportar todos nuestros datos** en cualquier momento, en un formato común y utilizable?
- [ ] **¿Nos avisarán** de una brecha de datos, y en cuánto tiempo?
- [ ] **¿Nos avisarán** antes de cambiar el modelo, el precio o los términos?
- [ ] **¿Qué certificaciones de seguridad** tienen, y pueden mostrarlas?
- [ ] **¿Hay subcontratistas,** y están vinculados por los mismos términos?
- [ ] **¿Cuál es nuestro recurso legal** si hacen mal uso de nuestros datos?
- [ ] **¿Hay una consola de administración** para que podamos ver y controlar el uso?

Si un proveedor no puede responder esto con claridad y por escrito, trata la herramienta como de alto riesgo y mantén los datos sensibles fuera de ella.

## Puntos clave

- Un servicio de IA de terceros funciona en los ordenadores de otro, así que en el momento en que tus datos se van, cambias control por conveniencia.
- El mayor riesgo es que tus datos confidenciales puedan usarse para entrenar un modelo que sirve a otros, y a menudo no puedes verlo ni detenerlo.
- Los proveedores cambian modelos, contratos y precios bajo tus pies, y la dependencia hace costoso irse —así que mantén tus datos exportables y tu flujo de trabajo intercambiable—.
- La IA en la sombra es tu propio personal usando herramientas no aprobadas; detenla con una buena herramienta aprobada más una regla escrita clara, no solo con prohibiciones.
- Protégete en tres capas: comprueba el proveedor primero, pon las promesas en un contrato segundo, y establece una política interna tercero.
