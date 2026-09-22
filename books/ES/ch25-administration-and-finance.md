# Capítulo 25 — Administración y finanzas

## En palabras simples

La administración y las finanzas son donde la IA ahorra más horas en silencio en un pequeño negocio. No porque el trabajo sea difícil, sino porque es repetitivo. Facturas, movimientos bancarios, notas de gastos, informes mensuales, previsiones de caja: las mismas tareas, una y otra vez, cada semana. La repetición es justo lo que se le bien al software, y la IA suma la capacidad de leer documentos desordenados y detectar patrones que una persona podría pasar por alto.

Imagina tu oficina trasera como una sala llena de papel que nunca deja de llegar. Cada factura es un papelito que alguien debe leer, escribir en un sistema, cruzar con un pedido, revisar si hay errores y archivar. Multiplica eso por cientos o miles de papeles al mes y verás a dónde se van los días. La IA no se cansa, no pierde la concentración a las cuatro de la tarde y no le molesta hacer la misma tarea por milésima vez.

Este capítulo cubre cuatro trabajos: leer facturas y documentos, cruzar (conciliar) registros, producir informes de forma automática y prever la caja. Cada uno es un lugar donde un pequeño negocio puede ahorrar tiempo real y cometer menos errores.

Una idea importante antes de empezar: la IA en finanzas es un *dibujante*, no el *que toma las decisiones*. Lee, ordena, cruza y sugiere. Una persona sigue aprobando el movimiento de dinero, firmando el informe y haciéndose responsable del resultado. Mantén a un humano en el ciclo para todo lo que toque dinero real. El método para juzgar si todo esto vale la pena está en el [Capítulo 16 — Metas, costos y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md); este capítulo te muestra qué automatizar y cómo.

## Un poco de historia

**Años 60–80: la revolución de la hoja de cálculo.** El primer gran cambio en el trabajo de oficina fue la hoja de cálculo electrónica. Antes, los contadores llevaban los libros a mano y un solo cambio podía significar horas de recálculo. Las hojas de cálculo hicieron el cálculo instantáneo. Fue la primera vez que el software se hizo cargo de una tarea central de finanzas, y marcó el patrón: automatiza la aritmética y deja al humano a cargo del significado.

**Años 90: OCR y escaneo de documentos.** El Reconocimiento Óptico de Caracteres —software que lee texto impreso desde una imagen escaneada y lo convierte en texto editable— llegó a las herramientas de negocio. De pronto, una factura en papel podía convertirse en datos en lugar de una pila de papel. El OCR temprano era lento y cometía errores, así que una persona aún revisaba todo. Pero la puerta estaba abierta: el papel podía volverse digital.

**Años 2000: automatización basada en reglas y RPA.** La Automatización Robótica de Procesos —«bots» de software que siguen reglas fijas para mover datos entre sistemas— se volvió popular. Un bot podía copiar el total de una factura de una pantalla y pegarlo en otra. Esto funcionaba en tareas predecibles, pero se rompía en cuanto un documento se veía distinto: rápido pero frágil.

**Años 2010: el aprendizaje automático lee documentos.** El aprendizaje automático —software que aprende patrones de muchos ejemplos en lugar de seguir reglas fijas— cambió la lectura de documentos. En vez de decirle al ordenador exactamente dónde mirar, le mostrabas miles de facturas, y aprendía a encontrar el proveedor, la fecha y el total por su cuenta, incluso cuando el diseño cambiaba.

**Años 2020: grandes modelos de lenguaje y agentes.** Los grandes modelos de lenguaje —IA entrenada con enormes cantidades de texto— ahora pueden leer una factura, entender qué dice y redactar una respuesta al proveedor. Manejan formatos inusuales que rompían las herramientas anteriores. El paso más nuevo es el *agente*: una IA que toma una tarea completa, como «procesar este correo de un proveedor», y la lleva a cabo en varios pasos por su cuenta, con un humano revisando el resultado. El ejemplo de Elanco más adelante en este capítulo es exactamente este tipo de agente.

El recorrido: de los libros escritos a mano, a las hojas de cálculo instantáneas, al texto escaneado, a los bots que siguen reglas, a una IA que lee y razona. Cada paso quitó más del trabajo repetitivo a las manos humanas y dejó a los humanos hacer el juicio.

## Curiosidad

### 25.5 El «intermediario humano» que la IA reemplazó

