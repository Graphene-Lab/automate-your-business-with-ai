# Capítulo 19 — Conectar la IA a los sistemas que ya usas

## En palabras simples

Tu negocio ya funciona con software: el sistema que registra tus clientes, el correo que respondes, las hojas de cálculo en las que vives, el programa de contabilidad desde el que facturas. La IA es más útil cuando se enchufa a estos sistemas existentes en vez de quedarse en un rincón sin hacer nada. Este capítulo trata de esa conexión —cómo habla la IA con las herramientas que ya tienes.

La idea clave es la **integración**: un enlace que deja que un software pase información a otro automáticamente. Cuando tu IA puede leer tu lista de clientes, redactar una respuesta en tu bandeja de entrada y escribir una nota de vuelta en tus registros, se convierte en un ayudante real. Cuando no puede conectarse a nada, es solo una ventana de chat lista a la que tienes que copiar y pegar.

Una buena analogía es la fontanería. Un filtro de agua nuevo es inútil si no está conectado a tus tuberías. El valor viene de la conexión, no del filtro a secas. Las integraciones son las tuberías que dejan que la IA fluya a tu trabajo diario. Tu trabajo es entender qué tuberías existen, cuáles puedes conectar tú mismo, y cuándo necesitas un fontanero.

Este capítulo mira los sistemas comunes a los que se conecta la IA —software de gestión, CRM, correo, hojas de cálculo. Da ejemplos de automatizaciones simples que puedes imaginarte. Explica qué es una **API** en palabras simples (es más simple de lo que suena). Te dice cuándo puedes hacerlo tú y cuándo llamar a un técnico. Y te advierte sobre las trampas: dependencias que te bloquean, y el mantenimiento que cada conexión necesita.

La promesa: la IA conectada ahorra tiempo real cada día. La cautela: una mala conexión puede romper cosas o atraparte. Hazlo con un mapa y un plan.

## Un poco de historia

**Años 1960–1970: programas que se hablan entre sí.** El software de negocio temprano tenía que intercambiar datos —un sistema de inventario alimentando un sistema de contabilidad. Los ingenieros construyeron los primeros enlaces entre programas, a menudo a mano, compartiendo archivos en formatos acordados. La integración nació de pura necesidad.

**Años 1990: la integración empresarial se vuelve una profesión.** Cuando las empresas ejecutaban muchos sistemas a la vez, conectarlos se convirtió en todo un campo. Herramientas de nombres largos —middleware, integración de aplicaciones empresariales— intentaron ser el centro que enlazaba todo. Era potente, caro, y normalmente necesitaba especialistas.

**Años 2000: la economía de las API.** El software empezó a exponer puertas limpias y documentadas para que otro software las usara. Esas puertas se llaman API. De pronto una pequeña empresa podía conectarse a grandes servicios —mapas, pagos, mensajería— sin construirlos. Apareció toda una economía de software conectado.

**Años 2010: el no-code y el integrador ciudadano.** Herramientas como Zapier y Make dejaron que no programadores conectaran apps populares señalando y haciendo clic. Podías decir "cuando un nuevo contacto caiga en mi formulario, añádelo a mi CRM y avísame por correo" sin escribir código. El "integrador ciudadano" —una persona de negocio que construye sus propias conexiones— se volvió real.

**Años 2020: la IA como el nuevo conector.** Las herramientas de IA ganaron la capacidad de leer, escribir y actuar a través de sistemas mediante sus propias API. Ahora la IA puede ser quien hace la conexión: leer tu bandeja, actualizar tus registros, redactar tus respuestas. La fontanería se volvió más lista, y la necesidad de entenderla creció igual de rápido.

El arco: de enlaces de archivo hechos a mano a un mundo donde el software espera estar conectado. La conexión ya no es un lujo; es donde vive el valor.

## Curiosidad

### La nota que conectó al mundo

