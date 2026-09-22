# Capítulo 31 — Un pequeño negocio de fabricación

*Este capítulo es un compuesto representativo. No es una empresa real. Combina los patrones comunes que vemos en pequeños talleres mecánicos y fabricantes que adoptan IA. Todos los números son ilustrativos —muestran la forma de la decisión, no una promesa—. Reemplázalos por los tuyos.*

## Contexto

Imagina un pequeño taller de mecanizado de precisión. Lo llamaremos **Northgate Machining**. Emplea a unas veinticinco personas. Fabrica piezas de metal a medida por encargo —piezas únicas y series cortas para otras fábricas—. Nada se queda en una estantería esperando a un comprador. Cada pieza empieza como una petición de un cliente.

El trabajo empieza con una **RFQ**, que significa «solicitud de presupuesto». Un cliente envía por correo un plano —normalmente un PDF con la forma de la pieza, sus medidas y el material del que debe hacerse—. El taller debe mirar ese plano, averiguar cuánto tardará cada paso de corte y acabado, sumar el coste del metal y del tiempo de máquina, y devolver un precio. Ese precio es el presupuesto. Si es demasiado alto, el cliente se va a otro sitio. Si es demasiado bajo, el taller gana el trabajo pero pierde dinero fabricándolo.

Dos presupuestadores experimentados hacen la mayor parte de esto. Llevan años haciéndolo. Pueden mirar un plano y saber más o menos cuánto cuesta. Pero «más o menos» está haciendo mucho trabajo en esa frase. El taller no tiene registro escrito de lo que los presupuestos pasados costaron realmente producir. El conocimiento vive en dos cabezas. Cuando esas dos personas están de vacaciones, presupuestar se ralentiza hasta casi pararse.

Detrás de los presupuestos está el resto del taller. El metal en bruto —barras, placas, varillas— se registra en una hoja de cálculo que se actualiza cuando alguien se acuerda. El control de calidad es una comprobación visual final a mano al terminar el trabajo. Los informes semanales para el dueño se teclean a mano desde tres hojas de cálculo distintas. Nada está conectado. Todo depende de que la gente recuerde escribir las cosas.

Este es un pequeño fabricante normal y sano. Es rentable. Está ocupado. Y está dejando dinero sobre la mesa en cuatro sitios: presupuestos, inventario, calidad e informes.

## El problema

La dueña, Elena, puede sentir los problemas pero no siempre verlos. Nombrémoslos llanamente.

**Presupuestar es lento e inconsistente.** Una pieza simple tarda una hora en presupuestarse. Una compleja tarda medio día. El promedio es de dos días desde que llega el correo hasta que sale el presupuesto. En esa ventana, el cliente ya ha preguntado a otros dos talleres. La velocidad importa. Peor, los dos presupuestadores valoran el mismo plano de forma distinta. Uno es cauteloso y pone precio alto. El otro es agresivo y pone precio bajo. A lo largo de un año, algunos trabajos se infravaloran en silencio. El taller los gana, los construye, y descubre más tarde que el tiempo de máquina costó más de lo que el precio cubría. Estas pérdidas son invisibles porque nadie compara el presupuesto con el coste real después.

**El inventario es adivinanza.** El taller compra metal en bruto cuando alguien nota que la estantería está baja. Demasiado a menudo, eso es demasiado tarde —un trabajo se retrasa porque la barra adecuada no está en stock—. Igual de a menudo, el taller compra demasiado, y material caro se queda meses, inmovilizando efectivo. La hoja de cálculo nunca está del todo bien. Nadie confía en ella, así que la gente vuelve a comprobar caminando hasta la estantería, lo que desperdicia tiempo.

**Los defectos de calidad se pillan demasiado tarde.** Una pieza mala a menudo se encuentra solo en la comprobación final, después de terminar todo el trabajo. Si el error se cometió en el primer corte, el taller puede haber hecho cincuenta piezas malas antes de darse cuenta. Eso es chatarra —material y tiempo de máquina tirados—. Pillar un defecto después de cincuenta piezas en lugar de después de una es cincuenta veces la pérdida.

