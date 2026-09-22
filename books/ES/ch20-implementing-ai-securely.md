# Capítulo 20 — Implementar la IA de forma segura

## En palabras simples

Cuando introduces la IA en tu negocio, estás dejando que un nuevo trabajador maneje tus datos. Como cualquier trabajador, ese nuevo empleado debe ser confiable, vigilado y tener límites. Este capítulo trata de eso: cómo usar la IA sin filtrar los datos de tus clientes, tus finanzas ni tus secretos.

La seguridad no es un producto que se compra. Es un conjunto de hábitos que se construyen. El objetivo es simple: **diseña tus automatizaciones de modo que, incluso cuando algo salga mal, tus datos sigan protegidos.** Esa idea tiene un nombre: **seguridad desde el diseño**, y significa que piensas en la seguridad desde el principio, no como algo posterior después de una brecha.

Una buena analogía es una casa. No dejas la puerta principal abierta de par en par porque "todavía no ha pasado nada malo". Cierras con llave, limitas a qué habitaciones pueden entrar las visitas, pones una luz con temporizador y tienes un plan por si vuelves a casa y encuentras una ventana abierta. La seguridad de la IA es la misma forma de pensar por capas: controla quién entra, protege lo que hay dentro, observa lo que pasa y sabe qué hacer si algo se rompe.

Este capítulo cubre los hábitos esenciales: diseñar automatizaciones seguras, controlar quién puede hacer qué, cifrar los datos para que sean ilegibles para los ladrones, vigilar y registrar lo que hace la IA, planificar el día en que algo salga mal, y capacitar a tu personal, porque el factor humano es la primera línea de defensa.

Una verdad honesta desde el inicio: ningún sistema es perfectamente seguro. El objetivo no es la perfección; es convertir tu negocio en un objetivo difícil y nunca en uno fácil. La mayoría de los ataques van tras el objetivo fácil. Una seguridad buena y simple te mueve de fácil a difícil.

## Un poco de historia

**Años 70 y 80: la seguridad empieza en el perímetro.** La seguridad informática temprana se centraba en mantener fuera a los extraños: cortafuegos, contraseñas, salas de servidores con llave. El modelo era un castillo: murallas fuertes, todo lo de dentro está a salvo. Esto funcionó hasta que la gente necesitó conectarse y compartir, y eso agrietó las murallas.

**Años 90: el perímetro se disuelve.** Internet y el correo electrónico hicieron que los datos empezaran a moverse. El modelo del castillo se rompió. Los virus y las intrusiones entraban por las mismas conexiones que hacían posible el negocio. La seguridad tenía que seguir a los datos, no solo vigilar la puerta.

**Años 2000: "menor privilegio" y defensa en profundidad.** El pensamiento de seguridad se giró hacia adentro. El principio de **menor privilegio** —dar a cada usuario y programa solo el acceso que necesita de verdad, nada más— se volvió central. También la **defensa en profundidad**: muchas capas superpuestas, de modo que si una falla, otra atrapa la amenaza.

**Años 2010: "asume la brecha".** Los expertos se dieron cuenta de que no siempre se puede mantener fuera a los atacantes. La nueva mentalidad era *asumir* que un intruso ya podría estar dentro, y enfocarse en limitar a qué puede llegar y detectarlo rápido. El registro, la monitorización y la respuesta rápida se volvieron tan importantes como las murallas.

**Años 2020: la IA añade una nueva superficie de ataque.** La IA trae nuevas formas de daño: trucos que engañan a la propia IA, envenenamiento de datos y el riesgo de alimentar con información sensible a herramientas que no controlas. (Estas amenazas específicas se tratan en el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).) Los viejos principios —menor privilegio, defensa en profundidad, asume la brecha— siguen aplicándose, ahora aplicados a un nuevo tipo de trabajador.

El recorrido: de un castillo con una sola muralla a muchas capas que asumen que la muralla puede ser violada. La lección nunca cambió: protege los datos en sí, no solo la puerta.

## Curiosidad

### 20.7 La empresa que detectó un ataque en un registro que nadie miraba

*La empresa específica de esta historia es ilustrativa: un compuesto realista, no una firma con nombre propio. El patrón que hay detrás es real y está bien documentado.*

Imagina una empresa mediana que tenía un sistema de registro: un historial de todo lo que pasaba en su red. Los registros funcionaban sin parar, anotando fielmente cada inicio de sesión, cada archivo al que se accedía y cada solicitud inusual. Durante meses, nadie los leyó. Ahí estaban, como una cámara de seguridad que nadie mira.

