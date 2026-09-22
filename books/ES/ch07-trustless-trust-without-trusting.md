# Capítulo 7 — Trustless: confiar sin tener que fiarse

## En palabras simples

La palabra "trustless" está mal elegida. Suena a un mundo sin confianza, donde nadie cree nada. No es eso lo que significa, y la idea real es mucho más útil.

Trustless significa: **no tienes que fiarte de una persona o de una institución, porque puedes verificar el hecho tú mismo.**

Empieza con un contraste familiar. Contratas una empresa de mudanzas. Das una señal. Ahora dependes de que se presenten. Debes fiarte de ellos, o de su marca, o de que la ley los castigue si no lo hacen. Ahora piensa en una máquina expendedora. Metes monedas, la bebida cae. No hay relación, ni promesa, ni necesidad de creer a nadie. La máquina hace cumplir el trato por cómo está construida. Esa es la sensación de trustless: el acuerdo lo hace cumplir un sistema en vez de las buenas intenciones de una persona.

Tres herramientas hacen esto posible.

**Verificación en lugar de promesas.** En vez de que alguien te diga que algo es verdad, lo compruebas. Una firma digital es el ejemplo común. Prueba que un archivo vino de quien tiene cierta clave, y que el archivo no ha cambiado desde que se firmó. No necesitas fiarte del remitente. Compruebas la firma.

**Transparencia en lugar de secreto.** En vez de guardar un registro en un cuaderno privado, lo guardas en algún sitio que muchas personas pueden leer y nadie puede reescribir en silencio. Si todos pueden ver el registro, una parte no puede cambiar la historia para su conveniencia.

**Aplicación automática en lugar de esperanza.** En vez de acordar condiciones y esperar que se cumplan, escribes las condiciones para que un programa las lleve a cabo. El dinero se libera cuando se cumple la condición. Nadie tiene que perseguir una factura.

Ahora la advertencia honesta, dicha pronto: trustless no significa libre de riesgo. Has movido tu confianza de las personas a los sistemas, y los sistemas los construyen personas. El código tiene errores. Los datos que dicen a un sistema qué pasó en el mundo real pueden estar mal o ser mentira. Las claves se pierden, y una clave perdida puede significar dinero perdido. El objetivo no es eliminar la confianza. Es colocar la confianza en un sitio que puedas inspeccionar, y reducir cuánta necesitas.

¿Por qué molestarse? Porque la confianza es cara. Cada intermediario en el que te apoyas —un banco, un agente de depósito en garantía, un corredor, un notario, una plataforma que retiene fondos hasta que el trabajo está hecho— se lleva una comisión y se lleva tiempo. Los sistemas trustless eliminan parte de eso, y hacen lo que queda más barato, más rápido y visible. Esto no es solo para bancos y programadores; tiene uso directo en cualquier empresa que compra a proveedores, contrata freelancers y necesita registros en los que su contable pueda confiar.

La pregunta más amplia de quién controla tus herramientas digitales está en el [Capítulo 11](ch11-digital-sovereignty.md). Si se recupera la inversión es una pregunta del [Capítulo 16](ch16-goals-costs-and-return-on-investment.md). El lado de seguridad de la verificación está en el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).

## Un poco de historia

**2008.** En octubre se publicó un paper titulado "Bitcoin: un sistema de efectivo electrónico entre pares" bajo el nombre de Satoshi Nakamoto. Su objetivo declarado era el pago electrónico sin terceros de confianza. El truco era un registro compartido y ordenado —una blockchain— mantenido junto por muchas computadoras independientes, de modo que ninguna de ellas pueda reescribirlo.

**2009.** La red Bitcoin empezó a funcionar en enero. Por primera vez, dos desconocidos podían saldar valor sin un banco en medio, y ninguno tenía que fiarse del otro.

**2015.** Llegó Ethereum y añadió la mejora clave: los contratos inteligentes. Un contrato inteligente es un programa almacenado en la red que se ejecuta exactamente como está escrito cuando se cumplen sus condiciones. El dinero ahora podía atarse a una regla.