Durante años, el equipo de compra-a-pago de Elanco —las personas que gestionan las preguntas y el papeleo entre comprar mercancías y pagarlas— trabajó como lo que la empresa llamaba «intermediario humano». Respondían a mano más de 30.000 consultas al año, y cada una tomaba más de diez minutos. Diez minutos aquí, diez minutos allá, multiplicados por treinta mil, son una montaña de horas gastadas moviendo información entre sistemas a mano.

Esa historia, con los números reales y el sistema de IA de dos capas que lo reemplazó, se cuenta por completo en «Un ejemplo real de negocio» más abajo. La curiosidad aquí es la frase en sí: «intermediario humano». Describe un trabajo donde una persona existe solo para llevar datos de un lugar a otro. Ese es el tipo de trabajo que la IA mejor elimina, y el tipo que debes buscar en tu propia oficina trasera.

## Un ejemplo real de negocio

**Elanco: un ecosistema de IA de dos capas para compra-a-pago, que recorta el tiempo de consulta cerca de un 99%.**

Elanco es una empresa global de salud animal que fabrica medicamentos y tratamientos para mascotas y animales de granja. Su equipo de compra-a-pago —el grupo que gestiona todo entre pedir mercancías y pagar al proveedor— tenía un problema crónico. El equipo pasaba sus días como «intermediario humano», respondiendo a mano más de 30.000 consultas al año. Cada consulta tomaba más de diez minutos: alguien buscaba en el sistema financiero, revisaba el pedido, consultaba al proveedor y escribía una respuesta. El trabajo era lento, repetitivo y propenso a errores.

Según The Hackett Group, que nombró este proyecto ganador en la categoría Compra-a-Pago de sus Premios Hackett a la Innovación 2026 (anunciado en un comunicado de Business Wire el 24 de junio de 2026), Elanco lo resolvió con un ecosistema de IA de dos capas basado en agentes, construido sobre ElancoGPT, la plataforma de IA segura de la propia empresa. Las dos capas eran:

- **Capa uno — AskSAP.** Los empleados podían hacer preguntas en lenguaje sencillo y obtener respuestas extraídas del sistema empresarial SAP de la empresa (el software que gestiona sus finanzas y operaciones). En lugar de abrir varias pantallas y buscar un número, una persona solo preguntaba: «¿Cuál es el estado de esta orden de compra?» y recibía una respuesta.
- **Capa dos — el agente de compra-a-pago.** Este agente escanea automáticamente los correos entrantes de proveedores, determina qué quiere el proveedor (la «intención»), contrasta la solicitud con datos en vivo del sistema empresarial y redacta una respuesta. Luego un empleado humano revisa el borrador antes de enviarlo.

El resultado fue dramático. El tiempo de resolución de consultas bajó a **menos de 10 segundos** —lo que The Hackett Group describió como **una reducción del 99%** respecto a los más de diez minutos anteriores—. La empresa también informó que el sistema eliminó por completo entre un **30% y un 40%** de las consultas manuales de compra-a-pago, porque muchas preguntas simplemente dejaron de hacerse una vez que los empleados podían encontrar las respuestas por sí mismos a través de AskSAP.

Dos cosas vale la pena notar. Primera, el humano sigue ahí: el agente *redacta*, el empleado *revisa*. Elanco no dejó que la IA enviara dinero o respuestas por su cuenta. Segunda, la mayor ganancia vino de dar a las personas una forma más rápida de encontrar respuestas, lo que eliminó la necesidad de la consulta desde el principio. Ese es un patrón que puedes copiar: la mejor automatización a menudo elimina la solicitud, no solo el trabajo.

Una nota sobre la fuente: este es un caso de los Premios a la Innovación de Hackett, no una historia de cliente de Microsoft. Las cifras de arriba provienen del anuncio de premio de The Hackett Group. Toma los porcentajes como los resultados reportados por la empresa, y recuerda que tus propios números variarán según tus sistemas y tu volumen.

## Cómo hacerlo

### 25.1 Facturas y documentos

Leer facturas y otros documentos a mano es uno de los mayores sumideros de tiempo en un pequeño negocio. El procesamiento de documentos con IA puede leer una factura, extraer los campos clave y ponerlos donde corresponden.

**Lo que la IA extrae.** De una factura típica, el software saca el nombre del proveedor, el número de factura, la fecha, los conceptos de línea, el impuesto y el total. Lee PDF, papel escaneado y adjuntos de correo. Las herramientas modernas manejan muchos diseños sin que le indiquen cada uno de antemano.