Entonces un día, un técnico nuevo, mientras ordenaba, echó un vistazo a los registros y vio algo raro: un programa se comunicaba con una dirección externa a horas extrañas, extrayendo datos lenta y constantemente. Llevaba semanas haciéndolo. Nadie se había dado cuenta porque nadie estaba mirando. Cuando por fin miraron, encontraron un intruso que había estado dentro, en silencio, mucho más tiempo del que nadie imaginaba.

La lección incómoda no es que la empresa fuera descuidada. Es que **la evidencia estuvo ahí todo el tiempo, y fue ignorada.** La empresa había invertido en la cámara, pero no en vigilarla.

Este patrón no es ficción. El informe anual de IBM *Cost of a Data Breach* (Coste de una brecha de datos) ha descubierto, año tras año, que las brechas tardan mucho en detectarse: del orden de **doscientos días** en promedio en las ediciones recientes, y que una gran parte son detectadas primero por alguien de fuera de la empresa, no por su propia monitorización. Los registros y las señales a menudo existen. Lo que falta es una persona que los mire.

Para tus automatizaciones con IA, la lección es directa: **un registro que nadie lee no es seguridad.** Si guardas registros de lo que hace tu IA, asigna a alguien que realmente los revise y configura alertas para que las señales importantes encuentren a un humano en vez de esperar a ser descubiertas.

## Un ejemplo real de negocio

*Lo siguiente es un compuesto ilustrativo de patrones comunes del mundo real, no una única empresa con nombre propio.*

Un pequeño minorista en línea quería que la IA redactara correos de atención al cliente. La forma fácil y arriesgada era darle a la IA acceso completo a toda la base de datos de clientes: nombres, direcciones, historial de pagos, y dejarla leer lo que necesitara. El dueño se detuvo y en cambio lo hizo de la forma más segura.

Le dieron a la IA acceso **solo de lectura** a justo los detalles de los pedidos que necesitaba para responder una pregunta de envío: ni registros de pago, ni el expediente completo del cliente. Configuraron que la IA pudiera redactar, pero que un humano pulsara el botón de envío. Activaron un registro que anotaba cada pedido que la IA tocaba. Le dijeron al equipo de soporte qué podía y qué no podía ver la IA, y les pidieron que reportaran cualquier cosa extraña.

A las tres semanas, el registro mostró que la IA había recibido la petición —de un cliente astuto— de revelar la dirección de otro cliente haciéndose pasar por esa persona. La IA se negó, porque simplemente no se le había dado acceso a esos datos. El intento falló sin causar daño, y el registro lo capturó, así que el equipo aprendió que existía ese truco.

Si el dueño hubiera tomado el camino fácil y le hubiera dado a la IA toda la base de datos, ese mismo truco podría haber funcionado. El diseño seguro —menor acceso, un humano en el envío, un registro vigilado— convirtió una posible brecha en nada. Así se ve la seguridad desde el diseño en la práctica.

## Cómo hacerlo

### 20.1 Principios de seguridad desde el diseño: cómo diseñar una automatización que no exponga datos

La seguridad desde el diseño significa incorporar la seguridad en la automatización desde el primer boceto. Haz estas preguntas antes de construir nada:

- **¿Qué datos necesita realmente esta automatización?** Usa los mínimos posibles. Si solo necesita un número de pedido, no le des el expediente completo del cliente.
- **¿Cuál es el peor escenario si se filtra o la engañan?** Imagina el fallo. Diseña para que el peor caso sea pequeño.
- **¿A dónde van los datos?** Conoce cada sistema que los datos tocan, sobre todo los que están fuera de tu control. No alimentes con datos sensibles a una herramienta que no puedes justificar.
- **¿Puede un humano detenerla?** Incorpora un interruptor de emergencia: una forma de apagar la automatización al instante si se comporta mal.
- **¿Falla de forma segura?** Si algo se rompe, la automatización debe detenerse y proteger, no abrirse. Una puerta que se cierra con llave cuando se va la luz es "a prueba de fallos".

El principio central es el **menor privilegio**: acceso mínimo, alcance mínimo, datos mínimos. Una automatización que nunca tuvo acceso a los datos sensibles no puede filtrarlos, por muy astuto que sea el ataque. Elimina el acceso desde el diseño, y el riesgo se va con él.

### 20.2 Control de acceso: quién puede hacer qué

El control de acceso es simplemente decidir quién tiene permiso para hacer qué, y hacerlo cumplir. Es la llave de cada habitación, no solo la de la puerta principal.

Tres reglas simples:

- **Dale a cada persona y a cada herramienta solo el acceso que necesita su trabajo.** Una herramienta de soporte que responde preguntas de envío necesita datos de pedidos, no datos de nóminas. Un empleado junior no debería tener el mismo acceso que el dueño.
- **Separa las funciones.** La persona que configura la IA no debería ser la única que puede aprobar sus acciones, ni la única que puede ver los registros. Reparte las llaves para que ninguna cuenta comprometida pueda hacerlo todo.
- **Revisa el acceso cuando la gente cambia.** Cuando el personal se incorpora, se mueve o se va, actualiza su acceso el mismo día. El acceso antiguo que se queda es una de las formas más comunes en que ocurren las brechas.

Usa las herramientas que tus sistemas ya tienen: roles de usuario, permisos y controles de inicio de sesión. Activa la **autenticación de dos factores** (un segundo paso además de la contraseña, como un código en tu teléfono) siempre que puedas. Detiene la mayoría de los ataques con contraseñas robadas.

### 20.3 Cifrado: proteger los datos en tránsito y en reposo

El **cifrado** significa revolver los datos de modo que solo alguien con la clave correcta pueda leerlos. Para un ladrón, los datos cifrados parecen un sinsentido. Protegen los datos en dos estados:

- **En tránsito**: datos que se mueven entre lugares, como un correo o una subida de archivo. El cifrado aquí significa que un ladrón que intercepta la conexión solo ve basura. Busca "https" y conexiones seguras.
- **En reposo**: datos que están quietos, como archivos en un disco o registros en una base de datos. El cifrado aquí significa que un ladrón que roba el disco duro sigue sin poder leerlos.

Para un pequeño negocio, los pasos prácticos son simples: usa herramientas que cifren por defecto (la mayoría de los servicios de buena reputación lo hacen), comprueba que las conexiones sean seguras (https) y pregúntale directamente a cualquier proveedor: "¿Están mis datos cifrados en tránsito y en reposo?". Un proveedor serio responde que sí y explica cómo. Si no puede, eso es una advertencia.

Una precaución: el cifrado protege los datos de agentes externos. No protege de alguien que tiene la clave y la usa mal. Por eso el control de acceso (20.2) y el cifrado trabajan juntos: el cifrado oculta los datos, el control de acceso limita quién tiene la clave.

### 20.4 Monitorización y registro: saber siempre qué está haciendo la IA

Un **registro** es un historial de lo que pasó: quién hizo qué, cuándo y sobre qué datos. La **monitorización** es vigilar esos registros, en vivo o de forma regular, para detectar problemas.

Por qué importa para la IA: una automatización con IA actúa sobre tus datos todo el día. Sin un registro, no puedes decir qué tocó, qué cambió ni si la engañaron. Con un registro, tienes un historial que puedes revisar y una pista que un atacante no puede ocultar.

Haz que el registro sea útil:

- **Registra las acciones importantes**: qué datos leyó la IA, qué escribió, qué envió y cualquier solicitud que rechazó.
- **Configura alertas** para que las señales importantes encuentren a un humano. No hagas que alguien se quede mirando una pantalla; haz que el sistema grite cuando algo inusual ocurra.
- **Míralos de verdad.** Como muestra la historia de curiosidad, un registro que nadie lee no es seguridad. Asigna a alguien para que revise, aunque sea brevemente, en un horario regular.
- **Mantén los registros a salvo** para que un intruso no pueda borrarlos.

La monitorización convierte un sistema silencioso en uno visible. No puedes proteger lo que no puedes ver.

### 20.5 Planes de respuesta a incidentes: qué hacer si algo sale mal

Algo saldrá mal tarde o temprano. La pregunta no es "si", sino "cuándo", y qué tan preparado estás. Un **plan de respuesta a incidentes** es un plan escrito para el mal día, hecho en un día tranquilo para no improvisar en pánico.

Un plan simple tiene cinco pasos:

1. **Detectar.** ¿Cómo sabrás que algo anda mal? (Una alerta, el reporte de un empleado, la queja de un cliente.)
2. **Contener.** ¿Cómo detienes el daño ahora mismo? (Apaga la automatización, corta la conexión, bloquea la cuenta.)
3. **Evaluar.** ¿Qué se expuso o se dañó? Revisa los registros.
4. **Corregir y recuperarse.** Repara la causa y restablece la operación normal y segura.
5. **Reportar y aprender.** Informa a las personas que necesitan saberlo, y sabe a quién estás obligado legalmente a informar. (Las leyes de privacidad como el RGPD tienen obligaciones de notificación; ver el [Capítulo 10](ch10-privacy-and-gdpr.md).) Luego escribe qué pasó y cómo prevenirlo la próxima vez.