En 2002, el director ejecutivo de Amazon, Jeff Bezos, envió una ahora famosa nota interna a sus equipos de ingeniería. Los detalles están ampliamente recogidos en la historia de la tecnología. La orden central era tajante: de ahora en adelante, cada equipo debía compartir sus datos y funciones a través de una interfaz limpia y documentada —una API— y nada más. Sin acceso directo a la base de datos de otro equipo. Sin atajos por la puerta de atrás. Si un equipo quería algo de otro equipo, tenía que pedirlo a través de la interfaz publicada, o construirlo él mismo.

La razón no era el orden. Era hacer a Amazon rápido y flexible. Cuando cada parte de la empresa podía alcanzarse por una puerta limpia, los equipos podían cambiar sus propios sistemas sin romper a los demás, y nuevos servicios podían construirse rápido sobre los viejos.

Esa disciplina se reconoce ampliamente como una base de lo que se convirtió en **Amazon Web Services (AWS)** —la plataforma en la nube que ahora impulsa una enorme parte de internet. Una regla sobre cómo el software habla con el software dentro de una empresa se convirtió en uno de los mayores negocios de tecnología de la Tierra.

La lección para una pequeña empresa es la misma en miniatura: **las conexiones limpias y documentadas te hacen flexible; los atajos desordenados te hacen frágil.** Cuando conectes la IA a tus sistemas, construye enlaces limpios, no parches por la puerta de atrás. La tubería ordenada de hoy es la libertad por la que te agradecerás mañana.

## Un ejemplo real de negocio

*Lo siguiente es una composición ilustrativa de patrones comunes del mundo real, no una empresa con nombre.*

Una pequeña firma de administración de propiedades funcionaba con tres sistemas que no se hablaban: un CRM con los contactos de inquilinos, una bandeja compartida para solicitudes de mantenimiento, y una hoja de cálculo que rastreaba los trabajos de reparación. Cada solicitud significaba copiar detalles a mano desde la bandeja a la hoja de cálculo, y luego al CRM. El personal pasaba horas al día en copiar-y-pegar, y detalles se colaban entre las grietas.

Conectaron los tres con una automatización simple. Cuando llegaba un correo de mantenimiento, una IA lo leía, extraía el nombre del inquilino, la propiedad y el problema, y creaba una fila en la hoja de cálculo automáticamente. También redactaba una respuesta al inquilino confirmando la solicitud. Un humano revisaba el borrador y pulsaba enviar. La nota del CRM la añadía la misma automatización.

El resultado no fue magia —fue fontanería. Las horas de copiar-y-pegar en gran parte desaparecieron. Se perdieron menos solicitudes, porque la misma automatización marcaba para un humano todo lo que no podía leer con claridad. La empresa no reemplazó al personal; eliminó la parte aburrida de su día para poder gestionar más propiedades sin más gente.

La lección: la victoria vino de conectar sistemas que ya existían, no de comprar algo nuevo y espectacular.

## Cómo hacerlo

### 19.1 Software de gestión, CRM, correo, hojas de cálculo

Estos son los cuatro sistemas que la mayoría de las empresas ya ejecutan, y los cuatro a los que la IA se conecta más a menudo.

- **Software de gestión (ERP).** Un sistema que dirige el núcleo de tu negocio —inventario, pedidos, producción, finanzas. ERP significa Planificación de Recursos Empresariales. La IA puede leer informes de él, marcar números inusuales, o redactar resúmenes.
- **CRM.** Significa **Gestión de Relaciones con Clientes** —el sistema que guarda tus clientes, contactos, y cada interacción con ellos. La IA puede redactar respuestas a contactos, registrar llamadas, y sacar el historial de un cliente para ayudarte a responder más rápido.
- **Correo.** La bandeja de entrada es donde vive la mayor parte del trabajo de una pequeña empresa. La IA puede clasificar, resumir y redactar respuestas aquí. Esta es a menudo la conexión de mayor valor.
- **Hojas de cálculo.** La herramienta universal. La IA puede llenarlas, leerlas y actualizarlas desde otras fuentes.

Empieza donde el dolor es mayor. Para la mayoría de las pequeñas empresas, eso es el correo y el CRM. Conectar la IA a esos dos da el mayor alivio diario. No intentes conectarlo todo a la vez —elige el que más duele y empieza ahí.

