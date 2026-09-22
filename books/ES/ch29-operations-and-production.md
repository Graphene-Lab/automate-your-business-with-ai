# Capítulo 29 — Operaciones y producción

## En palabras simples

Las operaciones son el motor de un negocio. Es todo lo que convierte entradas en salidas: fabricar un producto, moverlo, mantener las máquinas funcionando, comprobar la calidad y mantener a la gente a salvo. La producción es la parte de las operaciones que realmente hace la cosa. Cuando el motor funciona bien, los clientes reciben lo que pidieron, a tiempo, sin defectos. Cuando tartamudea, todo lo que viene después lo siente.

Piensa en tu operación como una nave de fábrica, ya fabriques artilugios o ofrezcas servicios. Las máquinas funcionan, las mercancías se mueven, la gente trabaja, y algo siempre puede salir un poco mal —una máquina a punto de fallar, un lote con un defecto, una entrega que llegará tarde, un trabajador en un lugar inseguro—. Un buen operador ve estas cosas pronto. La IA ayuda vigilándolo todo a la vez y señalando las pequeñas señales que un ojo humano cansado pierde.

Este capítulo cubre cuatro trabajos: mantenimiento predictivo (arreglar máquinas antes de que se rompan), control de calidad (pillar defectos automáticamente), logística (mover mercancías e información con eficiencia) y seguridad laboral (mantener a la gente fuera de peligro). Cada uno es un lugar donde una pequeña empresa puede recortar desperdicio, elevar la calidad y proteger a su gente.

Una idea honesta primero: la IA en operaciones es un *vigilante y un ayudante*, no un piloto automático que dirige solo la nave. Sensa, predice y sugiere. Una persona sigue decidiendo cuándo parar una línea, cuándo rechazar un lote, y cuándo mandar a alguien a casa porque no es seguro. El método para juzgar si todo esto compensa vive en el [Capítulo 16 — Objetivos, costes y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md); este capítulo te muestra qué automatizar y cómo. Para ver dónde se sientan las operaciones en el mapa de impacto y esfuerzo de todo tu negocio, mira el [Capítulo 12 — Dónde puede ayudar la IA a tu negocio](ch12-where-ai-can-help-your-business.md).

## Un poco de historia

**Años 1900–1950: la línea de montaje y el mantenimiento preventivo.** La producción moderna empezó con la línea de montaje en movimiento, que dividía el trabajo en pequeños pasos repetibles. Junto a ella llegó el mantenimiento *preventivo* —el hábito de revisar una máquina en un horario fijo, como cambiar el aceite de un coche cada pocos miles de millas, lo necesitara o no—. Esto reducía las averías pero desperdiciaba servicio en máquinas que estaban bien.

**Años 1960–1980: automatización y control de calidad.** Las fábricas añadieron máquinas automatizadas y control de calidad formal —inspeccionar productos contra un estándar y separar lo bueno de lo malo—. Los métodos estadísticos de calidad pillaban defectos en lotes. Esto elevó la calidad pero aún dependía de humanos para inspeccionar y de reglas fijas para revisar las máquinas.

**Años 1990: sensores y la cadena de suministro digital.** Sensores baratos dejaron que las máquinas informaran de su propio estado —temperatura, vibración, horas de funcionamiento—. Las cadenas de suministro se volvieron digitales, con software rastreando mercancías del proveedor al cliente. Por primera vez, un operador podía ver, en una pantalla, qué pasaba en toda la nave y en toda la cadena de suministro. Pero los datos se leían sobre todo a mano.

**Años 2000: el aprendizaje automático predice la avería.** El aprendizaje automático —software que aprende patrones de muchos ejemplos— cambió el mantenimiento. En lugar de revisar en un horario fijo, podías aprender de los datos de sensores cuándo una máquina *realmente* estaba a punto de fallar. Un patrón de vibración creciente que un humano no podía sentir se volvía una clara advertencia con días de antelación. Este fue el nacimiento del mantenimiento *predictivo*.

