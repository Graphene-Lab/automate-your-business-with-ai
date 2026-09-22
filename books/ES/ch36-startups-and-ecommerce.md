# Capítulo 36 — Startups y comercio electrónico

*Este capítulo es un compuesto representativo. No es una empresa real. Combina los patrones comunes que vemos en startups ágiles y pequeñas tiendas en línea que adoptan IA. Todos los números son ilustrativos —muestran la forma de la decisión, no una promesa—. Reemplázalos por los tuyos.*

## Contexto

Imagina una pequeña tienda en línea. La llamaremos **Lumen Goods**. Vende un producto físico directamente a clientes por internet —en este caso, iluminación para el hogar—. La empresa tiene seis personas. La fundadora, Sara, más un pequeño equipo donde cada uno lleva varios sombreros: una persona se encarga de envíos y existencias, otra del marketing, todos ayudan con las preguntas de clientes cuando la cola crece.

Lumen vende a través de su propio sitio web y un par de mercados en línea. El catálogo tiene unos pocos cientos de productos —cada uno un **SKU**, un artículo distinto con su propio código, como «lámpara de escritorio de latón, pequeña»—. Los pedidos llegan a todas horas de todo el país.

Una startup ágil es distinta de una empresa establecida en una forma que importa aquí. Casi no tiene gente de sobra. Cada hora que una fundadora pasa respondiendo «dónde está mi pedido» es una hora que no pasa construyendo el negocio. Lumen no puede contratar un equipo de soporte, un equipo de redacción y un equipo de datos. Pero enfrenta los mismos trabajos que esos equipos hacen: responder a clientes, escribir páginas de producto, recomendar el producto correcto, mantener el catálogo y los pedidos en orden.

Esta es exactamente la situación donde un equipo pequeño puede pegar por encima de su peso. Las grandes tiendas en línea tienen departamentos enteros para estos trabajos. Lumen puede apuntar unas pocas herramientas de IA a los mismos trabajos y cubrirlos con seis personas.

## El problema

Las fugas en una tienda en línea ágil son fáciles de nombrar.

**El soporte se come a los fundadores.** La pregunta más común con diferencia es «dónde está mi pedido» —a menudo abreviada WISMO—. Añade «¿cómo devuelvo esto?», «¿esto encaja?», «¿combinará con mi habitación?», y la bandeja de entrada se llena. Responder es simple pero constante, y recae en quien esté libre, que a menudo es Sara. Es el mayor drenaje del tiempo de un equipo pequeño.

**El contenido de producto es una montaña.** Unos pocos cientos de productos cada uno necesitan una descripción, texto amigable para búsquedas y una redacción que suene a la marca. Escribir todo a mano lleva semanas, y el catálogo sigue creciendo. Descripciones pobres, que faltan o copiadas dañan a la tienda de dos formas: los clientes no conectan, y la tienda se posiciona mal en los buscadores, así que menos gente la encuentra.

**Sin personalización.** Las tiendas grandes muestran a cada visitante productos que encajan con lo que miró y compró. Un navegador por primera vez y un cliente fiel ven cosas distintas. Lumen muestra a todos la misma página. Deja ventas sobre la mesa porque no puede apuntar.

**Fricción operativa.** Los pedidos salen mal en pequeñas formas —un problema de dirección, un descuadre de existencias entre el sitio web y el mercado, un envío retrasado—. Cada uno necesita un humano para notarlo y arreglarlo. A medida que los pedidos crecen, estas pequeñas excepciones se multiplican y comen en silencio tiempo y buena voluntad.

Si quieres ver cómo se clasifican frente al resto de tu tienda, el método de impacto y esfuerzo del [Capítulo 12 — Dónde puede ayudar la IA a tu negocio](ch12-where-ai-can-help-your-business.md) es el lugar para puntuarlas.

## La solución

Lumen ataca los cuatro trabajos en orden de cuán rápido liberan al equipo, y mantiene un humano en cualquier cosa que toque la marca o la confianza del cliente.

**Un agente de soporte que responde las preguntas comunes y conoce el pedido.** Un chatbot en el sitio web está conectado al sistema de pedidos. Cuando un cliente pregunta «dónde está mi pedido», el bot busca el pedido real y responde con el estado real y el enlace de seguimiento. Maneja devoluciones, tiempos de envío y las usuales preguntas pre-venta al instante, de día y de noche. El equipo solo ve las preguntas que el bot no puede resolver. Es el mismo patrón de chatbot de servicio al cliente tratado en el [Capítulo 27 — Atención y soporte al cliente](ch27-customer-care-and-support.md). La clave es que el bot lee los datos de pedidos reales de la tienda, así que responde con exactitud en lugar de adivinar.