**Cómo funciona en la práctica.** Apuntas la herramienta a una carpeta de facturas entrantes, o la conectas a tu correo. Lee cada una, extrae los campos y los introduce en tu sistema contable o los pone en una cola para que una persona los confirme. Cuantas más facturas ve, mejor se vuelve con tus proveedores específicos.

**La revisión humana.** No dejes que la herramienta registre facturas en tus libros sin revisión, al menos al principio. Configúrala para extraer y marcar, y que una persona apruebe. Observa la tasa de error (como aconseja el Capítulo 22). Con el tiempo, cuando la precisión se demuestre, puedes dejar que las facturas rutinarias y de bajo valor se registren automáticamente y enviar solo las inusuales a un humano.

**Dónde más ahorra.** Alto volumen y formatos repetitivos. Si procesas cientos de facturas al mes, el ahorro es grande y evidente. Si procesas diez, puede que la herramienta no se pague sola. Ajusta la herramienta a tu volumen.

**Vigila los campos de alto riesgo.** El total y el impuesto son los dos campos que deben estar bien, porque un número equivocado aquí cuesta dinero real. Revisa estos dos hasta que confíes en la herramienta; el nombre del proveedor y la fecha son de menor riesgo si fallan.

### 25.2 Conciliaciones

Conciliar significa cruzar dos conjuntos de registros para asegurarse de que coincidan. El ejemplo clásico es cruzar tu extracto bancario contra tu libro contable. Si coinciden, tus libros son correctos. Si no, algo falta, está duplicado o está mal, y debes encontrarlo.

**Por qué es doloroso a mano.** Cruzar línea por línea es lento y aburrido, y el aburrimiento causa errores. Una persona que revisa cientos de líneas bancarias terminará por pasar por alto un pago duplicado o un recibo que falta.

**Cómo ayuda la IA.** Las herramientas de conciliación con IA cruzan registros automáticamente comparando importes, fechas y números de referencia. Vinculan una línea bancaria con la factura que coincide, marcan las que encajan limpiamente y muestran solo los desacuerdos para que un humano los investigue. En lugar de revisar todo, revisas las excepciones.

**El modelo de excepciones.** Esta es la idea clave: deja que el software maneje el 95% que coincide y trae a una persona el 5% que no. El trabajo de la persona cambia de «cruzar cada línea» a «resolver las pocas que no coinciden». Ese es un trabajo más pequeño y más interesante, y es donde el juicio humano realmente aporta valor.

**Desacuerdos comunes que esperar.** Un pago que aparece dos veces (un duplicado), una comisión bancaria que nadie registró, un recibo que falta de un pago con tarjeta, un pago hecho al proveedor equivocado. La herramienta los marca; tú los resuelves. Con el tiempo aprendes tus propios patrones y puedes añadir reglas para atrapar los recurrentes automáticamente.

**Mantén un rastro de auditoría.** Sea lo que sea que haga la herramienta, asegúrate de que registre lo que cruzó y lo que marcó. Cuando tu contador o un auditor pregunte cómo se llegó a una cifra, necesitas un rastro claro. Las buenas herramientas producen esto; pregunta antes de comprar.

### 25.3 Informes automáticos

Los informes mensuales y semanales —pérdidas y ganancias, ventas por producto, gastos por categoría— son otro lugar donde la IA ahorra horas. En lugar de que una persona saque números a una hoja de cálculo cada mes, el informe puede construirse solo.

**Informes programados.** Configura el informe para que se genere en un horario fijo (cada lunes, el primero de mes) y lo entregue en tu bandeja de entrada o en una carpeta compartida. Los números se extraen de tus sistemas en vivo, así que el informe siempre está actualizado. Nadie tiene que acordarse de hacerlo.

**Resúmenes en lenguaje sencillo.** La IA moderna puede leer los números y escribir un resumen corto en palabras simples: «Los ingresos subieron un 8% este mes, impulsados por el producto X; los gastos subieron un 3%, sobre todo en envíos». Esto convierte una tabla de cifras en una frase que realmente puedes leer y sobre la que puedes actuar. Es como tener un analista junior que escriba los comentarios por ti.

**Haz preguntas en lenguaje sencillo.** Algunas herramientas te permiten preguntar «¿Cuáles fueron nuestros cinco mejores clientes este trimestre?» y obtener una respuesta sin escribir una fórmula. Esto es útil para las preguntas puntuales que antes significaban «lo miro más tarde» y luego nunca sucedían.