**Años 2010: la visión por computador inspecciona la calidad.** La visión por computador —IA que lee lo que ve una cámara— empezó a inspeccionar productos automáticamente. Una cámara podía ver una grieta, un arañazo o una pieza que falta más rápido y de forma más constante que un inspector humano, y sin cansarse. El control de calidad pasó de muestrear a comprobar cada unidad.

**Años 2020: los agentes ejecutan el flujo de trabajo.** Los grandes modelos de lenguaje y los agentes de IA —software que toma una tarea entera y la lleva a través de varios pasos— ahora ejecutan partes del propio flujo operativo: leer una petición, sacar datos de sistemas de backend y ejecutar el siguiente paso. El ejemplo de SOK Finance de abajo es exactamente esto: agentes de IA gestionando las operaciones de servicio diarias de un centro financiero, con humanos supervisando.

El arco: de horarios fijos, a inspección manual, a datos de sensores, a IA que predice y ve, a agentes que actúan. Cada paso movió la vigilancia y el trabajo rutinario al software y dejó a los humanos decidir e intervenir.

## Curiosidad

### 29.5 El centro de servicio que puso agentes de IA en primera línea

Cuando oímos «operaciones y producción», imaginamos una fábrica. Pero las operaciones también significan el centro de servicio que mantiene un negocio funcionando —el lugar donde llegan peticiones y alguien debe actuar sobre ellas rápido—.

SOK Finance, en Finlandia, gestiona un centro de servicio llamado Palveluässä que proporciona servicios de gestión financiera y de nóminas para el S Group —una red finlandesa de propiedad de clientes de empresas minoristas y de servicio con unas 2.000 sucursales—. Cada día llegan peticiones: «Envíame una copia de esta factura», «Cambia la fecha de vencimiento de este pago». Rutinario, de alto volumen y sensible al tiempo.

La curiosidad es qué hizo la empresa con ello. En lugar de contratar más gente para responder las mismas peticiones, pusieron *agentes* de IA en primera línea para manejar las rutinarias, para que el personal humano pudiera centrarse en los casos que necesitaban criterio. Ese cambio —de humanos haciendo cada petición a agentes haciendo lo rutinario y humanos supervisando— es la misma revolución silenciosa que ocurrió en la nave de fábrica, ahora aplicada a un centro de servicio. La historia completa, con la fuente real, está debajo.

## Un ejemplo empresarial real

**SOK Finance: agentes de IA ejecutando el flujo de trabajo del centro de servicio.**

SOK Finance opera el centro de servicio Palveluässä, que proporciona servicios de gestión financiera y de nóminas para el S Group, una red finlandesa de propiedad de clientes de empresas minoristas y de servicio con aproximadamente 2.000 sucursales. El centro de servicio gestiona un flujo constante de peticiones rutinarias de toda esa red —cosas como pedir una copia de una factura o cambiar una fecha de vencimiento de pago—. Cada petición es pequeña, pero juntas son una carga de trabajo grande y repetitiva que debe gestionarse rápido y de forma constante.

Según una nota de prensa de CGI (Helsinki, 23 de abril de 2026), CGI diseñó, implementó y desplegó una **solución multiagente de IA construida sobre AWS Bedrock** para SOK Finance, llevando la IA a uso en producción real en administración financiera y servicio al cliente. Una solución «multiagente» significa que varios agentes de IA trabajan juntos en una tarea, cada uno manejando un paso. En este caso, los agentes procesan mensajes entrantes de servicio al cliente, recuperan los datos necesarios de sistemas de backend y llevan a cabo automáticamente partes del proceso.

La nota describe la solución como acelerando significativamente procesos rutinarios como **peticiones de copia de factura y cambios de fecha de vencimiento**, y como mejorando la eficiencia y la consistencia comparado con la gestión manual anterior. CGI fue responsable del diseño, la implementación, el despliegue y la integración con los sistemas clave de SOK Finance.