**2016.** Un proyecto llamado The DAO guardaba fondos en un contrato inteligente y fue vaciado por un fallo en ese contrato. Las consecuencias dividieron a la comunidad. La lección fue tajante y sigue siendo cierta: la aplicación automática aplica los bugs con la misma lealtad con que aplica las funciones.

**2017 a 2021.** Las finanzas descentralizadas crecieron hasta ser un sector real: préstamos, comercio y liquidación gestionados por contratos en vez de bancos, con stablecoins —tokens pensados para mantener un valor estable— como su dinero de trabajo. También mostraron los mismos fallos a mayor escala: mal código, datos de precio erróneos, operadores deshonestos. En **2019** el W3C, el organismo que fija los estándares web, publicó las Credenciales Verificables: una forma de que una autoridad emita una afirmación digital —un título, una licencia, una prueba de edad— que cualquiera puede comprobar sin telefonear al emisor. Esa es la mitad de identidad del cuadro.

**2021 a 2023.** Se propuso en 2021 y luego se finalizó un estándar llamado ERC-4337, conocido como abstracción de cuenta. Permite que una cuenta sea un pequeño programa en vez de una sola clave privada, así que la cuenta puede tener sus propias reglas: límites de gasto, una lista de beneficiarios permitidos, una segunda firma para importes grandes, y recuperación si se pierde una clave.

**Mayo de 2025.** Una mejora de Ethereum llamada Pectra entró en vivo en la red principal. Permitió que una dirección de billetera corriente apuntara a código de contrato inteligente, llevando la agrupación de transacciones, comisiones patrocinadas y mejor recuperación a direcciones que antes no tenían nada de eso. También elevó el máximo que un solo validador puede apostar.

**Agosto de 2025.** Apareció un borrador de estándar llamado ERC-8004, titulado "Trustless Agents" (Agentes sin confianza). Fue escrito para el problema del que trata realmente este capítulo: agentes de software que tratan con los agentes de otras personas.

Lee la cronología como un largo argumento. Cada paso movió la aplicación de las manos de una persona a un sistema comprobable: primero el dinero, luego los acuerdos, luego la identidad, luego los permisos, y más recientemente los agentes.

## Curiosidad

### 7.6 Ethereum está construyendo la fontanería de una economía de agentes

En agosto de 2025 se publicó un borrador de estándar llamado **ERC-8004** en el sitio oficial de estándares de Ethereum. Su título es "Trustless Agents", y su propósito declarado es permitir que agentes de software descubran, elijan y trabajen con otros agentes a través de fronteras organizacionales sin confianza previa.

Define tres registros, todos en la cadena.

**Identidad.** Cada agente recibe un identificador en cadena, construido sobre el estándar común de tokens ERC-721, que apunta a un archivo de registro. Ese archivo guarda los metadatos del agente, las direcciones con las que puedes hablar, y qué modelos de confianza admite. En términos simples: un agente puede decir quién es, a quién representa y cómo puedes comprobarlo, y tú puedes buscarlo en vez de creerle.

**Reputación.** Una forma estándar de publicar y leer comentarios sobre un agente, para que el historial de desempeño no quede encerrado en la valoración privada de una sola plataforma. Cualquiera puede aportar señales, y la agregación puede hacerse fuera de la cadena. El punto es la portabilidad: el registro de un agente lo sigue, en vez de reiniciarse cada vez que cambia de mercado.

**Validación.** Enganches para obtener una comprobación independiente del trabajo de un agente. El estándar lista varios métodos: que otra parte vuelva a ejecutar el trabajo con dinero en juego, usar pruebas de aprendizaje automático de conocimiento cero —una forma de probar que un cálculo se hizo correctamente sin revelar los datos ni el modelo detrás—, usar enclaves de hardware confiables, o usar un juez humano de confianza.