**Los informes comen horas.** Cada viernes, alguien pasa tres o cuatro horas sacando números de las hojas de cálculo para construir un resumen para Elena. Ese tiempo es puro gasto general —no produce piezas ni gana clientes—.

Cada uno de estos es una pequeña fuga. Juntos, drenan dinero real y tiempo real. Si quieres ver cómo se clasifican estas cuatro actividades frente al resto de tu negocio, el método de impacto y esfuerzo del [Capítulo 12 — Dónde puede ayudar la IA a tu negocio](ch12-where-ai-can-help-your-business.md) es el lugar para puntuarlas.

## La solución

Elena no intenta «usar IA por todas partes». Elige las cuatro fugas y las ataca una a una, empezando por la más grande y fácil.

**Presupuestos más inteligentes.** En lugar de leer cada plano desde cero, el taller mete sus trabajos pasados en un sistema. Para cada trabajo pasado, ahora registra dos cosas que nunca vinculó antes: el presupuesto original y el coste real de producir. Con el tiempo esto se vuelve una biblioteca de referencia. Cuando llega un plano nuevo, un asistente de IA lee el PDF, saca las características clave —las dimensiones, las tolerancias (lo exacto que debe ser cada medida), el material, el número de piezas— y sugiere un precio basado en trabajos pasados similares. El presupuestador ya no empieza de una página en blanco. Empieza de un borrador y lo ajusta. La IA hace la primera pasada; el humano toma la decisión.

**Inventario que predice.** El taller conecta su hoja de cálculo de existencias a una simple herramienta de previsión. La herramienta mira lo rápido que se usa cada material y sugiere cuándo reponer y cuánto. No hace el pedido ella sola. Lanza una sugerencia: «Te quedarás sin esta barra de aluminio en nueve días; pide ahora». Una persona lo confirma. La adivinanza se vuelve un aviso.

**Comprobaciones de calidad en la máquina.** En lugar de comprobar solo al final, el taller pone una pequeña cámara en una máquina. Un sistema de visión por computador —IA que lee lo que ve una cámara— mira cada pieza conforme sale y señala cualquier cosa que parezca mal: una grieta, una dimensión equivocada, un agujero que falta. El operador ve la señal de inmediato y se detiene antes de hacer cincuenta copias malas. La comprobación humana final se queda; la cámara solo mueve la advertencia más pronto. (El tratamiento más profundo del control de calidad por visión y el mantenimiento predictivo está en el [Capítulo 29 — Operaciones y producción](ch29-operations-and-production.md).)

**Informes que se escriben solos.** Las hojas de cálculo se conectan a un asistente de informes. El viernes, en lugar de teclear, Elena recibe un resumen redactado: trabajos presupuestados, trabajos ganados, tasa de chatarra, niveles de existencias, efectivo inmovilizado. Lo lee y lo edita. Tres horas se vuelven quince minutos.

Observa el patrón en los cuatro. La IA nunca actúa sola. Lee, sugiere, señala y redacta. Un humano decide, confirma y aprueba. Es el mismo patrón de «el humano revisa el borrador de la máquina» que muestra el caso de Elanco en el [Capítulo 25 — Administración y finanzas](ch25-administration-and-finance.md). En un taller donde un número equivocado puede perder dinero real, esa regla no es opcional.

## Las herramientas

Nada de esto requirió un equipo de ingenieros. Las herramientas son estándar, dirigidas a pequeñas empresas.

- **Un asistente de lectura de documentos** que abre el plano en PDF y extrae dimensiones y características en un formulario estructurado. Es la misma clase de herramienta que lee facturas en el [Capítulo 25](ch25-administration-and-finance.md).
- **Un asistente de presupuestos** construido encima de eso, que compara las características extraídas con trabajos pasados y propone un precio. Puede ser una herramienta de bajo código acoplada a la hoja de cálculo de presupuestos existente del taller, conectada como se describe en el [Capítulo 19 — Conectar la IA a sistemas que ya usas](ch19-connecting-ai-to-systems-you-already-use.md).
- **Un complemento de previsión** para la hoja de cálculo de inventario o el sistema ERP (planificación de recursos empresariales) básico del taller. Muchas herramientas de inventario ahora incluyen una función de «sugerir una reposición».
- **Una cámara más una herramienta de inspección por visión por computador** en una máquina. Estas se venden como unidades pequeñas y autónomas para comprobaciones de calidad.
- **Un asistente de informes** que lee las hojas de cálculo conectadas y redacta el resumen semanal en lenguaje llano.