Dos cosas vale la pena notar. Primera, el rol humano cambia de *hacer cada petición* a *supervisar los agentes y manejar las excepciones*. Los agentes toman lo rutinario; las personas toman lo inusual y lo sensible. Segunda, la victoria es la consistencia tanto como la velocidad —un agente sigue los mismos pasos cuidadosos cada vez, donde una persona cansada una tarde ocupada puede fallar—.

Una nota sobre la fuente y las cifras: las cifras de arriba vienen del anuncio publicado por CGI. La nota describe los resultados en términos cualitativos —procesos más rápidos, mejor consistencia— y no publica un porcentaje duro de tiempo ahorrado o coste reducido. Trata el resultado como la experiencia reportada por la empresa, y recuerda que tus propios números dependerán de tu volumen y tus sistemas. El punto del caso es el *patrón*: agentes de IA ejecutando un flujo de servicio rutinario en producción, con humanos supervisando, a la escala de una red de 2.000 sucursales.

## Cómo hacerlo

### 29.1 Mantenimiento predictivo

El mantenimiento predictivo significa arreglar una máquina *antes* de que se rompa, prediciendo la avería a partir de datos en lugar de esperar a que ocurra o revisar en un horario fijo.

**El modo antiguo y su coste.** Tradicionalmente tenías dos opciones: hacer funcionar una máquina hasta que fallara (y pagar una parada no planificada), o revisarla en un horario fijo (y desperdiciar dinero revisando máquinas que estaban bien). Ambas pierden. Una avería inesperada detiene la producción en el peor momento y cuesta mucho más que una reparación planificada.

**Cómo predice la IA.** Pones sensores en la máquina para medir cosas como vibración, temperatura, sonido y horas de funcionamiento. La IA aprende el patrón normal y ve las primeras señales de problema —una vibración que sube lentamente, una temperatura que corre un poco caliente—. Esos pequeños cambios a menudo aparecen días antes de una avería. La IA te avisa a tiempo para arreglar la máquina durante una parada planificada, no en medio de una corrida.

**Qué ahorra.** El gran ahorro es evitar el tiempo de inactividad no planificado —la avería sorpresa que detiene todo—. Una reparación planificada una martes por la tarde es barata; una avería durante tu pedido más grande del mes es cara. El mantenimiento predictivo convierte lo segundo en lo primero.

**Empieza pequeño.** No necesitas sensores en cada máquina. Empieza con la una o dos máquinas cuya avería más duele —el cuello de botella, la de largo tiempo de reparación, la que detiene toda la línea—. Ponle unos pocos sensores y observa. Prueba el valor ahí antes de expandirte.

**El humano decide la parada.** La IA señala el riesgo; una persona decide cuándo bajar la máquina. No dejes que el sistema detenga la producción por su cuenta sin un humano confirmando la decisión. La advertencia es el valor; la decisión se mantiene humana.

### 29.2 Control de calidad

El control de calidad significa comprobar que un producto cumple su estándar y pillar defectos antes de que el producto llegue al cliente. La IA cambia el control de calidad de *muestrear* a *comprobar cada unidad*, y de *ojos cansados* a *ojos consistentes*.

**La visión por computador inspecciona.** Una cámara más IA puede mirar cada producto en la línea y ver una grieta, un arañazo, una pieza que falta, una etiqueta equivocada o una costura mala. Comprueba cada unidad, no solo una muestra, y no se cansa ni se aburre. Un inspector humano comprobando miles de unidades al día perderá cosas; la cámara no.

**La consistencia es la victoria.** Los humanos varían. Una persona está más despierta por la mañana, más lenta después de comer, y se deja llevar fácilmente por lo que vio la última vez. La IA aplica el mismo estándar a cada unidad, todo el día. Esa consistencia vale mucho en un negocio donde un defecto que llega a un cliente cuesta una devolución, una queja o una reputación.

