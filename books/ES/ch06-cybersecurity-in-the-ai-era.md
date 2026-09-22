# Capítulo 6 — Ciberseguridad en la era de la IA

## En palabras simples

Durante casi toda la historia de la informática empresarial, la seguridad significó una sola cosa: mantener a los extraños fuera de tu edificio. Tenías una puerta con llave, una contraseña, un cortafuegos. El malo estaba fuera. Tus datos estaban dentro.

La inteligencia artificial ha difuminado esa línea. Hoy, cuando un empleado escribe una lista de clientes, un contrato o una nómina en una herramienta de IA en línea, ese texto sale del edificio. Viaja a ordenadores que pertenecen a otro. Puede que se almacene allí. Puede que lo lea personal de soporte. Puede que se guarde durante meses. En algunos casos puede que se use para mejorar el producto de esa empresa. La mayoría de la gente nunca piensa en esto, porque la herramienta parece una caja de búsqueda. No es una caja de búsqueda. Es un servicio, gestionado por una empresa, en máquinas que tú no controlas.

La IA cambia el panorama de seguridad en dos direcciones a la vez.

**Los atacantes mejoraron.** Un modelo de lenguaje le da a un criminal tres cosas que antes eran caras: velocidad, escala y acabado. Un correo de phishing que antes parecía una mala traducción ahora puede escribirse en un alemán o japonés de negocios fluido en segundos, personalizado con detalles de un perfil público. Se puede copiar una voz a partir de unos segundos de una grabación, y así es como empleados de finanzas en casos de fraude reportados aprobaron transferencias porque quien llamaba sonaba como su propio jefe. Nada de esto requiere un genio. Requiere una suscripción.

**Tu superficie de ataque se hizo más grande.** «Superficie de ataque» es solo un término para el número de sitios por donde alguien puede entrar. Cada función de IA que añades es una puerta nueva: herramientas de chat, complementos que alcanzan tu correo, agentes que leen carpetas y envían mensajes, modelos entrenados con tus registros, proveedores que guardan una copia de cada prompt y cada respuesta. Hace dos años tu empresa tenía una puerta principal. Ahora puede tener cuarenta, y la mayoría las abrieron tus propios empleados sin avisar a nadie.

Una idea más organiza todo lo demás. La seguridad protege tres cosas, conocidas por tres palabras cortas.

- **Confidencialidad.** Solo las personas adecuadas ven los datos.
- **Integridad.** Los datos no han sido cambiados en secreto.
- **Disponibilidad.** El sistema funciona cuando lo necesitas.

La mayoría de los dueños tratan la seguridad de la IA como solo un problema de confidencialidad. No lo es. Un competidor que envenena tu modelo es un problema de integridad. Un proveedor cuyos sistemas se caen y detienen tus pagos durante semanas es un problema de disponibilidad, y ese causó el mayor daño en la historia más adelante en este capítulo. Cuando mires cualquier herramienta de IA, haz las tres preguntas.

Una advertencia más. El pensamiento «somos demasiado pequeños para que nos ataquen» no es cierto. Los ataques modernos son automatizados: un software escanea todo internet buscando puertas sin llave, como un ladrón prueba todos los coches de un aparcamiento. No te eligen porque seas interesante. Te golpean porque fuiste fácil, y porque guardas datos de clientes, datos bancarios y registros fiscales con muy poca protección alrededor.

La buena noticia es que la mayor parte de la protección que necesitas no es alta tecnología. Es una lista corta de hábitos aburridos, un mapa de a dónde van tus datos, y unos pocos controles en el lugar correcto.

El lado legal de los datos personales está en el [Capítulo 10](ch10-privacy-and-gdpr.md). El uso de herramientas de IA por parte del personal sin aprobación —la «IA en la sombra»— está en el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md). La construcción paso a paso está en el [Capítulo 20](ch20-implementing-ai-securely.md).

## Un poco de historia

La historia de la seguridad repite una lección: el perímetro se mueve, y los defensores tardan en darse cuenta.