### 19.2 Ejemplos de automatizaciones simples

Los ejemplos concretos te ayudan a imaginar lo posible. Cada uno de estos es una conexión pequeña y común:

- **De bandeja a CRM.** Un nuevo correo de consulta crea automáticamente un contacto en tu CRM, con los datos del remitente rellenados.
- **De formulario a hoja de cálculo.** Un cliente rellena un formulario web; las respuestas caen en una fila de la hoja de cálculo automáticamente, y la IA etiqueta la solicitud por tipo.
- **De correo a borrador de respuesta.** La IA lee una solicitud estándar y escribe un borrador de respuesta en tu bandeja; tú revisas y envías.
- **De documento a registro.** La IA lee un PDF de factura y escribe el importe, la fecha y el proveedor en tu sistema contable.
- **De reunión a notas.** La IA convierte una reunión grabada en un resumen y elementos de acción, y los archiva donde tu equipo pueda verlos.
- **De ticket a alerta.** La IA lee los mensajes de soporte entrantes y marca los enfadados o urgentes para un humano primero.

Fíjate en el patrón: la IA lee de un sitio, hace algo útil, y escribe en otro, con una revisión humana donde importa. Esa es la forma de casi toda buena automatización.

### 19.3 Cuándo necesitas un técnico

Puedes hacer una cantidad sorprendente tú mismo con herramientas sin código. Pero algunos trabajos necesitan un profesional. Sabes cuál es cuál.

**Probablemente puedes hacerlo tú** cuando: las apps son populares (así que existen conectores sin código), los datos son simples, la automatización es pequeña, y un error es barato. Las herramientas de señalar-y-hacer-clic cubren mucho aquí.

**Llama a un técnico cuando:**

- **La conexión toca dinero, registros legales o datos sensibles.** Un error aquí es caro o peligroso.
- **Los sistemas son viejos o hechos a medida** y no tienen un conector listo para usar.
- **Necesitas un enlace fiable y siempre activo** que no deba fallar.
- **La seguridad está involucrada** —conectarse a datos de clientes significa acertar con el control de acceso (mira el [Capítulo 20](ch20-implementing-ai-securely.md)).
- **No entiendes lo que estás conectando.** Nunca conectes lo que no puedas explicar.

Un técnico no es una admisión de fracaso. Es la decisión correcta para las partes arriesgadas o complejas, igual que llamas a un fontanero para la tubería principal y arreglas el grifo tú mismo.

### 19.4 APIs e integraciones explicadas de forma simple

Una **API** suena técnica, pero la idea es simple. Una API es un **menú que un software ofrece a otro.** Es una lista de cosas que se te permite pedirle que haga, y cómo pedirlas.

Piensa en la cocina de un restaurante. No entras y empiezas a cocinar. Miras el menú, pides de lo que se ofrece, y la cocina lo trae. El menú es la API. Te dice qué puedes solicitar ("los datos de este cliente", "añade una fila nueva", "envía este correo") y cómo solicitarlo. No puedes pedir algo fuera del menú, y nunca tocas la cocina directamente.

Por qué importa esto para la IA: cuando un sistema tiene una API, una IA puede usar ese menú para leer y escribir datos de forma segura y predecible. Cuando un sistema no tiene API, conectarse a él es difícil o imposible. Así que cuando eliges software, una buena pregunta es: **¿tiene una API?** Si sí, la IA probablemente puede conectarse. Si no, puede que quedes atrapado.

Una **integración** es la conexión que construyes usando una o más API —el acto de cablear el menú de un sistema a las necesidades de otro. La API es la puerta; la integración es el pasillo que construyes a través de ella.

Dos términos simples que oirás:

- **Acceso de lectura** —la IA puede mirar datos pero no cambiarlos. Más seguro.
- **Acceso de escritura** —la IA puede cambiar datos. Más potente, más arriesgado. Da acceso de escritura solo donde lo necesitas.

### 19.5 Evitar dependencias y bloqueos