Cómo elegir entre estas sin ser engañado por demos brillantes está tratado en el [Capítulo 17 — Elegir herramientas sin ser engañado](ch17-choosing-tools-without-being-fooled.md). Una precaución específica de un taller mecánico: **los planos son confidenciales.** El plano de una pieza de un cliente es su propiedad intelectual. Antes de meter planos en cualquier herramienta en la nube, comprueba a dónde van los datos y quién puede verlos. Para algunos talleres, mantener la IA en sus propios ordenadores —autoalojamiento, explicado en el [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md)— es la opción más segura. Los riesgos de enviar archivos sensibles a servicios de terceros están en el [Capítulo 9 — Servicios de terceros e IA en la sombra](ch09-third-party-services-and-shadow-ai.md).

## Los costes

Aquí hay un presupuesto ilustrativo del primer año para un taller como Northgate. Estos son números inventados para mostrar la forma. Usa los tuyos.

**Costes directos.**
- Asistente de presupuestos y documentos: unos 9.000 € al año en suscripciones.
- Complemento de previsión: unos 3.000 € al año.
- Unidad de cámara e inspección por visión: unos 6.000 € de pago único, más 1.200 € al año.
- Asistente de informes: unos 2.400 € al año.
- Configuración e integración (ayuda externa para conectar las herramientas a las hojas de cálculo y la máquina): unos 10.000 € de pago único.
- Formación de los presupuestadores y operadores: unos 3.000 € de pago único.

Total del primer año: unos **34.600 €**. En años estables después, los costes de pago único desaparecen y las suscripciones recurrentes llegan a unos **15.600 €**.

**Costes indirectos.** Estos son los que la gente olvida.
- Los presupuestadores pasan horas aprendiendo la herramienta y comprobando sus borradores. Eso es tiempo real, valorado a su coste horario cargado.
- La caída de aprendizaje: durante las primeras semanas, presupuestar es más lento, no más rápido, mientras la gente confía en el nuevo sistema.
- La cámara de visión necesita recalibración ocasional cuando cambia la iluminación o la pieza.
- Alguien debe revisar los presupuestos sugeridos por la IA y los puntos de reposición cada día. Nunca te saltes esto.

El método completo para contar estos costes con honestidad, y para convertir los ahorros en una cifra de retorno, vive en el [Capítulo 16 — Objetivos, costes y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md). No hagas las cuentas de cabeza. Escríbelas.

## Los resultados

Tras un año, medido contra la línea base que Elena registró antes de empezar, el resultado ilustrativo tiene este aspecto. Recuerda: tus números diferirán. Estos muestran a qué puede parecerse un buen ajuste, no lo que será el tuyo.

- **El tiempo de presupuestar** cayó de un promedio de dos días a unas pocas horas para la mayoría de las piezas. El presupuestador revisa un borrador en lugar de construir desde cero.
- **Menos trabajos infravalorados.** Como el presupuesto está anclado a lo que los trabajos similares costaron realmente, la distancia entre precio presupuestado y coste real se estrechó. El taller dejó de perder dinero en silencio en trabajos que ganaba.
- **La tasa de victorias mejoró.** Presupuestos más rápidos significaron que Northgate respondió a más RFQ dentro de la ventana donde el cliente aún está eligiendo.
- **La chatarra bajó.** Pillar un defecto en la máquina en lugar de al final recortó material y tiempo de máquina desperdiciados. En lugar de cincuenta piezas malas, el operador lo pilló en la primera o segunda.
- **La rotación de existencias mejoró.** Menos roturas de stock significaron menos trabajos retrasados. Menos sobrecompra significó menos efectivo congelado en la estantería.
- **Los informes** pasaron de tres o cuatro horas de tecleo a unos quince minutos de lectura y edición.

La advertencia honesta: nada de esto ocurrió el primer día. El asistente de presupuestos fue tosco el primer mes porque la biblioteca de trabajos pasados era escasa. La cámara de visión dio falsas alarmas hasta que se calibró. Los ahorros se incrementaron durante semanas, exactamente como predice la advertencia de la curva de aprendizaje del [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). Elena midió los números reales después de la subida, no durante.