En **1988** el gusano Morris dejó fuera de servicio algo así como el diez por ciento de los ordenadores conectados de la incipiente internet. Lo escribió un estudiante de posgrado, no un criminal, y demostró que un programa que se autopropaga podía cruzar el planeta en horas. Durante **los años 1990 y 2000** la respuesta estándar fue el modelo de perímetro: un cortafuegos en el borde, antivirus en cada PC, datos en un servidor en un armario. Funcionó mientras los datos se quedaron donde los pusiste.

En **2013** se violó el minorista estadounidense Target. Los atacantes no entraron en Target. Entraron en una pequeña empresa que suministraba equipos de calefacción y refrigeración para sus tiendas, tomaron las credenciales de acceso de esa empresa, y las usaron para llegar a los sistemas de pago de Target. Se robaron alrededor de 40 millones de números de tarjeta. La lección fue sobre conexión, no sobre código: tu riesgo ahora incluye a todos a los que te enchufas.

En **2016** Microsoft puso un chatbot llamado Tay en redes sociales. En un día, los usuarios le enseñaron a publicar material ofensivo alimentándolo con mensajes repetidos, y lo retiraron. Nadie rompió el programa. Rompieron lo que el modelo estaba leyendo. Esa es la semilla de la inyección de prompts, aunque aún no tenía nombre.

En **2017** el malware NotPetya se propagó desde un software de contabilidad ucraniano y causó daños medidos en decenas de miles de millones de dólares en todo el mundo, golpeando al gigante naviero Maersk, al fabricante farmacéutico Merck y a muchos otros. Un eslabón envenenado en una cadena de suministro de software se convirtió de golpe en problema de todos.

En **2020** el trabajo remoto eliminó el perímetro físico casi de la noche a la mañana. En **2022** ChatGPT convirtió la IA generativa en una herramienta de oficina normal en cuestión de semanas, y el personal empezó a pegar trabajo real en herramientas sin un contrato de empresa detrás. En **septiembre de 2022** el investigador de seguridad Simon Willison publicó una entrada titulada «Prompt injection attacks against GPT-3» y dio nombre a un problema que la gente había estado viendo pero no podía describir: instrucciones ocultas dentro de un texto que un modelo lee, que anulan las instrucciones que tú le diste.

En **2023** los modelos de pesos abiertos significaron que una empresa podía ejecutar IA en su propio hardware, como explica el [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md). Ese mismo año, los proveedores empezaron a enviar «agentes» que pueden actuar en lugar de solo responder, lo que elevó el coste de cada error. En **2024** el riesgo de los proveedores se volvió imposible de ignorar, como se cuenta en la sección Curiosidad más abajo. A partir de **2025**, llegaron agentes con herramientas y credenciales adjuntas, así que el radio de explosión de un permiso equivocado es ahora todo lo que ese agente pueda alcanzar.

Lee la cronología como un largo argumento. Cada paso movió la confianza de una puerta con llave a una relación: un contratista, un proveedor, un complemento, un modelo, un agente. La seguridad dejó de ser un muro y se convirtió en una pregunta sobre quién, y qué, has conectado.

## Curiosidad

### 6.8 El proveedor que casi detiene un sistema sanitario

El 12 de febrero de 2024, unos atacantes entraron en Change Healthcare, una empresa que procesa facturas médicas y pagos en Estados Unidos. Según el testimonio que el director ejecutivo de UnitedHealth Group dio al Congreso de EE. UU. en mayo de 2024, entraron por un portal de acceso remoto que no exigía autenticación de múltiples factores —la segunda comprobación en un inicio de sesión que impide que la mayoría de las contraseñas robadas funcionen—. No había ningún malware ingenioso en la puerta principal. Hubo una contraseña robada y una segunda cerradura que faltaba. Los atacantes pasaron nueve días dentro, moviéndose en silencio y copiando unos seis terabytes de datos. El 21 de febrero activaron un ransomware y bloquearon los sistemas.

