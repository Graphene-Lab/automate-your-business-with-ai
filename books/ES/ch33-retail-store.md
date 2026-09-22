# Capítulo 33 — Una tienda minorista

*Este capítulo es una composición representativa. No es una tienda real. Reúne los patrones comunes que vemos en minoristas independientes que adoptan la IA. Todas las cifras son ilustrativas —muestran la forma de la decisión, no una promesa. Reemplázalas por las tuyas.*

## Contexto

Imagina una tienda independiente de propiedad familiar. La llamaremos **Cornerstone Home & Garden**. Vende herramientas, pintura, artículos de jardín y pequeños enseres domésticos. Una tienda física, más una pequeña tienda en línea. Unos quince empleados. Lleva unos pocos miles de productos distintos —cada uno un **SKU**, que simplemente significa un artículo distinto con su propio código, como "taladro de 18 voltios, modelo X" o "pintura plástica verde de 5 litros."

La tienda funciona con un sistema **POS** —la caja del punto de venta que registra cada venta. Esa caja sabe qué se vendió y cuándo. Pero saber qué se vendió no es lo mismo que saber qué pedir la próxima semana, o qué pregunta un cliente en el mostrador, o cómo traer gente de vuelta por la puerta.

Durante años, todo eso se hizo por intuición. El dueño, Marco, reabastece cuando un estante parece bajo. Adivina cuánto stock de palas de nieve comprar cada invierno basándose en el invierno pasado, que no se parecía en nada a este. Las preguntas de clientes llegan por teléfono y correo y se responden cuando alguien está libre. El marketing es un envío ocasional de correo que Marco teclea él mismo, a todos, con el mismo mensaje. La tienda sobrevive. Pero inmoviliza efectivo en el stock equivocado, pierde ventas cuando el artículo correcto se agota, y gasta dinero de marketing que apenas mueve la aguja.

Un pequeño minorista independiente compite contra grandes cadenas que tienen equipos enteros haciendo previsión y marketing. Cornerstone no puede contratar un equipo. Pero puede apuntar unas pocas herramientas de IA a los mismos trabajos.

## El problema

Las fugas en una tienda pequeña son fáciles de nombrar.

**Sobre-stock y roturas de stock.** Cuando Marco adivina mal por arriba, un stock caro se queda en el estante durante meses. Eso es efectivo congelado —dinero que podría usarse en otra parte está encerrado en cajas que nadie compra. Esto se llama **stock muerto**. Cuando adivina mal por abajo, el artículo se agota, y el cliente se va sin comprar —o peor, lo compra en un competidor y deja de volver. Ambos errores cuestan dinero, y ambos vienen de adivinar.

**Fallos estacionales.** La demanda oscila con la estación e incluso con el clima. Un invierno suave deja palas de nieve sin vender. Una repentina ola de calor vacía las regaderas antes de que Marco pueda reabastecer. La memoria humana de "el año pasado" es un mal guía para este año.

**Servicio al cliente lento.** Preguntas como "¿tienen esto en stock?" o "¿cuál es su horario?" o "¿puedo devolver esto?" se acumulan por teléfono y correo. Responderlas es simple pero roba tiempo del piso de la tienda. Sin responder, se convierten en ventas perdidas.

**Marketing genérico.** El envío de correo de Marco va a todos con el mismo mensaje. Un jardinero y un pintor reciben el mismo correo. La mayor parte se ignora. El gasto de marketing es pequeño, pero el retorno es más pequeño porque no apunta a nadie en particular.

Si quieres ver cómo estas cuatro se clasifican frente al resto de tu tienda, el método de impacto y esfuerzo del [Capítulo 12 — Dónde puede ayudar la IA a tu negocio](ch12-where-ai-can-help-your-business.md) es el lugar para puntuarlas.

## La solución

Marco elige las cuatro fugas y empieza con la que libera más efectivo con menos riesgo.

**Previsión de la demanda para el stock.** La tienda conecta su historial de ventas del POS a una herramienta de previsión. La herramienta mira qué se vendió, cuándo, y qué tan rápido, y añade patrones estacionales. Luego sugiere qué pedir y cuánto, en vez de dejarlo a la intuición de Marco. No hace el pedido ella misma. Levanta una sugerencia: "Normalmente vendes esto en tres semanas; pide ahora." Una persona lo confirma. La adivinanza se convierte en un aviso. (El tratamiento más profundo de la previsión de la demanda y el inventario está en el [Capítulo 29 — Operaciones y producción](ch29-operations-and-production.md).)