**No te saltes la lectura humana.** Un informe automático es un punto de partida, no un documento de decisión terminado. Lee el resumen, comprueba que los números tengan sentido y añade tu propio juicio antes de actuar sobre él o compartirlo. La IA puede resumir con confianza y aun así estar equivocada si los datos de base están desordenados. Basura entra, basura con confianza sale.

**Estandariza el formato.** Una vez que te decidas por un diseño de informe, mantenlo estable. Un formato consistente es más fácil de leer mes a mes y más fácil para notar cuando algo se ve raro. Cambia el formato solo de forma deliberada, no cada vez.

### 25.4 Previsiones de flujo de caja

Prever el flujo de caja significa predecir cuánto dinero habrá en el banco en las próximas semanas y meses. Es distinto de la ganancia. Un negocio puede ser rentable sobre el papel y aun así quedarse sin caja si los pagos llegan tarde. La caja es oxígeno; la ganancia es comida. Puedes sobrevivir mucho tiempo sin comida y solo minutos sin oxígeno.

**Por qué ayuda la IA.** Una buena previsión necesita combinar muchas señales: facturas que has enviado pero no cobrado, cuentas que debes, patrones estacionales y qué tan confiablemente tus clientes pagan realmente a tiempo. La IA puede mirar tu historial y aprender, por ejemplo, que el cliente A suele pagar dos semanas tarde, mientras que el cliente B paga temprano. Luego pondera la previsión en consecuencia.

**Empieza por lo básico.** Una previsión simple responde: qué caja entra, qué sale y cuál es el saldo, semana a semana para las próximas 8 a 13 semanas. Construye esto incluso sin IA; una hoja de cálculo funciona. La IA lo mejora aprendiendo patrones de pago y marcando el riesgo.

**Vigila el hueco.** El número más importante es el punto más bajo de la previsión. Si la previsión muestra que tu saldo cae por debajo de un nivel seguro en la semana nueve, tienes tiempo ahora para arreglarlo: persigue facturas, retrasa una compra, consigue una línea de crédito. Todo el valor de prever es ver el descenso antes de que ocurra.

**Trata las previsiones como rangos, no como promesas, y actualízalas a menudo.** Una previsión es una estimación, no una garantía. Preséntala como un rango probable con un mejor caso y un peor caso, y planifica para que el peor caso sea sobrevivible. Las previsiones de caja se quedan obsoletas rápido, así que actualízalas cada semana; una previsión de hace un mes es casi inútil porque ha cambiado mucho. El hábito de una revisión semanal de caja es una de las rutinas más valiosas que un dueño de un pequeño negocio puede crear.

## Ética y responsabilidad

Las finanzas son donde los errores cuestan dinero real y confianza real, así que la responsabilidad importa aquí más que en casi cualquier otro lugar.

**Mantén un humano en el ciclo para el movimiento de dinero.** La IA debe redactar, extraer, cruzar y sugerir. Una persona debe aprobar todo lo que envíe dinero, cambie un saldo o firme un informe. Un agente que lee un correo de un proveedor y paga sin revisión es un riesgo de fraude: una factura falsa, un correo suplantado o un total mal leído pueden vaciar la caja rápido. El agente de Elanco redacta y un humano revisa; copia ese patrón exactamente.

**Protege los datos financieros.** Las facturas y los registros bancarios son sensibles. Usa herramientas que mantengan tus datos seguros y, donde sea posible, dentro de tu propio entorno. Ten cuidado al enviar documentos financieros a servicios de IA públicos. Los conceptos básicos de seguridad se cubren en el [Capítulo 6 — Ciberseguridad en la era de la IA](ch06-cybersecurity-in-the-ai-era.md) y la opción de autoalojamiento en el [Capítulo 8 — Autoalojamiento: mantén tus datos bajo control](ch08-self-hosting-keep-your-data-under-control.md).

**Sé honesto en los informes.** Un resumen automático puede hacer que un mal mes suene bien. No dejes que el pulido de un informe escrito por IA esconda un problema real. Lee los números tú mismo y reporta la verdad, sobre todo cuando es incómoda.

**Cuida el rastro de auditoría y mantén la segregación de funciones.** Guarda registros de lo que la IA extrajo, cruzó y cambió; si un auditor pregunta cómo se produjo una cifra, debes poder mostrar el camino. Y recuerda que la automatización puede esconder una mala transacción tan fácilmente como encontrarla: la persona que configura un proveedor no debe ser la misma que aprueba su pago. La IA no elimina la necesidad de controles internos; cambia cómo se ven.

## Errores a evitar