**Pílalo pronto.** Cuanto antes pilles un defecto, más barato es. Un defecto pillado en la máquina que lo hizo cuesta una pieza. El mismo defecto pillado en el ensamblaje final cuesta una rehacer. Pillado por el cliente, cuesta una devolución y confianza. La IA en cada estación pilla problemas en la fuente, no al final.

**Empieza con el defecto costoso.** No intentes inspeccionarlo todo al principio. Encuentra el defecto que más te cuesta —el que causa más devoluciones o quejas— y pon una comprobación de visión en eso. Prueba que pilla el problema caro, y luego añade más comprobaciones.

**Mantén un humano para la decisión de criterio.** La IA puede señalar una unidad sospechosa; una persona decide si es realmente defectuosa, especialmente en casos límite. No dejes que un sistema de visión deseche buen producto porque fue demasiado estricto. Revisa los rechazos y ajusta el umbral.

### 29.3 Logística

La logística es el movimiento de mercancías e información: conseguir la cosa correcta al lugar correcto en el momento correcto, al menor coste. Es un rompecabezas de rutas, existencias, tiempos y proveedores, y la IA es muy buena en rompecabezas como este.

**Optimización de rutas y entregas.** La IA puede planificar rutas de entrega que ahorren millas, combustible y tiempo, tomando en cuenta el tráfico, las ventanas de entrega y el tamaño de carga. Para un negocio con una flota, incluso un pequeño ahorro por ruta se acumula rápido a lo largo de un año.

**Previsión de existencias y demanda.** La IA mira tu historial de ventas y predice qué necesitarás y cuándo, para que almacenes lo suficiente sin sobrecomprar. Pocas existencias significan una venta perdida; demasiadas significan efectivo inmovilizado y desperdicio. La IA equilibra lo dos aprendiendo tus patrones y estacionalidad.

**Pilla el cuello de botella.** La IA puede ver dónde se ralentizan las mercancías —un proveedor que siempre llega tarde, un paso de almacén que se atasca, una ruta que siempre se pasa—. Ver el cuello de botella es el primer paso para arreglarlo. Todo el valor es hacer visible el retraso invisible.

**Conecta los sistemas.** La IA de logística funciona mejor cuando puede ver tus pedidos, tus existencias y tus entregas juntas. Conectar la IA a los sistemas que ya usas —tus pedidos, tu inventario, tu seguimiento— es lo que hace el cuadro completo. El cómo para esa conexión está en el [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).

**Mantén un humano para la excepción.** La IA planifica lo rutinario; una persona maneja la sorpresa —la huelga, la tormenta, el proveedor que falla—. No dejes que un plan optimizado choque con una disrupción del mundo real sin un humano listo para anularlo. El plan es un punto de partida, no una camisa de fuerza.

### 29.4 Seguridad laboral

La seguridad laboral significa mantener a la gente fuera de peligro. La IA puede vigilar condiciones inseguras y comportamiento inseguro y avisar antes de que ocurra un accidente. Este es uno de los usos más valiosos de la IA, porque lo que protege es una persona.

**La visión por computador vigila peligros.** Cámaras más IA pueden ver un trabajador sin el equipo de protección adecuado, una persona de pie en una zona peligrosa, un derrame en el suelo, o una salida de emergencia bloqueada. Cuando ve uno, lanza una alerta para que el peligro se arregle antes de que alguien salga dañado.

**Predice el momento arriesgado.** La IA puede aprender cuándo los accidentes son más probables —un turno cierto, una máquina cierta, una hora del día cuando la gente está cansada— e incrementar la vigilancia entonces. Es como tener un responsable de seguridad que nunca parpadea y ve toda la nave a la vez.