**Alertas de stock.** Encima de la previsión, la tienda fija alertas simples: cuando un artículo cae por debajo de un nivel seguro, márcalo; cuando un artículo no se ha vendido en mucho tiempo, márcalo como posible stock muerto. Marco ve ambas y actúa.

**Un chatbot para las preguntas comunes.** Un chatbot en el sitio web y la tienda en línea responde las preguntas repetidas —stock, horario, devoluciones, entrega— al instante, en lenguaje simple, en más de un idioma si hace falta. El personal al teléfono queda libre para las preguntas que necesitan una persona. Este es el mismo patrón de chatbot de servicio al cliente visto en el [Capítulo 27 — Atención y soporte al cliente](ch27-customer-care-and-support.md), y el mismo tipo de agente guía de compras que describe el caso de mobilezone en el [Capítulo 26 — Ventas y marketing](ch26-sales-and-marketing.md).

**Marketing que apunta.** En vez de un envío a todos, un asistente de marketing ayuda a Marco a dividir su lista de clientes en grupos —jardineros, pintores, habituales— y redactar un mensaje distinto para cada uno. La IA escribe los borradores; Marco los revisa contra la voz de la tienda antes de enviar. El mismo gasto llega a la gente correcta con el mensaje correcto.

Fíjate en el patrón. La IA predice, marca, responde y redacta. Un humano confirma el pedido, maneja las preguntas difíciles, y aprueba el marketing. La tienda mantiene el control en cada paso.

## Las herramientas

Nada de esto requirió un científico de datos. Las herramientas son comerciales y apuntan a pequeños minoristas.

- **Un complemento de previsión** para el POS o el sistema de inventario. Muchos sistemas de caja modernos ya incluyen una función de "sugerir un reabastecimiento" que lee tu propio historial de ventas.
- **Alertas de stock simples**, a menudo integradas en la misma herramienta de inventario.
- **Un chatbot de servicio al cliente** en el sitio web, conectado a la lista de productos de la tienda para poder responder "¿tienen esto?" con precisión.
- **Un asistente de marketing** que segmenta la lista de clientes y redacta correos de campaña y publicaciones sociales.

Cómo elegir entre estas sin dejarse engañar por una demo brillante se trata en el [Capítulo 17 — Elegir herramientas sin ser engañado](ch17-choosing-tools-without-being-fooled.md). Cómo conectarlas al POS y a la lista de clientes que ya tienes está en el [Capítulo 19 — Conectar la IA a los sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).

Una cautela específica del comercio minorista: la lista de clientes guarda datos personales —nombres, correos, historial de compras—. Las reglas de privacidad del [Capítulo 10 — Privacidad y GDPR](ch10-privacy-and-gdpr.md) se aplican a cómo esa lista se usa para marketing, incluido obtener consentimiento para enviar correo a la gente.

## Los costos

Aquí hay un presupuesto ilustrativo del primer año para una tienda como Cornerstone. Son números inventados para mostrar la forma. Usa los tuyos.

**Costos directos.**
- Complemento de previsión e inventario: unos 4.800 € al año.
- Chatbot de servicio al cliente: unos 3.600 € al año.
- Asistente de marketing: unos 3.600 € al año.
- Configuración e integración con el POS y la lista de clientes: unos 7.000 de una sola vez.
- Formación del personal: unos 2.000 de una sola vez.

Total del primer año: aproximadamente **21.000 €**. En años estables después, las suscripciones recurrentes suman unos **12.000 €**.

**Costos indirectos.**
- Tiempo del personal para revisar las sugerencias de reabastecimiento y las respuestas del chatbot.
- El bajón de aprendizaje mientras todos confían en el nuevo sistema.
- Alguien debe revisar los borradores de marketing antes de que salgan, para que la voz de la tienda siga siendo correcta.
- Limpiar el historial de ventas para que la previsión tenga buenos datos de los que aprender.

El método completo para contar estos costos y convertir el ahorro en una cifra de retorno está en el [Capítulo 16 — Objetivos, costos y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md). No hagas las cuentas de cabeza. Anótalas.

## Los resultados

Tras un año, medido contra una línea base que Marco registró antes de empezar, el resultado ilustrativo se ve así. Tus números diferirán. Estos muestran a qué puede parecerse un buen encaje.