Escribe el plan en una página. Nombra quién hace qué. Ten listos los contactos de emergencia. Haz un simulacro rápido una vez al año para que todos sepan su parte. Un plan ensayado convierte una crisis en un evento manejable.

### 20.6 Capacitación del personal: el factor humano es la primera defensa

La cerradura más fuerte la puede abrir una sola persona descuidada. Tu personal es a la vez tu mayor riesgo y tu mejor defensa. La capacitación los transforma del punto débil en la primera línea.

Qué enseñar, en términos simples:

- **Reconocer los trucos.** Los atacantes engañan a la gente con correos falsos, solicitudes urgentes y llamadas del tipo "hablo de sistemas, dame tu contraseña". Enseña al personal a detectarlos y a dudar de ellos.
- **Tratar los datos con cuidado.** Quién puede ver qué, y por qué. Nunca compartir datos de clientes fuera de los canales aprobados.
- **Reportar, no ocultar.** Haz que sea seguro y esperado reportar un error o una solicitud extraña. Un empleado que reporta un correo sospechoso a tiempo salva a la empresa. Uno que lo oculta deja que un problema pequeño crezca.
- **Conocer los límites de la IA.** El personal debe saber qué puede y qué no puede ver la IA, y nunca pedirle que haga algo fuera de sus límites seguros.
- **Higiene de contraseñas e inicios de sesión.** Contraseñas fuertes, autenticación de dos factores, no compartir inicios de sesión.

Mantén la capacitación breve, regular y práctica, no una charla de una vez al año. Un recordatorio mensual de cinco minutos y un canal de reporte claro hacen más que un largo curso anual que nadie recuerda.

## Ética y responsabilidad

La seguridad es un deber ético, no solo técnico.

**Protege a las personas cuyos datos custodias.** Clientes, empleados y socios te confiaron su información. Una brecha daña a personas reales. Tratar esos datos de forma segura es una cuestión de honestidad y cuidado.

**Reporta con honestidad cuando algo salga mal.** Si debes notificar a clientes o reguladores, hazlo de inmediato y con la verdad. Encubrir una brecha es peor que la brecha misma, tanto ética como legalmente.

**No uses la seguridad como excusa para esconderte.** "Estamos seguros" nunca debería significar "no puedes comprobarlo". La rendición de cuentas y la transparencia van de la mano.

**Equilibra la seguridad con la usabilidad.** Una seguridad tan pesada que nadie puede trabajar se salta por encima, y una seguridad saltada no es seguridad en absoluto. Haz que el camino seguro sea el camino fácil.

**Capacita con respeto, no con culpa.** Cuando alguien comete un error, enseña, no castigues. Una cultura de culpa esconde los errores; una cultura de aprendizaje los saca a la luz a tiempo.

Protege tus datos como querrías que protegieran los tuyos.

## Errores que debes evitar

**Demasiado acceso.** Darle a la IA o al personal más acceso del necesario. Usa el menor privilegio.

**Ningún humano en el envío.** Dejar que la IA actúe sola en mensajes que llegan al cliente. Mantén una revisión humana.

**Alimentar con datos sensibles a herramientas sin verificar.** Pegar datos de clientes en una herramienta que no puedes justificar. Sabes a dónde van los datos.

**Un registro que nadie lee.** Recoger historiales y nunca mirarlos. Asigna a alguien y configura alertas.

**Sin plan de incidentes.** Improvisar en el mal día. Escribe el plan en un día tranquilo.

**Compartir inicios de sesión.** Una cuenta compartida por muchas personas destruye la rendición de cuentas. Dale a cada persona la suya.

**Sin autenticación de dos factores.** Dejar las cuentas expuestas a contraseñas robadas. Activa el 2FA en todas partes.

**Ignorar los cambios de personal.** Acceso antiguo que se queda después de que alguien se va. Actualiza el acceso el día que cambian los roles.

**Culpar en lugar de capacitar.** Castigar los errores para que la gente los esconda. Enseña y fomenta el reporte.

**Asumir que el proveedor es seguro.** Confiar sin preguntar. Pregunta a los proveedores sobre cifrado y acceso.

**La seguridad como ocurrencia tardía.** Construir la automatización primero y pensar en la seguridad después. Diseña la seguridad desde el inicio.

**Sin interruptor de emergencia.** No hay forma de detener la automatización rápido cuando se comporta mal. Construye el botón de apagado.

## Ejercicio práctico

### 20.8 Ejercicio: escribe tu plan de seguridad para la IA

Escribe un plan de seguridad de una página para una automatización con IA que uses o planees usar. Rellena cada línea.

**1. La automatización.** Nómbrala y di qué datos toca.