¿Por qué debería importarle a un pequeño dueño de negocio un borrador de estándar? Muestra dónde cree la industria que está el problema difícil: no "¿puede un agente hacer la tarea" sino "¿cómo sé si creer a este agente" —una pregunta de negocio, no técnica. Si tiene éxito, podrás consultar un registro público en vez de fiarte de una presentación de ventas, lo que cambia quién tiene el poder en la conversación. Y las mismas tres preguntas son una lista de verificación útil hoy, sin ninguna blockchain: *¿Quién eres, y a quién representas? ¿Cómo te has comportado antes? ¿Puede comprobarse tu trabajo de forma independiente?*

Dos piezas más de la misma fontanería ya están operativas. La abstracción de cuenta, el estándar ERC-4337, significa que un agente puede tener un presupuesto con reglas impuestas por código: un tope duro de gasto, una lista blanca de beneficiarios permitidos, una segunda firma humana por encima de un umbral. Y desde la mejora Pectra en mayo de 2025, una dirección corriente puede apuntar a ese código. Esa combinación —un agente que puede pagar, dentro de una caja que no puede abandonar— es la forma práctica de una economía trustless de agentes.

Toma todo esto como dirección, no como un producto para comprar este trimestre. El ERC-8004 es un borrador. Los conceptos, en cambio, son utilizables ahora.

## Un ejemplo real de negocio

### El mango que tardó siete días en rastrearse, y luego dos segundos

En 2017 Walmart e IBM hicieron una prueba piloto en cadenas de suministro de alimentos, y las cifras que publicaron se hicieron famosas en la industria. Rastrear el origen de un mango obtenido en Centro o Sudamérica solía tomar unos siete días de llamadas, correos y persecución de papel. Con los registros guardados en un libro compartido, el mismo rastreo tomó unos 2,2 segundos. IBM lo describió como trazabilidad completa de extremo a extremo. Una prueba paralela rastreaba cerdo en China.

Dos notas honestas. La cifra vino de una prueba controlada, no de un despliegue completo en vivo, y los 2,2 segundos son el tiempo de consultar el registro, no el tiempo de arreglar un envío contaminado.

Ahora mira qué cambió. Antes, cada parte guardaba su propio cuaderno: la granja escribía la fecha de cosecha, el envasador el lote, el transportista el contenedor, la tienda la entrega. Para responder una pregunta tenías que pedir a cuatro empresas que buscaran en sus cuadernos privados y esperar que respondieran rápido y con honestidad. Después, todos escribían en el mismo registro a medida que avanzaban. Nadie podía reescribir en silencio su página, y "¿de dónde vino esto?" se convirtió en una consulta en vez de una negociación.

Ese es el valor trustless en una frase: **reemplazaste una cadena de promesas por un registro compartido que puedes leer.**

También muestra el límite, que importa más que la victoria. Un registro compartido prueba lo que se anotó. No prueba que la anotación fuera verdad. Si un proveedor introduce una granja falsa o una fecha falsa, el libro conserva la mentira a la perfección. El eslabón débil es el momento en que un humano o un sensor pone un hecho en el sistema. Cualquier proyecto trustless que ignore ese momento es decoración.

## Cómo hacerlo

### 7.3 Cómo funciona en la práctica: identidad verificable, reputación, pagos programables

No necesitas una criptomoneda para usar el pensamiento trustless. Cuatro bloques de construcción se aplican al negocio corriente.

**Bloque 1: Identidad verificable.**
La pregunta es: ¿es realmente quien dice ser, y puedo comprobarlo sin telefonear a nadie? Los certificados digitales y las firmas digitales ya responden esto por ti cada día. Cuando un proveedor envía un documento firmado con una firma digital reconocida, puedes verificar tanto quién lo firmó como que nada cambió después. Una credencial verificable va más allá: tu contable puede probar que tiene una licencia vigente, o un empleado puede probar que pasó una comprobación de antecedentes, sin entregar todo el certificado y sin que tú llames al organismo emisor.