**Contenido de producto que redacta a escala.** Un asistente de contenido escribe un primer borrador de cada descripción de producto desde una especificación breve —las características del producto, los materiales y unas notas—. Puede producir muchos productos en el tiempo que una persona escribe uno. Una persona luego lee cada borrador y lo ajusta a la voz de la marca y comprueba que cada afirmación sea cierta. La página en blanco se ha ido; la voz de marca se mantiene humana.

**Personalización que apunta.** Una herramienta de recomendación observa lo que un visitante navega y muestra productos relacionados que encajan. Un asistente de marketing divide la lista de clientes en grupos y redacta un correo distinto para cada uno —los clientes nuevos reciben una bienvenida, los compradores pasados reciben una sugerencia relevante—. El mismo gasto llega a las personas correctas con el mensaje correcto. Es el mismo patrón de marketing descrito en el [Capítulo 26 — Ventas y marketing](ch26-sales-and-marketing.md).

**Operaciones que señalan las excepciones.** En lugar de una persona buscando problemas, una herramienta vigila los pedidos entrantes y señala los que necesitan atención —una dirección mala, un descuadre de existencias, un retraso— para que el equipo los arregle rápido. El catálogo se mantiene sincronizado entre el sitio web y los mercados. Los pequeños problemas dejan de volverse grandes.

Observa el patrón. La IA responde, redacta, recomienda y señala. Un humano mantiene la voz de marca, comprueba cada afirmación de producto, y maneja los casos que necesitan criterio. El equipo de seis personas cubre trabajo que de otro modo necesitaría muchos más.

## Las herramientas

Nada de esto requirió un científico de datos. La mayor parte está integrado en las herramientas que una pequeña tienda en línea ya usa.

- **Un chatbot de soporte** conectado al sistema de pedidos de la tienda, para que pueda responder «dónde está mi pedido» con el estado real.
- **Un asistente de contenido de producto** que redacta descripciones y texto amigable para búsquedas desde una especificación breve.
- **Un motor de recomendación** que muestra productos relacionados, y un **asistente de marketing** que segmenta la lista de clientes y redacta correos.
- **Una herramienta de monitorización de pedidos** que señala excepciones y mantiene el catálogo sincronizado entre canales.

Muchas plataformas de comercio electrónico ahora incluyen estas funciones directamente. Cómo elegir entre ellas sin ser engañado por una demo brillante está tratado en el [Capítulo 17 — Elegir herramientas sin ser engañado](ch17-choosing-tools-without-being-fooled.md). Cómo conectarlas a la plataforma de la tienda y los datos de pedidos está en el [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).

Una precaución específica del comercio electrónico: la lista de clientes y las herramientas de personalización manejan datos personales —nombres, correos, historial de navegación y compra—. Las reglas de privacidad del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md) se aplican a cómo se usan esos datos, incluido obtener consentimiento para enviar correos a la gente y para rastrear la navegación para recomendaciones.

## Los costes

Aquí hay un presupuesto ilustrativo del primer año para una tienda como Lumen. Estos son números inventados para mostrar la forma. Usa los tuyos. Una startup ágil empieza más barato que una empresa grande, pero vigila los costes por unidad a medida que creces.

**Costes directos.**
- Chatbot de soporte (conectado al sistema de pedidos): unos 3.600 € al año.
- Asistente de contenido de producto: unos 3.600 € al año.
- Motor de recomendación: unos 4.800 € al año.
- Asistente de marketing: unos 3.600 € al año.
- Monitorización de pedidos y sincronización de catálogo: unos 3.000 € al año.
- Configuración e integración con la plataforma de comercio electrónico: unos 6.000 € de pago único.
- Formación del equipo: unos 1.500 € de pago único.

Total del primer año: unos **26.100 €**. En años estables después, las suscripciones recurrentes llegan a unos **18.600 €**.

**Costes indirectos.**
- Alguien debe leer cada borrador de producto y comprobar cada afirmación antes de que se publique.
- La caída de aprendizaje mientras el equipo confía en las nuevas herramientas.
- Muchas de estas herramientas cobran **por uso** —por mensaje, por producto, por correo—. Barato al principio, pero la factura crece con el volumen. Vigílalo a medida que escalas.
- Limpiar el catálogo de productos y la lista de clientes para que las herramientas tengan buenos datos con los que trabajar.

El método completo para contar estos costes y convertir los ahorros en una cifra de retorno está en el [Capítulo 16 — Objetivos, costes y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md). No hagas las cuentas de cabeza. Escríbelas.