Cada conexión crea una **dependencia** —una cosa ahora depende de otra. Las dependencias son normales, pero demasiadas, o las equivocadas, pueden bloquearte.

Vigila estas trampas:

- **Un punto único de fallo.** Si una conexión se rompe y todo tu flujo de trabajo se detiene, eso es un punto único frágil. Ten un respaldo: una forma de hacerlo a mano si el enlace muere.
- **Una cadena de dependencias.** Si A necesita B necesita C necesita D, un eslabón roto detiene todo. Mantén las cadenas cortas.
- **Una dependencia de una herramienta que puede desaparecer.** Si te conectas a un servicio pequeño que cierra, tu automatización muere. Prefiere herramientas estables y establecidas.
- **Bloqueo (lock-in) a través de la integración.** Si todos tus sistemas están cableados de una forma que solo un proveedor entiende, irse se vuelve difícil. Mantén las conexiones limpias y documentadas para poder recablear después. (El bloqueo se trata en el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).)
- **Conexiones sin documentar.** Un enlace que nadie sabe cómo funciona es una bomba de relojería. Documenta cada conexión.

La regla: **construye conexiones limpias, cortas y documentadas con un respaldo manual.** La lección de la nota de Amazon otra vez —puertas limpias, sin parches por la puerta de atrás.

### 19.6 Mantenimiento y actualizaciones

Una conexión no es "ajustar y olvidar". Es algo vivo que necesita cuidados.

- **Los sistemas cambian.** Tu CRM se actualiza, tu proveedor de correo cambia un formato, una API tiene una nueva versión. Cuando un lado cambia, la conexión puede romperse.
- **Fallos silenciosos.** Una conexión puede dejar de funcionar en silencio, y los datos dejan de fluir sin que nadie se dé cuenta. Comprueba que los datos realmente llegan.
- **Aparecen nuevos casos.** La automatización manejaba los casos comunes; llega un nuevo tipo de solicitud y no sabe qué hacer. Revisa qué le falta.
- **Actualizaciones de seguridad.** Las conexiones a datos necesitan que su acceso se revise con el tiempo, sobre todo cuando el personal entra o sale.

Planifica el mantenimiento: asigna a alguien para vigilar las conexiones, revisarlas con regularidad y arreglar las roturas rápido. Construye una alerta simple —si no fluyen datos durante un día, alguien debe saberlo. Un poco de cuidado evita que la fontanería se desborde.

## Ética y responsabilidad

Conectar la IA a tus sistemas significa conectarla a datos de personas reales. Eso conlleva responsabilidad.

**Conecta con consentimiento y cuidado.** Si la IA leerá correos o registros de clientes, sabe qué estás conectando y si está permitido. Respeta las reglas de privacidad (mira el [Capítulo 10](ch10-privacy-and-gdpr.md)).

**Mínimo acceso.** Dale a la IA solo el acceso que necesita. Si solo necesita leer, no le des escritura. Si solo necesita una carpeta, no le des toda la unidad. Esto limita el daño si algo sale mal.

**Mantén un humano en el envío.** Para cualquier cosa que llegue a un cliente, un humano debe revisar antes de que salga. Una automatización que actúa sola sobre mensajes que ven los clientes puede causar daño real.

**Documenta para dar cuentas.** Cuando algo sale mal, necesitas saber qué hizo la automatización y por qué. Una conexión documentada es una conexión responsable.

**No conectes lo que no puedas explicar.** Si no puedes decir en palabras simples qué hace una conexión a los datos de quién, no deberías construirla. La complejidad que no entiendes es un riesgo que no puedes controlar.

Construye conexiones como querrías que se tratara tu propio dato.

## Errores a evitar

**Conectarlo todo a la vez.** Intentar cablear cada sistema el primer día. Elige el que más duele y empieza ahí.

**Sin mapa.** Conectar sin saber qué tienes y cómo se enlaza. Dibuja el mapa primero.

**Parches por la puerta de atrás.** Atajos rápidos y sin documentar que se rompen después y te atrapan. Construye puertas limpias en su lugar.