## Lecciones aprendidas

**Empieza con los presupuestos.** De las cuatro fugas, presupuestar fue el de mayor impacto y menor riesgo para probar. Un presupuesto equivocado lo pilla el presupuestador antes de que salga. Eso lo hizo el primer proyecto perfecto —la misma regla de «alto impacto, alta facilidad primero» del [Capítulo 12](ch12-where-ai-can-help-your-business.md)—.

**Tus trabajos pasados son el combustible.** El asistente de presupuestos solo era tan bueno como el registro de presupuestos pasados y sus costes reales. Lo más valioso que hizo Elena fue empezar a vincular cada presupuesto a su coste real de producción. Sin esos datos, la IA no tenía de qué aprender. La preparación de datos se trata en el [Capítulo 14 — Datos: la materia prima](ch14-data-the-raw-material.md).

**La IA redacta; el humano decide.** Ni un presupuesto salió sin que una persona lo aprobara. Ni un pedido de reposición se hizo sin que una persona lo confirmara. En un taller donde un número equivocado es dinero real, el control humano es la seguridad, no una demora.

**Los planos son confidenciales.** Trata cada plano de cliente como propiedad intelectual sensible. Decide a dónde puede ir antes de meterlo en ningún sitio. Para algunos talleres eso significa autoalojarse; para otros, un proveedor evaluado con un contrato claro.

**Calibra la cámara; no confíes en ella a ciegas.** El sistema de visión no fue enchufar-y-usar. Necesitó ajuste para distinguir un defecto real de una sombra. Presupuesta para eso, y mantén la comprobación humana final en su lugar.

**Espera la subida.** El primer mes fue más lento y desordenado que el duodécimo. Juzga el proyecto después de la curva de aprendizaje, no durante.

**Conecta, no reemplaces.** Northgate no tiró sus hojas de cálculo ni su ERP. Acopló la IA a lo que ya funcionaba, como se describe en el [Capítulo 19](ch19-connecting-ai-to-systems-you-already-use.md). El taller mantuvo sus sistemas y añadió una capa más inteligente encima.

La lección del pequeño fabricante es la misma que la de todos los demás sectores: encuentra la fuga, elige la de mayor valor y más fácil, deja que la IA redacte y señale, mantén un humano en la decisión, y mide con honestidad. Un taller con veinticinco personas y sin ingenieros puede hacer esto. Las herramientas están listas. Lo único que falta es una mirada clara a dónde se está fugando el dinero.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que tecleas para obtenerlo.

### Diseña una pieza simple

![Una pieza simple modelada con la herramienta CAD](../../assets/examples/part-design.png)
*Una pieza simple modelada con la herramienta CAD*

**Lo que pides:** `Diseña un pequeño soporte de metal de 80 por 40 milímetros con cuatro agujeros de montaje.`

El agente dirige la herramienta CAD para modelar la pieza con las dimensiones correctas, y obtienes un archivo que puedes revisar o exportar.

*Consejo: Describe la forma y las medidas; el agente maneja los pasos de CAD.*

---

### Comprueba cómo encajan las piezas

![Una comprobación de ensamblaje entre dos piezas](../../assets/examples/assembly-check.png)
*Una comprobación de ensamblaje entre dos piezas*

**Lo que pides:** `Coloca estas dos piezas juntas y comprueba si hay solapamiento o problemas de holgura.`

El agente ensambla las piezas en el modelo CAD y señala dónde chocan o dónde el ajuste es demasiado apretado.

*Consejo: Pilla los problemas de ajuste en pantalla, no en el banco del taller.*

---

### Un plano para el taller

![Un plano técnico acotado para producción](../../assets/examples/technical-drawing.png)
*Un plano técnico acotado para producción*

**Lo que pides:** `Produce un plano técnico del soporte con las dimensiones clave marcadas.`

El agente genera un plano con las dimensiones marcadas, listo para la persona que hará la pieza.

*Consejo: Pide la vista que necesitas —superior, lateral— para que el plano sea claro.*

<!-- END agentbridge-examples -->