**Una línea legal seria: no leas emociones.** La IA que infiere las *emociones* de un trabajador de su cara o voz está prohibida en el lugar de trabajo bajo el Reglamento de IA de la UE. La visión de seguridad trata de *peligros y equipo*, no de cómo se *siente* un trabajador. Mantén la cámara en la nave y la máquina, no en el estado de ánimo de la persona. La lista completa de prácticas prohibidas está en el [Capítulo 5 — Reglas y responsabilidad legal](ch05-rules-and-legal-responsibility.md).

**Avisa a tus trabajadores.** Si usas monitorización de seguridad basada en IA que afecta a los trabajadores, debes informar a tus trabajadores y sus representantes antes de empezar, como exige la ley para IA de alto riesgo en el lugar de trabajo. Sé abierto sobre qué vigilan las cámaras y por qué. El secretismo rompe la confianza. La regla de aviso al trabajador se trata en la Curiosidad de este capítulo y en el [Capítulo 5](ch05-rules-and-legal-responsibility.md).

**Úsalo para proteger, no para castigar.** Los datos de seguridad deben hacer el lugar de trabajo más seguro —arreglar el peligro, cambiar el proceso, formar al equipo—. No deben volverse una herramienta para disciplinar a individuos por cada pequeño fallo. Úsalos para encontrar y eliminar el peligro, no para armar un caso contra un trabajador.

## Ética y responsabilidad

Las operaciones tocan la seguridad y el medio ambiente, así que las apuestas éticas son reales y concretas.

**Las decisiones de seguridad se mantienen humanas.** La IA puede avisar de un peligro, pero una persona decide cuándo parar una línea o mandar a alguien a casa. Nunca dejes que un sistema tome una decisión crítica para la seguridad sin un humano en el bucle. Un «todo despejado» falso puede dañar a alguien.

**Respeta la privacidad y los derechos de los trabajadores.** Cámaras y sensores en el lugar de trabajo vigilan a personas. Úsalos para seguridad y operaciones, no para vigilancia. Di a los trabajadores qué se vigila y por qué, y sigue las reglas de privacidad del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md).

**Nunca leas emociones.** El reconocimiento de emociones en el lugar de trabajo está prohibido. Mantén la monitorización en peligros y equipo, nunca en los sentimientos de un trabajador.

**Protege los datos operativos.** Los datos de sensores, los calendarios de producción y los registros de la cadena de suministro son sensibles y valiosos. Mantenlos seguros y, donde importe, dentro de tu propio entorno. Los fundamentos de seguridad están en el [Capítulo 6 — Ciberseguridad en la era de la IA](ch06-cybersecurity-in-the-ai-era.md), y la opción de autoalojamiento en el [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md).

**Sé honesto sobre los resultados.** Un número de calidad o eficiencia que parece demasiado bueno debe comprobarse antes de reportarlo. Reporta las cifras reales, incluidas las fallas, para que puedas arreglar lo que sigue roto.

**Usa los datos para mejorar, no para castigar.** Los datos operativos y de seguridad deben hacer el trabajo mejor y más seguro para todos. Cuando se vuelven un palo para golpear a individuos, envenenan el lugar de trabajo y esconden los problemas reales.

## Errores a evitar

**Esperar a la avería.** Aferrarse a funcionar-hasta-fallar cuando una reparación planificada era barata y predecible. Predice y actúa pronto.

**Sensores sin un plan.** Recoger datos en los que nunca actúas. Empieza con la máquina que más duele y ata cada sensor a una decisión.

**Dejar que la IA pare o deseche sola.** Sin control humano en una parada de línea o un rechazo de producto. Mantén la decisión humana.

**Comprobaciones de visión demasiado estrictas.** Un sistema de calidad que desecha buen producto porque el umbral es demasiado ajustado. Revisa los rechazos y ajústalo.

**Inspeccionar el defecto equivocado.** Poner visión en un problema barato mientras el caro se cuela. Atina al defecto costoso primero.

**Un plan que ignora el mundo real.** Dejar que un plan logístico optimizado choque con una disrupción sin anulación humana. Mantén una persona lista.