**Demasiado acceso.** Dar a la IA acceso de escritura a todo cuando solo necesita leer una cosa. Usa el mínimo acceso.

**Sin respaldo.** Una conexión que, cuando se rompe, detiene todo el flujo de trabajo sin plan manual. Ten siempre un respaldo.

**Ignorar los fallos silenciosos.** Asumir que la conexión funciona porque nadie se quejó. Comprueba que los datos realmente llegan.

**Sin plan de mantenimiento.** Cablearlo y marcharse. Las conexiones necesitan cuidados.

**Conectarse a una herramienta que puede desaparecer.** Construir sobre un servicio inestable que puede desaparecer. Prefiere herramientas estables.

**Dejar que la IA actúe sola sobre mensajes a clientes.** Sin revisión humana sobre lo que llega a un cliente. Mantén un humano en el envío.

**Enlaces sin documentar.** Nadie sabe cómo funciona la conexión. Documenta cada uno.

**Olvidar los cambios de personal.** No actualizar el acceso cuando la gente entra o sale. Revisa el acceso con regularidad.

## Ejercicio práctico

### 19.7 Ejercicio: un mapa de los sistemas de tu empresa

No puedes conectar lo que no puedes ver. Dibuja un mapa de los sistemas en los que funciona tu negocio.

**Paso 1 — Enumera cada sistema.** Anota cada pieza de software que tu negocio usa a diario: CRM, correo, contabilidad, hojas de cálculo, inventario, planificación, formularios web, herramientas de chat. No dejes nada fuera.

**Paso 2 — Para cada uno, anota cuatro cosas:**

- **Qué guarda** (qué dato vive ahí).
- **Quién lo usa** (qué personas o roles).
- **¿Tiene una API?** (Revisa el sitio del proveedor o pregunta; marca sí / no / desconocido.)
- **¿Qué tan sensible es el dato?** (Bajo / medio / alto.)

**Paso 3 — Dibuja los enlaces actuales.** En papel, traza líneas entre sistemas que ya pasan datos hoy, incluso si un humano los lleva por copiar-y-pegar. Marca qué enlaces son manuales.

**Paso 4 — Detecta el dolor.** Encierra los enlaces manuales que más tiempo consumen o más errores causan. Estos son tus mejores candidatos a automatizar.

**Paso 5 — Marca el riesgo.** Para cada candidato, anota la sensibilidad. Los enlaces de alta sensibilidad necesitan un técnico y una revisión humana; los de baja sensibilidad puedes probarlos tú.

**Paso 6 — Elige uno.** Elige el único enlace de mayor dolor y menor riesgo como tu primera integración. Haz una prueba piloto (mira el [Capítulo 18](ch18-your-first-pilot-project.md)).

Mantén el mapa en una página. Actualízalo cuando los sistemas cambien. El mapa es tu plan y tu defensa contra conectar a ciegas.

## Lista de verificación

### 19.8 Lista de verificación de integración

Antes de conectar la IA a un sistema, y después, revisa cada casilla.

- [ ] **Tengo un mapa de todos mis sistemas y qué dato guarda cada uno.**
- [ ] **Sé qué sistemas tienen una API y cuáles no.**
- [ ] **Sé qué tan sensible es el dato en cada sistema.**
- [ ] **Elegí el enlace de mayor dolor y menor riesgo para conectar primero.**
- [ ] **Usé una conexión limpia y documentada, no un parche por la puerta de atrás.**
- [ ] **Di a la IA solo el acceso que necesita (mínimo acceso).**
- [ ] **Sé la diferencia entre acceso de lectura y de escritura y usé escritura solo donde hacía falta.**
- [ ] **Un humano revisa cualquier cosa que llegue a un cliente.**
- [ ] **Tengo un respaldo manual si la conexión se rompe.**
- [ ] **Comprobé que la conexión es estable y no un punto único de fallo.**
- [ ] **Construí una forma de detectar fallos silenciosos (alerta si no fluyen datos).**
- [ ] **Documenté cómo funciona la conexión y quién la mantiene.**
- [ ] **Asigné a alguien para mantener y vigilar la conexión.**
- [ ] **Revisé el acceso del personal actual y lo revisaré cuando el personal cambie.**
- [ ] **Ejecuté la conexión como una prueba piloto antes de confiar plenamente en ella.**