Change Healthcare es una filial de UnitedHealth Group, y está en el medio de la cadena de pagos sanitarios estadounidense. Cuando se detuvo, una parte muy grande de las reclamaciones médicas, los pagos de farmacias y las autorizaciones de seguros se detuvo con ella. Las clínicas pequeñas no podían cobrar y se quedaron sin efectivo en semanas; los gremios del sector informaron de pérdidas de los proveedores que llegaban a decenas de millones de dólares al día en toda la red afectada. Nombres grandes que no tenían nada que ver con la brecha —cadenas de farmacias, aseguradoras regionales, un hospital naval— encontraron sus propias operaciones bloqueadas, porque todos hacían pasar datos por el mismo intermediario.

UnitedHealth luego adelantó más de 2.000 millones de dólares en préstamos de emergencia a los proveedores afectados a mediados de marzo, y más de 6.000 millones a mediados de abril. Informes de Reuters y Wired dijeron que se pagó un rescate de unos 22 millones de dólares en bitcoin a una billetera vinculada al grupo criminal ALPHV, también conocido como BlackCat, que UnitedHealth confirmó el 29 de febrero como el atacante. En octubre de 2024 UnitedHealth estimó que unos 190 millones de personas vieron afectados sus datos, una de las mayores brechas jamás registradas.

¿Por qué le importa esto a una pequeña empresa que nunca tocará una reclamación médica? Por quién fue la víctima real. Los hospitales y farmacias que sufrieron no fueron hackeados. Muchos de ellos tenían buena seguridad. Resultaron dañados porque una empresa en el medio de su flujo de trabajo fue hackeada, y no podían sobrevivir sin esa empresa. Su seguridad solo era tan buena como el proveedor menos protegido de su cadena.

Ahora añade el ángulo del análisis, porque está más cerca de casa de lo que parece. En 2024, OpenAI reveló un incidente que no fue en absoluto una brecha de sus propios sistemas. El problema estaba en Mixpanel, un servicio de análisis de terceros usado en el sitio de desarrolladores de su interfaz de programación de aplicaciones. Los servicios de análisis son pequeños trozos de software que una empresa pone en su sitio web para contar visitas y ver cómo hace clic la gente. Ese proveedor fue violado, y se expusieron nombres, direcciones de correo y detalles de dispositivos de algunos titulares de cuentas. El contenido de los chats, las contraseñas y las claves secretas no.

El daño allí fue limitado. La lección no. Cuando compras un servicio de IA, también compras todas las empresas en las que ese servicio se apoya: su análisis, su alojamiento, sus herramientas de soporte, sus complementos. Heredas una cadena de suministro que nunca elegiste y de la que quizá nunca oíste hablar.

## Un ejemplo empresarial real

### El ingeniero que le pidió ayuda al chatbot

En abril de 2023 Bloomberg informó de que Samsung había prohibido las herramientas de IA generativa como ChatGPT en los equipos de la empresa. La razón no era una teoría sobre el riesgo. Ingenieros habían pegado código fuente confidencial en un chatbot público mientras buscaban una corrección de un error, en más de una ocasión, en una división que trabajaba en semiconductores —uno de los tipos de código más celosamente guardados del mundo—. Una nota interna revisada por Bloomberg señaló supuestamente que una encuesta interna encontró que el 65 por ciento de los encuestados ya creía que la herramienta era un riesgo de seguridad.

Mira esto desde el lado del ingeniero. No se robó nada. Nadie entró. Una persona estaba atascada en un problema, encontró una herramienta que lo resolvía en diez segundos, y la usó. La herramienta era excelente. El criterio fue malo. El código no era suyo para regalarlo.

Este es el fallo de seguridad de IA más común que existe, y no es exótico. Ocurre en bufetes de abogados cuando alguien pega el contrato de un cliente para resumirlo. En despachos de contabilidad con una declaración de impuestos. En agencias con una campaña no publicada de un cliente. En recursos humanos con una pila de currículums. El patrón es siempre el mismo: una herramienta útil, una persona con prisa, y un copiar-y-pegar que cruza una frontera que nadie trazó.

De ello se siguen dos cosas. Primera, la solución no es solo una prohibición, porque una prohibición sin alternativa no detiene el comportamiento; lo esconde, lo cual es peor, ya que ahora no puedes ver los datos fluyendo. Segunda, la solución no es solo formación, porque una persona con prisa a las cinco de la tarde no recordará una política de cuarenta páginas. La solución es hacer que el camino seguro sea el camino fácil: una herramienta aprobada que sea más rápida que la insegura, más un control que atrape los peores datos antes de que salgan. Ambos están en la siguiente sección.