**Dejar que la IA mueva dinero sin revisión.** El error más peligroso de todos. Exige siempre aprobación humana para los pagos.

**Automatizar un mal proceso.** Si tu proceso actual de facturas es un desastre, automatizarlo solo crea un desastre más rápido. Limpia el proceso primero, luego automatiza.

**Confiar en la extracción a ciegas.** La IA puede leer mal un total o una cifra de impuesto. Revisa los campos de alto riesgo hasta que tengas prueba de precisión.

**Sin manejo de excepciones.** Si solo automatizas los casos fáciles y no tienes plan para los inusuales, los inusuales se acumulan y rompen el sistema. Diseña para las excepciones desde el primer día.

**Saltarse el rastro de auditoría.** Una herramienta que no puede mostrar lo que hizo es un pasivo en una auditoría. Exige trazabilidad.

**Prever el mejor caso y apostar por él.** Una previsión es un rango. Planifica para que el peor caso sea sobrevivible.

**Previsiones obsoletas y confusión entre ganancia y caja.** Una previsión de caja de hace un mes es inútil; actualízala cada semana. Y recuerda que puedes ser rentable y aun así quedarte sin dinero: prevé la caja, no solo la ganancia.

**Sobreautomatizar bajo volumen.** Si solo tienes diez facturas al mes, puede que una herramienta no compense. Ajusta la herramienta a tu volumen.

**Enviar datos sensibles a IA pública.** Las facturas y las líneas bancarias son sensibles. Usa herramientas seguras o autoalojadas.

**Sin línea base.** No medir cuánto tardaba la tarea antes, así que no puedes probar el ahorro. Mide antes de empezar (ver Capítulo 22).

**Esconder malas cifras.** Un informe pulido de IA que enmascara un mal mes es deshonesto. Reporta la verdad.

## Ejercicio práctico

### 25.7 Ejercicio: mapea la automatización de tu oficina trasera

Elige una tarea de la oficina trasera y planifica su automatización de principio a fin.

**Paso 1 — Elige la tarea.** Escoge la tarea de finanzas o administración más repetitiva que tengas: captura de facturas, conciliación bancaria, el informe mensual o la previsión de caja.

**Paso 2 — Mide la línea base.** ¿Cuánto tiempo toma ahora y cuántas veces al mes la haces? Anota ambas cosas. Este es tu número «antes».

**Paso 3 — Dibuja los pasos actuales.** Lista cada paso que un humano hace hoy: recibir, leer, escribir, cruzar, revisar, archivar. Ver los pasos hace la automatización obvia.

**Paso 4 — Marca cada paso.** Para cada paso, márcalo: **la IA lo hace** (extraer, cruzar, resumir), **el humano lo revisa** (aprobar, firmar) o **el humano lo decide** (la decisión de juicio). Cada movimiento de dinero debe ser aprobado por un humano.

**Paso 5 — Elige la herramienta.** Escoge una herramienta que encaje con tu volumen y tu sistema contable. No compres la más grande; compra la que encaje.

**Paso 6 — Empieza con extraer y marcar.** Lanza con la IA extrayendo y marcando, y un humano aprobando todo. No pases a totalmente automático el primer día.

**Paso 7 — Fija el umbral de error.** Decide la tasa de error que dispara una acción. Por ejemplo, «si más del 3% de los totales extraídos están mal, nos detenemos y revisamos la herramienta».

**Paso 8 — Planifica la previsión de caja.** Construye una previsión de caja simple de 8 a 13 semanas, incluso en una hoja de cálculo. Marca el punto más bajo. Decide qué harás si cae por debajo de tu nivel seguro.

Haz esto primero con una tarea. Una vez que funcione y los números prueben el ahorro, pasa a la siguiente tarea. Una tarea bien automatizada te enseña más que cinco a medio terminar.

## Lista de verificación

### 25.8 Lista de verificación de administración y finanzas

Antes de automatizar cualquier tarea de finanzas, revisa esto.