Si una casilla está vacía, la conexión no está lista. Rellénala primero. Una IA conectada es un ayudante poderoso; una conectada a ciegas es una carga.

## Puntos clave

- El valor de la IA viene de conectarse a los sistemas que ya ejecutas —la conexión es la fontanería, y el valor fluye a través de ella.
- Una API es simplemente un menú que un software ofrece a otro; si un sistema tiene una API, la IA probablemente puede conectarse, así que pregunta "¿tiene una API?" al elegir software.
- Usa el mínimo acceso —dale a la IA solo lo que necesita, prefiere lectura sobre escritura, y mantén un humano en cualquier cosa que llegue a un cliente.
- Construye conexiones limpias, cortas y documentadas con un respaldo manual; los parches por la puerta de atrás y los fallos silenciosos son las trampas que te rompen.
- Las conexiones son cosas vivas que necesitan mantenimiento, monitorización y revisiones de acceso —monta las y nunca te vayas.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Comprueba un proveedor antes de comprometerte

![Un resumen de diligencia debida de un proveedor](../../assets/examples/due-diligence.png)
*Un resumen de diligencia debida de un proveedor*

**Lo que pides:** `Investiga este proveedor y dime su reputación, cuánto tiempo lleva en el mercado, y cualquier señal de alarma.`

El agente reúne lo que está disponible públicamente y te da una imagen equilibrada con fuentes, para que decidas con los ojos abiertos.

*Consejo: Pídele que enumere lo que no pudo encontrar, para que sepas dónde indagar más.*

---

### Comprueba un pedido en tu sistema

![Un estado de pedido sacado del sistema de negocio](../../assets/examples/order-status.png)
*Un estado de pedido sacado del sistema de negocio*

**Lo que pides:** `¿Cuál es el estado del pedido 4821?`

El agente busca el pedido en tu sistema conectado y te dice su estado en palabras simples —sin cazar menús.

*Consejo: Esto funciona una vez que tu sistema de negocio está conectado. Mira el capítulo de conexión del libro.*

---

### El mismo asistente en tu navegador

![El chat web de AgentBridge en una ventana del navegador](../../assets/examples/web-chat.png)
*El chat web de AgentBridge en una ventana del navegador*

**Lo que pides:** `(browser) Redacta una nota de agradecimiento a nuestros clientes habituales.`

Abre la dirección web y chatea en el navegador. Mismas herramientas, mismos documentos, misma memoria —solo una ventana distinta.

*Consejo: Útil cuando estás en otra máquina pero aún quieres tu propio asistente.*

---

### Enchúfalo a tus propias herramientas

![La API HTTP permite a otros programas usar el asistente](../../assets/examples/http-api.png)
*La API HTTP permite a otros programas usar el asistente*

**Lo que pides:** `POST /v1/chat/completions  { "model": "default-agent", "messages": [...] }`

Tus propios programas pueden llamar al asistente a través de una API web estándar, igual que llamarían a cualquier servicio en línea. Una integración, muchos usos.

*Consejo: Esto es para el paso técnico —el capítulo de conexión del libro lo recorre.*

---

### Conecta otras herramientas de IA a él

![AgentBridge conectado a otras herramientas de IA vía MCP](../../assets/examples/mcp-connector.png)
*AgentBridge conectado a otras herramientas de IA vía MCP*

**Lo que pides:** `(MCP) Conecta AgentBridge como un servidor de herramientas.`

Otras aplicaciones de IA pueden usar las herramientas de AgentBridge mediante el estándar MCP, así que todo tu kit de herramientas funciona junto.

*Consejo: MCP es para conectar herramientas; para el uso diario el chat es todo lo que necesitas.*

<!-- END agentbridge-examples -->