**Bloque 2: Registros a prueba de manipulaciones.**
La pregunta es: ¿puede alguien reescribir la historia en silencio? Un libro compartido es una respuesta. También lo es un truco más simple llamado hash —una huella corta calculada a partir de un archivo. Si registras la huella de un documento en el momento en que lo acuerdas, y el archivo se cambia después, la huella no coincidirá. Puedes producir esa huella más tarde y probar el estado del documento entonces. Esto no cuesta casi nada y no necesita permiso especial.

**Bloque 3: Pagos programables.**
La pregunta es: ¿puede el dinero moverse solo cuando se cumple la condición? El depósito en garantía (escrow) es la versión antigua: un tercero retiene fondos y los libera con un disparador. La versión nueva escribe el disparador en código, así que no se necesita una decisión humana en el momento de liberar. El pago por hitos para un freelancer es el caso obvio: el pago se libera cuando se acepta el entregable, y la regla de aceptación se escribe de antemano.

**Bloque 4: Auditabilidad.**
La pregunta es: después de los hechos, ¿podemos ver ambos la misma verdad? Cada acción debe dejar un registro con marca de tiempo, ordenado y no editable. Cuando ambas partes leen el mismo registro, las discusiones se acortan. Tu contable, tu auditor y tu cliente pueden todos comprobar lo mismo sin pedirte un favor.

**Cómo empezar en pequeño, hoy:**

1. Elige un proceso donde ahora persigues confirmaciones.
2. Escribe la condición de liberación como una sola frase comprobable. Si no puedes escribirla como frase comprobable, el proceso no está listo.
3. Pregúntate si una máquina puede medir el disparador. Entregado significa una nota de entrega firmida escaneada. Aprobado significa un clic en un botón de aprobación. Completado significa un cambio de estado en tu propio sistema.
4. Pon el dinero detrás de una regla que espere esa medición: un servicio de depósito en garantía, un calendario de pagos en tu sistema contable, o un flujo de trabajo que requiera el disparador antes de liberar.
5. Registra cada paso donde ambas partes puedan verlo.
6. Solo entonces automatiza.

### 7.4 Agentes de IA interactuando entre sí: el futuro del negocio automatizado

La versión interesante de esto está cerca. Tu agente de software habla con el agente de software de un proveedor, y saldan una transacción sin un humano en cada paso.

Para que eso funcione de forma segura, deben existir cinco cosas.

**Identidad y autoridad.** No solo "este es el agente del proveedor X", sino "este agente está autorizado a comprometer hasta 500 unidades a un precio inferior a 4,20 cada una". La autoridad debe ser demostrable y acotada, no supuesta.

**Un acuerdo legible por máquina.** Ambos lados necesitan los términos en una forma estructurada —cantidad, precio, fecha de entrega, penalización—, no un hilo de correos amigable. Un humano puede perdonar la ambigüedad. Un sistema automatizado se atascará en ella o la explotará.

**Una vía de pago que pueda esperar.** El pago debe ser condicional: retenido, luego liberado con evidencia. Un pago instantáneo e incondicional elimina todo apalancamiento y toda razón para cumplir.

**Evidencia.** Una confirmación de entrega, un registro de aceptación, un recibo firmado, en una forma que ambos sistemas puedan leer y ninguno pueda alterar en silencio.

**Una vía de disputa.** Algo debe manejar el caso en que los dos agentes no estén de acuerdo, o en que el mundo no fue como la regla asumía. Sin una ruta de escalada, un pequeño desacuerdo se convierte en un pago atascado y un proveedor enfadado.

Qué es realista ahora: los agentes ya pueden buscar, comparar, redactar cotizaciones y preparar pedidos. Lo que aún no es rutinario es dejarlos comprometer dinero y términos legales por su cuenta. El camino sensato es un humano aprobando el compromiso final mientras el agente prepara todo. Eso conserva la velocidad y elimina el riesgo.

### 7.5 Qué significa para tu empresa: contratos inteligentes, pagos automáticos, auditabilidad