**2. Menor acceso.** Enumera exactamente qué datos necesita. Elimina todo lo demás. Escribe el acceso que realmente vas a otorgar.

**3. Revisión humana.** ¿Dónde está el humano en el bucle? ¿Qué puede hacer la IA sola y qué necesita la aprobación de una persona?

**4. Ubicación de los datos.** ¿A dónde van los datos? Enumera cada sistema, sobre todo los que están fuera de tu control. Anota los que no puedas justificar y elimínalos.

**5. Cifrado.** ¿Están los datos cifrados en tránsito y en reposo? Compruébalo con cada proveedor y escribe la respuesta.

**6. Control de acceso.** ¿Quién puede hacer qué? Enumera los roles. Anota dónde activarás la autenticación de dos factores.

**7. Registro.** ¿Qué registrarás? ¿Quién lo mirará y con qué frecuencia? ¿Qué disparará una alerta?

**8. Interruptor de emergencia.** ¿Cómo la apagas al instante? Escribe los pasos exactos.

**9. Plan de incidentes.** Escribe los cinco pasos: detectar, contener, evaluar, corregir, reportar, con nombres de quién hace cada uno. Anota cualquier obligación legal de notificación (ver el [Capítulo 10](ch10-privacy-and-gdpr.md)).

**10. Capacitación del personal.** ¿Qué le enseñarás al equipo sobre esta automatización y cómo reportarán un problema?

Ponlo en una página. Compártelo con las personas involucradas. Guárdalo donde puedas encontrarlo en el mal día. Un plan que escribiste en un día tranquilo vale diez veces más que un plan que inventas en una crisis.

## Lista de verificación

### 20.9 Lista de verificación: las 15 preguntas de seguridad

Antes de dejar que una automatización con IA toque datos reales, responde estas quince preguntas. Cada una debe ser un "sí" claro.

- [ ] **1. Menor acceso:** ¿Tiene la automatización solo los datos que realmente necesita, y nada más?
- [ ] **2. Humano en el envío:** ¿Hay un humano revisando todo lo que llega a un cliente?
- [ ] **3. Ubicación de los datos:** ¿Conozco todos los sistemas que los datos tocan, incluidos los que están fuera de mi control?
- [ ] **4. Herramientas verificadas:** ¿Me he negado a alimentar con datos sensibles a cualquier herramienta que no pueda justificar?
- [ ] **5. Cifrado en tránsito:** ¿Están los datos cifrados mientras se mueven entre sistemas?
- [ ] **6. Cifrado en reposo:** ¿Están los datos cifrados mientras se almacenan?
- [ ] **7. Inicios de sesión individuales:** ¿Cada persona tiene su propio inicio de sesión, sin compartir?
- [ ] **8. Autenticación de dos factores:** ¿Está activado el 2FA en las cuentas importantes?
- [ ] **9. Funciones separadas:** ¿Están la configuración, la aprobación y la revisión de registros repartidos entre varias personas?
- [ ] **10. Revisión del acceso:** ¿Actualizo el acceso el día que el personal se incorpora, se mueve o se va?
- [ ] **11. Registro:** ¿Estoy registrando lo que la IA lee, escribe, envía y rechaza?
- [ ] **12. Registros vigilados:** ¿Alguien está realmente revisando los registros, con alertas para las señales importantes?
- [ ] **13. Interruptor de emergencia:** ¿Puedo apagar la automatización al instante, y sé cómo?
- [ ] **14. Plan de incidentes:** ¿Tengo un plan escrito y con nombres para detectar, contener, evaluar, corregir y reportar?
- [ ] **15. Personal capacitado:** ¿Se ha enseñado al equipo a detectar trucos y reportar problemas de forma segura?

Si alguna respuesta es "no", la automatización no está lista. Arréglala antes de salir en vivo. La seguridad no es un producto que compras una vez; son quince preguntas a las que sigues respondiendo que sí.

## Puntos clave

- La seguridad desde el diseño significa incorporar la seguridad desde el inicio: menor acceso, un humano en el envío y un interruptor de emergencia, para que el peor caso siga siendo pequeño.
- Un registro que nadie lee no es seguridad: recoge historiales, configura alertas y asigna a alguien que realmente mire.
- El cifrado oculta los datos a los agentes externos (en tránsito y en reposo), mientras que el control de acceso limita quién tiene la clave: necesitas ambos trabajando juntos.
- Escribe tu plan de respuesta a incidentes en un día tranquilo: detectar, contener, evaluar, corregir, reportar, aprender, con nombres asignados a cada paso.
- El factor humano es la primera defensa: capacita al personal para detectar trucos y reportar de forma segura, y haz que el camino seguro sea el camino fácil.