**Reconocimiento de emociones en el trabajo.** Usar IA para leer los sentimientos de los trabajadores. Está prohibido y es incorrecto.

**Monitorización secreta.** No avisar a los trabajadores antes de que empiece la monitorización de seguridad u operaciones basada en IA. Eso rompe la ley y la confianza.

**Deriva hacia la vigilancia.** Usar datos de seguridad y operaciones para vigilar y castigar a individuos en lugar de eliminar peligros.

**Automatizar un proceso roto.** Si la línea o la cadena de suministro es un desastre, la IA hace un desastre más rápido. Arregla el proceso primero.

**Sin línea base.** No medir el tiempo de inactividad, la tasa de defectos o el tiempo de entrega antes, así que no puedes probar la ganancia. Mide primero (mira el [Capítulo 22 — Medir resultados y ROI](ch22-measuring-results-and-roi.md)).

**Sobreprometer los números.** Citar la cifra del mejor caso de un proveedor como tu resultado. Usa tus propios números medidos.

## Ejercicio práctico

### 29.7 Ejercicio: planifica una automatización de operaciones

Elige un trabajo de operaciones y planifica su asistencia con IA de punta a punta, con la seguridad y la decisión humana integradas.

**Paso 1 — Elige el trabajo.** Elige uno: mantenimiento predictivo, control de calidad, logística o seguridad laboral. Haz uno, no todos.

**Paso 2 — Define el objetivo y la métrica.** ¿Menos tiempo de inactividad? ¿Menos defectos? ¿Entrega más rápida? ¿Menos incidentes de seguridad? Elige un número para medir.

**Paso 3 — Mide la línea base.** ¿Cuál es ese número ahora? Horas de tiempo de inactividad no planificado, tasa de defectos, entregas a tiempo, incidentes al mes. Escríbelo.

**Paso 4 — Encuentra el objetivo costoso.** Identifica la única falla más cara en ese trabajo —la máquina cuya avería más duele, el defecto que más cuesta, la ruta que siempre llega tarde, el peligro que causa más daño—. Atina a ese primero.

**Paso 5 — Marca cada paso.** Para cada paso, márcalo: **la IA lo hace** (sentir, predecir, inspeccionar, planificar), **el humano lo revisa** (confirmar la advertencia, comprobar el rechazo), o **el humano lo decide** (parar la línea, desechar el lote, mandar a alguien a casa). Cada decisión crítica para la seguridad debe ser humana.

**Paso 6 — Comprueba la línea legal.** Si el trabajo implica monitorizar trabajadores, confirma que estás vigilando peligros y equipo, no emociones, y planifica cómo informarás a los trabajadores y sus representantes antes de empezar.

**Paso 7 — Conecta los datos.** Decide qué sistemas necesita ver la IA —sensores, inventario, seguimiento— y cómo los conectarás (mira el [Capítulo 19](ch19-connecting-ai-to-systems-you-already-use.md)).

**Paso 8 — Lanza pequeño y mide.** Ejecútalo en una máquina, una línea o una ruta primero. Compara la métrica con la línea base. Escala solo lo que pruebe que funciona.

Haz un trabajo bien. El análisis de objetivo costoso del paso 4 es valioso por sí solo —te muestra dónde tu operación realmente pierde más dinero o causa más daño, lo cual es útil incluso antes de comprar cualquier herramienta—.

## Lista de comprobación

### 29.8 Lista de comprobación de operaciones y producción

Antes de automatizar cualquier tarea de operaciones, comprueba estas.