## Los resultados

Tras un año, medido contra una línea base que Sara registró antes de empezar, el resultado ilustrativo tiene este aspecto. Tus números diferirán. Estos muestran a qué puede parecerse un buen ajuste.

- **Soporte desviado.** El chatbot manejó la mayoría de las preguntas de «dónde está mi pedido» y rutinarias, así que los fundadores pasaron mucho menos tiempo en la bandeja de entrada y más tiempo construyendo.
- **Contenido a escala.** Las páginas de producto del catálogo se rellenaron en semanas en lugar de meses, y la tienda se volvió más fácil de encontrar en las búsquedas.
- **La conversión mejoró.** Las recomendaciones y los correos dirigidos trajeron más ventas del mismo tráfico, porque las personas correctas vieron los productos correctos.
- **Menos fuegos.** Las excepciones de pedidos se señalaron pronto, así que los problemas se arreglaron antes de llegar al cliente.
- **El equipo se mantuvo pequeño.** Seis personas cubrieron trabajo que de otro modo habría necesitado muchos más, que es todo el sentido de una startup ágil.

La advertencia honesta: nada de esto fue instantáneo. El chatbot dio respuestas equivocadas al principio hasta que se conectó a datos de pedidos exactos. Los borradores de contenido necesitaron edición intensa hasta que el asistente aprendió la marca. Las recomendaciones fueron débiles hasta que hubo suficiente historial de navegación. Las ganancias se incrementaron durante semanas, como predice la advertencia de la curva de aprendizaje del [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). Sara midió los números reales después de la subida, no durante.

## Lecciones aprendidas

**El superpoder de un equipo pequeño es la palanca.** Lumen no contrató; apuntó herramientas a trabajos. Para una startup ágil, la IA no trata de reemplazar personas. Trata de dejar que unas pocas personas cubran más terreno. Ese es el uso de mayor valor de la IA cuando no tienes personal de sobra.

**El bot solo es tan bueno como los datos detrás de él.** Un chatbot de soporte puede responder «dónde está mi pedido» solo si lee los datos de pedidos reales y actuales. Un bot que adivina da respuestas equivocadas con seguridad y molesta a los clientes. Conéctalo a la fuente de verdad. La preparación de datos se trata en el [Capítulo 14 — Datos: la materia prima](ch14-data-the-raw-material.md).

**Nunca dejes que la IA invente una afirmación de producto.** Un asistente de contenido puede escribir una descripción que suene genial y sea falsa —un material que el producto no tiene, una característica que le falta—. Una afirmación falsa es un problema legal y un asesino de confianza. Un humano comprueba cada afirmación contra el producto real antes de que se publique. El problema de fiabilidad está en el [Capítulo 2 — IA explicada de forma simple](ch02-ai-explained-simply.md), y el deber de honestidad está en el [Capítulo 4 — IA ética: hacer lo correcto](ch04-ethical-ai-doing-the-right-thing.md).

**Mantén la voz de marca humana.** El asistente escribe rápido, pero no conoce el tono de tu marca. Lee y ajusta cada borrador. La máquina redacta; tú mantienes la voz.

**La personalización necesita consentimiento.** Las recomendaciones y los correos dirigidos usan datos personales —historial de navegación y compra—. Solo envía correos a gente que aceptó, y sigue las reglas del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md). Una personalización que ignora el consentimiento cambia una pequeña ganancia de ventas por un gran riesgo de confianza y legal.

**Vigila la factura por uso a medida que escalas.** Muchas herramientas amigables con startups cobran por mensaje, por producto, por correo. A pequeño volumen parece casi gratis. A gran volumen puede sorprenderte. Modela el coste al tamaño que esperas alcanzar, no solo al tamaño con el que empiezas.

**Mide con honestidad y espera la subida.** Registra la línea base antes de empezar. Juzga el proyecto después de la curva de aprendizaje, no durante. El método está en el [Capítulo 22 — Medir resultados y ROI](ch22-measuring-results-and-roi.md).

La lección de la startup ágil es la misma que la de cada sector, con una razón extra para moverse pronto: encuentra los trabajos que comen a tu pequeño equipo —soporte, contenido, personalización, operaciones—, deja que la IA responda, redacte, recomiende y señale, mantén un humano en la voz de marca y cada afirmación de producto, respeta el consentimiento, y mide con honestidad. Una tienda de seis personas puede hacer esto. Las herramientas están listas y son baratas para empezar. Lo único que falta es una mirada clara a a dónde van las horas del equipo.