- [ ] **Mediste la línea base** — tiempo por tarea y con qué frecuencia la haces.
- [ ] **Un humano aprueba cada movimiento de dinero** — ninguna IA envía dinero por su cuenta.
- [ ] **Limpia el proceso antes de automatizarlo.**
- [ ] **Revisas los campos de alto riesgo** (totales, impuesto) hasta que confíes en la herramienta.
- [ ] **Diseñaste para las excepciones** — los casos inusuales tienen un camino claro hacia un humano.
- [ ] **La herramienta mantiene un rastro de auditoría** que puedas mostrar a un contador o auditor.
- [ ] **Los datos financieros se mantienen seguros**, no enviados a servicios de IA públicos.
- [ ] **Los informes los lee un humano** antes de que actúes sobre ellos o los compartas.
- [ ] **Reportas las malas cifras con honestidad**, no solo el resumen pulido.
- [ ] **Mantienes la segregación de funciones** — la configuración de proveedores y la aprobación de pagos son personas separadas.
- [ ] **Prevés la caja, no solo la ganancia**, y vigilas el punto más bajo.
- [ ] **Actualizas la previsión de caja cada semana.**
- [ ] **Tratas las previsiones como un rango**, y planificas para que el peor caso sea sobrevivible.
- [ ] **Ajustas la herramienta a tu volumen** — nada de sobreautomatizar tareas diminutas.
- [ ] **Fijaste un umbral de error** que dispara una revisión.
- [ ] **Mantienes la decisión de dinero separada de la decisión de personas** (ver Capítulo 16).

Si una casilla está vacía, el riesgo sigue siendo tuyo. Llénala antes de dejar que la IA se acerque al dinero.

## Puntos clave

- La administración y las finanzas están llenas de trabajo repetitivo —facturas, cruces, informes, previsiones—, y la repetición es justo lo que se le bien a la IA.
- Mantén a la IA como el dibujante y al humano como el que toma las decisiones: deja que extraiga, cruce y sugiera, pero una persona debe aprobar todo lo que mueva dinero.
- El caso de Elanco (ganador de un Premio a la Innovación de Hackett 2026) recortó el tiempo de consulta de compra-a-pago a menos de 10 segundos, cerca de un 99% de reducción, usando un agente de dos capas que redacta respuestas para revisión humana y elimina muchas consultas por completo.
- Prevés la caja, no solo la ganancia, actualízala cada semana y planifica para que el descenso del peor caso sea sobrevivible.
- Limpia el proceso antes de automatizarlo, diseña para las excepciones y mantén un rastro de auditoría que puedas mostrar.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Haz una factura en segundos

![Un documento de factura terminado producido por el agente](../../assets/examples/client-invoice.png)
*Un documento de factura terminado producido por el agente*

**Lo que pides:** `Haz una factura para Bright Cafe por 12 horas de contabilidad a 45 euros la hora, con vencimiento en 14 días.`

El agente escribe una factura formal con los datos de tu negocio, los conceptos de línea, el subtotal, el impuesto y el total, y una fecha de vencimiento. Obtienes un documento real que puedes imprimir o enviar. Si un número está mal, lo dices y lo corrige.

*Consejo: Pídela como un archivo Word real (/tools office-files) si quieres seguir editándola en Microsoft Office.*

---

### Escribe una carta formal

![Una carta comercial formal, con formato y lista](../../assets/examples/business-letter.png)
*Una carta comercial formal, con formato y lista*

**Lo que pides:** `Escribe una carta formal a nuestro arrendador pidiendo renovar el contrato por otros dos años en las mismas condiciones.`

El agente escribe la carta con el saludo adecuado, un cuerpo claro y un cierre cortés, en la voz de tu negocio. La revisas, cambias una palabra si quieres, y la envías.

*Consejo: Dile a quién escribes y qué quieres; él se encarga del tono formal por ti.*

---

### Un presupuesto que puedes leer

![Una hoja de cálculo de presupuesto con un gráfico de barras claro](../../assets/examples/monthly-budget.png)
*Una hoja de cálculo de presupuesto con un gráfico de barras claro*

**Lo que pides:** `Crea una hoja de cálculo de presupuesto mensual con lo planificado y lo real para alquiler, marketing y salarios, más un gráfico.`

El agente crea la hoja de cálculo con las categorías, las columnas de planificado y real, los totales y un gráfico que muestra la diferencia de un vistazo. Puedes abrirla en Excel y seguir trabajando.

*Consejo: Pide el título del gráfico y la moneda para que coincida con tu negocio.*

---

### Envía la factura por correo

![La factura adjunta a un correo listo para enviar](../../assets/examples/invoice-email.png)
*La factura adjunta a un correo listo para enviar*

**Lo que pides:** `Envía por correo la factura que acabamos de hacer al cliente con una nota de presentación breve y amable.`

El agente adjunta la factura y escribe una breve nota de presentación con el importe y la fecha de vencimiento. Un mensaje, enviado.

*Consejo: Encadena: «haz la factura y envíala por correo al cliente» en una sola petición.*

<!-- END agentbridge-examples -->