**Contratos inteligentes, en palabras simples.** Un contrato inteligente es un programa que guarda un acuerdo y lo lleva a cabo cuando ocurre la condición dicha. No es astuto y no es un contrato en el sentido del abogado. Es una máquina expendedora muy literal. Escribe la regla con cuidado y es un gran sirviente. Escríbela con vaguedad y también es un gran sirviente —de lo que realmente escribiste.

**Pagos automáticos.** La forma práctica es un pago que espera. Espera una confirmación de entrega, un clic de aprobación, un hito aceptado, una fecha alcanzada. Cada uno está topado, registrado y es visible para ambos lados antes de moverse.

**Auditabilidad.** Cada paso deja un registro. Tu contable cierra el mes más rápido porque no hay nada que reconstruir. Una disputa con un cliente termina en minutos porque ambos lados miran la misma línea. Si un regulador pregunta, produces el registro en vez de una historia.

**Dónde encaja bien:** pagos a proveedores transfronterizos donde la aplicación es lenta; hitos de freelancers y contratistas; mercados donde comprador y vendedor son desconocidos; acuerdos de intercambio de datos donde debes probar qué liberaste y cuándo; seguros que pagan por un evento medido, como un retraso de vuelo.

**Dónde encaja mal:** cualquier cosa que necesite juicio, negociación o una relación. Cualquier cosa donde el disparador no pueda medirse con honestidad. Cualquier cosa donde un pago automático erróneo sea difícil de recuperar.

## Ética y responsabilidad

Los sistemas trustless cambian quién es responsable, y esa es exactamente la razón por la que necesitan un pensamiento cuidadoso.

**El código que hace cumplir también hace cumplir los errores.** Si tu regla libera un pago por una condición fácil de fingir, has automatizado una pérdida. Escribe la regla para el caso deshonesto, no solo para el eficiente.

**Los oráculos son personas.** Un "disparador medible por máquina" a menudo depende de que un humano introduzca datos en algún sitio. El eslabón más débil de una cadena trustless es el momento en que una persona escribe la verdad en ella. Diseña pensando que esa persona va con prisa, se equivoca o se deja sobornar.

**La inmutabilidad choca con la privacidad.** Poner datos personales en un registro permanente e inmutable puede entrar en conflicto con los derechos de protección de datos, incluido el derecho al olvido. Mantén los datos personales fuera de los libros públicos; guarda solo referencias y huellas. El detalle legal está en el [Capítulo 10](ch10-privacy-and-gdpr.md).

**No quites al humano de un problema humano.** Los clientes infelices no quieren una regla perfectamente aplicada; quieren que alguien los escuche. Lo trustless es para el tramo aburrido de una transacción, no para el momento en que alguien está alterado.

**Sé transparente, y mantén un dueño con nombre.** Di a las personas cuyo trabajo ahora mide el sistema, y explica cómo puede anularse una decisión; una regla que nadie puede cuestionar acabará estando mal sin nadie que pueda arreglarla. La aplicación automática no elimina la responsabilidad —alguien en tu empresa debe seguir siendo dueño del resultado, como establece el [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md).

## Errores a evitar

### 7.7 No todo necesita ser trustless

1. **Usar una blockchain donde bastaría una hoja de cálculo.** Si las partes se fían entre sí, el registro es pequeño, y un contrato normal funciona, un libro distribuido añade costo y complejidad para nada.
2. **Confundir trustless con libre de riesgo.** El código tiene bugs, los datos pueden estar mal, las claves pueden perderse, y a menudo no hay un número de soporte al que llamar.
3. **Automatizar un mal proceso.** Un sistema trustless hará cumplir tu mal proceso más rápido y con más consistencia de lo que nunca lo hizo una persona.
4. **Poner datos personales en una cadena pública.** No pueden borrarse después.
5. **Sin interruptor de parada.** Cualquier sistema de pago automático necesita una forma de detenerlo en un clic.
6. **Sin tope de gasto.** Un agente con una billetera abierta es una chequera abierta.
7. **Fiarte demasiado del disparador.** Pregúntate cómo podría fingirse el disparador, y luego decide si eso importa.
8. **Perseguir un discurso de ventas.** "Trustless" es una idea de diseño útil, no una razón para comprar un token. Si una propuesta no puede explicar el disparador, el registro y la vía de disputa, es marketing.
9. **Eliminar a todos los intermediarios.** Algunos intermediarios se ganan su comisión. Un notario, un agente de aduanas o un asegurador pueden estar haciendo un trabajo real que el código no puede hacer.
10. **Olvidar quién es responsable.** Incluso con aplicación automática, un humano con nombre debe ser dueño del resultado.