## Cómo hacerlo

### 6.7 Cómo protegerte: cortafuegos de IA, filtros, monitorización

Haz esto en orden. Cada paso depende del anterior.

**Paso 1: Dibuja el mapa antes de comprar nada.**
Toma una hoja de papel. Enumera cada herramienta de IA que toque tu empresa, incluidas las gratuitas en los teléfonos del personal. Para cada una: qué datos entran, qué sale, dónde se almacena, quién es el proveedor, y si tienes un contrato firmado. Encontrarás herramientas que no conocías. Este es el documento de seguridad más valioso que producirás este año.

**Paso 2: Pon una puerta entre tu gente y los servicios de IA.**
Una «pasarela de IA» o «cortafuegos de IA» es un único punto por el que pasa todo el tráfico de IA, para que puedas verlo y controlarlo. Los productos convencionales hacen esto: servicios de seguridad de contenido y de blindaje de prompts de las grandes plataformas en la nube, barreras integradas en los servicios de modelos en la nube, pasarelas conscientes de la IA, y herramientas de prevención de pérdida de datos que inspeccionan lo que envían los empleados. Necesitas saber que la categoría existe y qué compra: un lugar para permitir o bloquear herramientas, inspeccionar contenido y guardar registros.

**Paso 3: Filtra lo que sale.**
El control de mayor valor de esta lista. Configura tu pasarela o herramienta de pérdida de datos para bloquear o avisar sobre las categorías que nunca deben salir: números de identificación nacional y fiscales, números bancarios y de tarjeta, información de salud, archivos de nómina, contratos firmados, código fuente y documentos confidenciales de clientes. Una ventana emergente que diga «esto parece datos personales, ¿estás seguro?» detiene por sí sola una gran parte de los accidentes, porque la mayoría son accidentes.

**Paso 4: Filtra lo que entra.**
Esta es la defensa contra la inyección de prompts, y tiene una regla de oro: **nunca dejes que una herramienta de IA actúe sobre instrucciones que encuentra dentro de un documento, un correo, una página web o una hoja de cálculo.** Un modelo que lee tu bandeja de entrada debe resumir, no obedecer. Donde una herramienta deba actuar, exige que un humano confirme antes de que se ejecute. Trata cada documento externo como entrada no confiable, igual que tratas un adjunto de un desconocido.

**Paso 5: Da a los agentes el mínimo poder posible.**
Decide los permisos de un agente en papel antes de conectarlo. Solo lectura donde puedas. Su propia cuenta de servicio, nunca un inicio de sesión de administrador compartido. Una carpeta, no toda la unidad. Un límite de gasto para lo que cueste dinero. Un límite de tiempo. Un dueño humano con nombre. Si no necesita borrar, no dejes que borre. Dale a la herramienta el conjunto más pequeño de llaves que aún le permita hacer el trabajo.

**Paso 6: Registra todo y lee los registros.**
Registra quién usó qué herramienta de IA, cuándo y más o menos para qué —y luego revísalo. Una mirada semanal de quince minutos te muestra herramientas no aprobadas, volumen inusual y patrones que puedes convertir en política. Sin registros no hay investigación: después de un incidente estarás adivinando.

**Paso 7: Mantén un control humano en todo lo irreversible.**
Cualquier acción que no se pueda deshacer —enviar dinero, borrar registros, enviar un correo a una lista de clientes, firmar algo— necesita un paso de aprobación humana. No una notificación. Una aprobación.

**Paso 8: No descuides lo básico aburrido.**
La IA no reemplaza la seguridad ordinaria; se asienta encima de ella. Autenticación de múltiples factores en cada cuenta que pueda alcanzar datos de la empresa, incluidos los portales de proveedores. Un gestor de contraseñas para que nadie reutilice contraseñas. Actualizaciones puntuales. Copias de seguridad probadas y guardadas sin conexión. Protección de endpoints en cada máquina. Si esto es débil, ningún control específico de IA te salvará.