- **Bajaron las roturas de stock.** Menos clientes se fueron con las manos vacías porque la previsión marcó el reabastecimiento pronto.
- **Bajó el stock muerto.** Menos efectivo quedó congelado en cajas que nadie quería, porque la herramienta vio los movimientos lentos y el exceso de pedido antes de que ocurriera.
- **Efectivo liberado.** Con menos dinero encerrado en el stock equivocado, la tienda tuvo efectivo para usar en otra parte.
- **Preguntas de clientes respondidas al instante.** El chatbot gestionó las comunes día y noche, y la cola telefónica se acortó.
- **El marketing trabajó más duro.** Los mensajes segmentados y apuntados obtuvieron más respuesta que el viejo envío de talla única, con el mismo pequeño presupuesto.

La cautela honesta: nada de esto fue instantáneo. La previsión fue tosca los primeros meses porque necesitaba un año limpio de historial de ventas para aprender. El chatbot dio respuestas erróneas al principio hasta que se le alimentó con datos de producto exactos. Las ganancias se aceleraron a lo largo de semanas, como predice la advertencia de la curva de aprendizaje del [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). Marco midió los números reales tras la rampa, no durante ella.

## Lecciones aprendidas

**La previsión es solo tan buena como tu historial de ventas.** Una herramienta de previsión aprende de tus ventas pasadas. Si el historial está desordenado o incompleto, la previsión es débil. Limpiar los datos primero fue lo más valioso que hizo Marco. La preparación de datos se trata en el [Capítulo 14 — Datos: la materia prima](ch14-data-the-raw-material.md).

**Empieza por el efectivo.** De las cuatro fugas, el stock fue el de mayor impacto porque el stock muerto inmoviliza dinero real. También fue de bajo riesgo, porque una persona confirma cada pedido. Eso lo hizo el proyecto ideal para empezar —la regla de "primero el de alto impacto y alta facilidad" del [Capítulo 12](ch12-where-ai-can-help-your-business.md).

**Nunca dejes que la IA pida por su cuenta.** Una sugerencia de reabastecimiento es segura. Una orden de compra automática sin humano y sin tope de gasto no lo es. Un fallo o una mala previsión puede pedir miles de unidades que nadie quiere. Mantén un humano y un tope en cada pedido.

**El chatbot necesita buenos datos de producto.** Solo puede responder "¿tienen esto?" si la lista de stock que lee es exacta. Un chatbot alimentado con datos erróneos da respuestas erróneas con confianza y molesta a los clientes.

**El marketing de IA redacta; tú conservas la voz.** El asistente escribe rápido, pero no conoce el tono de tu tienda. Lee cada borrador antes de que salga. Y respeta el consentimiento —solo envía correo a gente que acordó recibir correo, como requiere el [Capítulo 10](ch10-privacy-and-gdpr.md).

**Un modelo se rompe con una sorpresa.** La previsión aprende del pasado. Un evento una vez por década —una tormenta, una escasez repentina— rompe el patrón. La herramienta no lo verá venir. Mantente listo para anularlo con tus propios ojos.

**Mide con honestidad y espera la rampa.** Registra la línea base antes de empezar. Juzga el proyecto tras la curva de aprendizaje, no durante ella.

La lección del pequeño minorista es la misma que la de todos los demás sectores: encuentra la fuga, elige la más fácil de alto valor —normalmente el stock que inmoviliza efectivo—, deja que la IA prediga y redacte, mantén un humano en el pedido y el mensaje, y mide con honestidad. Una tienda independiente de quince personas puede hacer esto. Las herramientas están listas. Lo único que falta es una mirada clara a dónde está atascado el efectivo.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### ¿Dónde debería abrir a continuación?

![Dos ubicaciones candidatas mostradas en un mapa](../../assets/examples/location-analysis.png)
*Dos ubicaciones candidatas mostradas en un mapa*

**Lo que pides:** `Muestra estas dos ubicaciones candidatas de tienda en un mapa y anota qué hay cerca de cada una.`

El agente mapea ambos sitios y anota características cercanas —flujo peatonal, competidores, aparcamiento— para ayudarte a sopesar la elección.

*Consejo: Combina esto con un paso de investigación web del vecindario para una imagen más completa.*

<!-- END agentbridge-examples -->