## Ejercicio práctico

### 7.8 Piensa en un proceso de negocio que podría beneficiarse de la automatización trustless

Elige un proceso donde ahora gastas tiempo comprobando, persiguiendo o discutiendo. Trabaja estas nueve preguntas por escrito.

1. **¿Quiénes son las partes?** Nómbralas. Anota si ya se fían entre sí.
2. **¿Qué debe ser verdad antes de que se mueva el dinero?** Una frase.
3. **¿Quién verifica eso hoy?** ¿Una persona? ¿Cuánto tarda? ¿Con qué frecuencia se equivoca?
4. **¿Cuánto cuesta esa verificación?** Tiempo, comisiones, retrasos. Números aproximados están bien; márcalos como aproximados.
5. **¿Puede una máquina medir el disparador?** Si sí, ¿cuál es la señal? Si no, ¿puede rediseñarse el proceso para que pueda?
6. **¿Cuál es el rastro de evidencia?** Qué registro existe, dónde, y puede alguna de las partes cambiarlo.
7. **¿Qué pasa en una disputa?** Quién decide, y qué tan rápido.
8. **¿Cuál es la peor forma en que esto podría abusarse?** Escribe el escenario deshonesto antes del eficiente.
9. **¿Cuál es el tope?** La pérdida máxima si la regla está mal.

Ahora puntúalo. Si el costo de verificación es una gran parte del valor de la transacción, el disparador es medible por máquina, y puedes fijar una pérdida máxima baja, el proceso es un fuerte candidato. Si el disparador no puede medirse por una máquina, o la pérdida máxima es alta, mantén un humano en él.

Escribe una página. Lleva un candidato a tu próxima reunión.

## Lista de verificación

### 7.9 Cuándo considerar un enfoque trustless

- [ ] **Pagas a un intermediario principalmente para retener o comprobar algo**, y esa comprobación podría escribirse como una regla.
- [ ] **Las partes no se fían ya entre sí**, y construir confianza sería lento o imposible.
- [ ] **La condición de liberación puede enunciarse como una sola frase comprobable** que una máquina puede medir.
- [ ] **La transacción ocurre a menudo**, así que el costo inicial se reparte entre muchos usos.
- [ ] **Es transfronteriza o entre empresas**, donde la aplicación local es lenta o poco clara.
- [ ] **Necesitas un registro compartido y no editable** que ambos lados y tu auditor puedan leer.
- [ ] **Puedes fijar un tope duro de gasto** y una parada en un clic antes de automatizar.
- [ ] **Ningún dato personal necesita quedar en el registro permanente.**
- [ ] **Existe una vía de disputa** y nombra un humano que puede anular la regla.
- [ ] **Lo has comparado con honestidad** con un contrato normal y un proceso normal, y lo trustless aún gana en costo, velocidad o riesgo.

## Puntos clave

- Trustless no significa ausencia de confianza; significa que verificas un hecho en vez de fiarte de que una persona te lo cuente.
- Las tres partes que funcionan son identidad verificable, registros a prueba de manipulaciones, y aplicación automática de una condición escrita.
- El borrador ERC-8004 de Ethereum y los estándares de abstracción de cuenta muestran hacia dónde va el negocio entre agentes: identidad, reputación y validación independiente, con presupuestos acotados por código.
- El eslabón más débil es el disparador —el momento en que un humano o un sensor dice al sistema lo que realmente pasó.
- No uses lo trustless donde un contrato normal funciona; úsalo donde la verificación es cara, el disparador es medible y la pérdida máxima está topada.