**Paso 9: Forma con una regla, no con un manual.**
Dale al personal una frase que puedan llevar: *si no lo pondrías en un correo a un desconocido, no lo metas en una herramienta de IA.* Luego diles qué hacer en su lugar, y haz que esa alternativa sea fácil. Las reglas sin alternativas se ignoran.

**Paso 10: Planifica que el proveedor esté caído.**
Pregunta a cada proveedor de IA: qué pasa si no está disponible durante una semana. Ten una alternativa manual para cualquier proceso que hayas vuelto dependiente de ellos. La disponibilidad es una propiedad de seguridad, y la historia sanitaria de arriba es la prueba.

## Ética y responsabilidad

La seguridad es un asunto ético antes que técnico. Cuando los clientes te dan su dirección, su detalle de salud o su información de pago, confían en que la guardes de forma segura. Perderla no es un accidente que te pasó a ti; es un daño hecho a ellos. Ese es el mismo deber de cuidado del que se habla en el [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md), aplicado a los sistemas en lugar de a las decisiones.

De ello se siguen tres deberes. **Deber de competencia:** desplegar una herramienta que no entiendes no es neutral. Si no puedes decir a dónde van tus datos, no puedes protegerlos, y «no lo sabíamos» es una defensa débil ante un regulador, un cliente o un tribunal. El deber de alfabetización del Reglamento de IA de la UE, tratado en el [Capítulo 5](ch05-rules-and-legal-responsibility.md), lo deja explícito. **Deber de divulgar:** si sufres una brecha, informa a las personas afectadas de forma rápida y clara. Esconderlo para proteger tu reputación transfiere el coste de tu problema a las personas que confiaron en ti; los plazos legales están en el [Capítulo 10](ch10-privacy-and-gdpr.md). **Proporcionalidad en la monitorización:** registrar el uso de IA protege a la empresa, y también significa leer lo que tu personal teclea. Fija una política escrita que diga qué se registra, por qué, quién puede verlo y durante cuánto tiempo. Monitoriza el flujo de datos, no a la persona. La vigilancia secreta daña la confianza y a menudo incumple la ley local.

Una última regla: no uses herramientas de IA para atacar otros sistemas, y no pruebes tus propias defensas con datos en vivo o cuentas de clientes en vivo. Usa un entorno de pruebas aparte.

## Errores a evitar

1. **Tratar una herramienta de IA como un buscador.** Un buscador indexa páginas públicas. Un servicio de IA recibe tu texto, lo almacena y lo procesa en ordenadores de otro.
2. **Conceder permisos amplios «para que funcione».** La conveniencia de hoy es una brecha mañana. Concede el mínimo y amplía solo con una necesidad probada.
3. **Dejar que una IA lo lea todo.** Apuntar un asistente a una unidad compartida que guarda nóminas, archivos legales y registros de clientes convierte una cuenta comprometida en exposición total.
4. **Sin registros.** Sin registros no puedes averiguar qué pasó, ni probar que tenías el control.
5. **Aceptar «de nivel empresarial» como respuesta.** Pregunta en su lugar: ¿entrenan con mis datos, cuánto tiempo guardan los prompts, quiénes son sus subencargados, dónde se almacenan los datos, me avisarán si sufro una brecha?
6. **Ignorar el plan gratuito de consumo.** El personal en cuentas personales significa que tus datos van a algún sitio sin contrato y sin controles.
7. **Bloquearlo todo.** Una prohibición sin alternativa aprobada no detiene el uso; lo esconde.
8. **Confundir confidencialidad con integridad.** El envenenamiento y la manipulación no son fugas. Protege solo contra los datos que salen y te perderás los datos que se corrompen.
9. **Confiar en un proveedor porque es grande.** La mayor brecha de pagos sanitarios de la historia empezó con un segundo factor de inicio de sesión que faltaba.
10. **Tratar la seguridad como un proyecto de una sola vez.** Las amenazas, las herramientas y el personal cambian. Revisa el mapa cada trimestre.

## Ejercicio práctico

### 6.9 Mapea tus puntos de vulnerabilidad

Reserva noventa minutos con un colega que conozca el trabajo diario. No hagas esto solo.