- [ ] **Mediste la línea base** —tiempo de inactividad, tasa de defectos, tiempo de entrega, incidentes de seguridad—.
- [ ] **Atinaste a la falla más costosa primero**, no a la más fácil.
- [ ] **Un humano toma cada decisión crítica para la seguridad** —parar una línea, desechar un lote—.
- [ ] **El mantenimiento predictivo está atado a una acción real**, no solo datos recogidos.
- [ ] **Las comprobaciones de calidad están ajustadas** para que no desechen buen producto.
- [ ] **La IA de logística puede ver tus pedidos, existencias y entregas juntas.**
- [ ] **Un humano puede anular el plan optimizado** cuando el mundo real lo interrumpe.
- [ ] **La monitorización de seguridad vigila peligros y equipo, nunca emociones** (el reconocimiento de emociones está prohibido).
- [ ] **Informaste a los trabajadores y sus representantes** antes de cualquier monitorización de IA que les afecte.
- [ ] **Los datos operativos se mantienen seguros**, no enviados a servicios de IA públicos.
- [ ] **Usas los datos para eliminar peligros y mejorar el proceso**, no para castigar a individuos.
- [ ] **Arreglas el proceso roto antes de automatizarlo.**
- [ ] **Reportas tus propios números medidos**, no el mejor caso del proveedor.

Si una casilla está vacía, el riesgo —para tu producto, tu gente o tu confianza— sigue siendo tuyo. Rellénala antes de dejar que la IA se acerque a la nave.

## Puntos clave

- La IA en operaciones es un vigilante y ayudante: sensa, predice, inspecciona y planifica, mientras un humano mantiene cada decisión crítica para la seguridad.
- El caso de SOK Finance (un anuncio de CGI) puso IA multiagente en AWS Bedrock en producción real en un centro de servicio que atiende a una red de ~2.000 sucursales, acelerando peticiones rutinarias como copias de factura y cambios de fecha de vencimiento, con humanos supervisando las excepciones.
- El mantenimiento predictivo convierte una avería sorpresa en una reparación planificada barata; el control de calidad por visión por computador comprueba cada unidad de forma consistente en lugar de muestrear con ojos cansados.
- En seguridad laboral, monitoriza peligros y equipo de protección —nunca las emociones de los trabajadores, que el Reglamento de IA de la UE prohíbe— y avisa a los trabajadores antes de cualquier monitorización que les afecte.
- Atina a la falla más costosa primero, mantén una anulación humana para disrupciones del mundo real, y mide tu propia línea base antes de confiar en el número de ningún proveedor.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que tecleas para obtenerlo.

### Mantén el inventario en orden

![Una hoja de inventario con artículos de stock bajo resaltados](../../assets/examples/inventory-list.png)
*Una hoja de inventario con artículos de stock bajo resaltados*

**Lo que pides:** `Haz una hoja de inventario con artículo, cantidad, nivel de reposición y proveedor, y resalta lo que está por debajo del nivel de reposición.`

El agente monta la hoja de inventario y marca los artículos que necesitan reponerse. Actualiza las cantidades y pídele que vuelva a comprobar cualquier momento.

*Consejo: Una comprobación semanal programada puede decirte qué reponer antes de que te quedes sin existencias.*

---

### Planifica una ruta de entrega

![Una ruta de entrega trazada por las paradas](../../assets/examples/delivery-route.png)
*Una ruta de entrega trazada por las paradas*

**Lo que pides:** `Planifica la mejor ruta para estas cinco direcciones de entrega y muéstrala en un mapa.`

El agente traza las paradas en un mapa en un orden eficiente y te da la distancia y el tiempo estimado. Sigues la ruta y ahorras combustible.

*Consejo: Añade ventanas de tiempo («parada B antes del mediodía») y el agente las tiene en cuenta.*

---

### ¿Está en stock?

![Una comprobación de stock en vivo respondida en segundos](../../assets/examples/stock-check.png)
*Una comprobación de stock en vivo respondida en segundos*

**Lo que pides:** `¿Tenemos el artículo SKU 3391 en stock, y cuántos?`

El agente comprueba el stock en tu sistema y responde con la cantidad, para que puedas prometer o no prometer con confianza.

*Consejo: Complementalo con una alerta de stock bajo programada a diario para evitar sorpresas.*

<!-- END agentbridge-examples -->