**Parte A — Enumera los datos (20 minutos).** Escribe cada categoría de información sensible que tu empresa posee. Filas típicas: nombres y contactos de clientes, datos de pago o bancarios, números de identificación nacional o fiscales, registros de empleados y nóminas, currículums y datos de candidatos, información de salud o de seguros, contratos y presupuestos, código fuente o diseños, planes estratégicos y financieros.

**Parte B — Traza cada uno (40 minutos).** Para cada fila responde cinco preguntas por escrito:

1. ¿Dónde vive? (sistema, carpeta, hoja de cálculo, papel)
2. ¿Quién puede alcanzarlo? (roles, personas con nombre, contratistas)
3. ¿Qué herramienta de IA lo toca, si alguna?
4. ¿Sale de nuestro edificio? ¿A dónde va, y bajo qué contrato?
5. ¿Podemos ver que ocurra? (registro, sí o no)

**Parte C — Puntúa y elige (30 minutos).** Marca cada fila:

- **Rojo** — datos sensibles que salen de la empresa sin contrato y sin registro.
- **Ámbar** — datos sensibles que se quedan dentro pero son ampliamente alcanzables, o salen bajo un contrato que no has leído.
- **Verde** — datos de baja sensibilidad, o datos sensibles con contrato, un filtro y registros.

Cada fila roja es una acción para este mes. Elige las cinco principales y escribe un dueño y una fecha límite junto a cada una. Unas cinco iniciales típicas: autenticación de múltiples factores en cuentas de proveedores, una herramienta de IA aprobada para el personal, una regla de pérdida de datos para números de identificación, acceso a unidades compartidas reducido a las carpetas que cada rol necesita, y una regla de uso aceptable de una página. Mantén el mapa en una página, y actualízalo cada trimestre y cada vez que añadas una nueva herramienta de IA.

## Lista de comprobación

### 6.10 Las 10 acciones de seguridad mínimas

- [ ] **Cada cuenta tiene autenticación de múltiples factores**, incluidos portales de proveedores, correo, banca, almacenamiento en la nube e inicios de sesión administrativos.
- [ ] **Existe un mapa escrito** de cada herramienta de IA en uso, qué datos entran en cada una, y dónde se almacenan esos datos.
- [ ] **Existe una herramienta de IA aprobada y es más fácil de usar** que las alternativas no aprobadas.
- [ ] **El filtrado de salida está en marcha** para números de identificación y fiscales, datos de pago, datos de salud, nómina, contratos y código fuente.
- [ ] **Ninguna herramienta de IA actúa sobre instrucciones encontradas dentro de documentos que lee**; las acciones necesitan confirmación humana.
- [ ] **Cada agente de IA funciona con el mínimo privilegio**: su propia cuenta, solo lectura donde sea posible, gasto limitado, sin derechos de administrador.
- [ ] **Existen registros del uso de IA, y alguien los revisa semanalmente.**
- [ ] **Las acciones irreversibles requieren un paso de aprobación humana**, no solo una notificación.
- [ ] **La diligencia debida sobre el proveedor está hecha por escrito**: entrenamiento con tus datos, periodo de retención, subencargados, ubicación de los datos, condiciones de notificación de brechas.
- [ ] **Las copias de seguridad están probadas y guardadas sin conexión, y existe una alternativa manual** para cualquier proceso que dependa de un proveedor de IA.

## Puntos clave

- La IA hace los ataques más baratos y rápidos, y multiplica el número de puertas a tu negocio; ambas cosas cambian a la vez.
- La fuga más común no es un hackeo —es un empleado servicial pegando datos confidenciales en una herramienta que nunca comprobó—.
- Protege las tres propiedades: confidencialidad (datos que salen), integridad (datos envenenados) y disponibilidad (un proveedor caído).
- Las defensas centrales son un mapa de datos, una pasarela controlada, filtrado de salida, mínimo privilegio para los agentes, y registros que alguien lee de verdad.
- Tu riesgo incluye el riesgo de tus proveedores, y también el de los proveedores de ellos; pregunta en quién se apoyan ellos antes de apoyarte tú en ellos.
