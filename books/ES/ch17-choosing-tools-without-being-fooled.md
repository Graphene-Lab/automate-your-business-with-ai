# Capítulo 17 — Elegir herramientas sin dejarse engañar

## En palabras simples

Todo proveedor de IA te dirá que su herramienta es fácil, barata y revolucionaria. Algunos dicen la verdad. Muchos no. Este capítulo es tu defensa. Te enseña a mirar más allá de la demo brillante y del vendedor seguro de sí mismo, y a elegir una herramienta que de verdad encaje con tu negocio.

La idea más importante aquí es sencilla: **no estás comprando una herramienta, estás comprando un resultado.** Una herramienta solo vale lo que hace por ti. Un producto hermoso que no resuelve tu problema es un juguete caro. Tu trabajo es conectar cada decisión con un problema real y un número real.

Una buena analogía es comprar un coche. En el showroom todos los coches se ven increíbles. El cuero brilla, el motor ronronea, el vendedor es encantador. Pero no compras un coche por el showroom. Lo compras por el camino que realmente recorres, los pasajeros que realmente llevas y el combustible que puedes pagar. Así que haces preguntas difíciles, lo pruebas en *tus* caminos y revisas los costos de mantenerlo. Elegir herramientas de IA exige la misma disciplina.

Este capítulo cubre cómo elegir entre comprar software ya hecho, construir algo a medida o hacerlo tú mismo. Te da las preguntas exactas que debes hacerle a un proveedor. Te muestra dónde se esconden los costos ocultos. Explica por qué una demo no es suficiente y cómo hacer en cambio una pequeña prueba piloto. Y mira las herramientas de código abierto —software cuyo código es libre de usar y modificar— como una opción real y asequible.

Una regla para llevar contigo: **baja la velocidad.** El vendedor quiere urgencia. "Este precio termina el viernes." "Solo quedan dos licencias." La urgencia es un truco para que no pienses. Una buena herramienta sobrevive a una semana de reflexión cuidadosa. Una mala depende de que tú no pienses. Tómate esa semana.

## Un poco de historia

**Años 60–70: el software es a medida.** En los primeros tiempos, si una empresa quería software, pagaba a especialistas para escribirlo desde cero. No existía la opción "de estante". El software era un traje hecho a medida, caro y lento de entregar.

**Años 80: la revolución del software empaquetado.** Productos como las hojas de cálculo y los procesadores de texto llegaron en una caja. Por primera vez, un negocio podía comprar una herramienta general y adaptarla a muchos trabajos. Esto era más barato y rápido que los desarrollos a medida. Así nació el mercado moderno de software.

**Años 90–2000: las grandes suites y la trampa del cautiverio.** Los grandes proveedores vendían enormes suites integradas —un producto para todo—. Funcionaban bien, pero cambiarse a otra cosa era doloroso y costoso. Las empresas descubrieron que la decisión fácil de hoy podía convertirse en una cárcel cara mañana. La palabra **cautiverio del proveedor** —quedar atrapado con un proveedor porque irse es demasiado difícil— entró al vocabulario de los negocios. (El cautiverio se trata a fondo en el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).)

**Años 2000: el código abierto se vuelve masivo.** Linux, Apache y luego miles de proyectos libres demostraron que el software podía construirse en comunidad y regalarse, y aun así impulsar los sitios web más grandes del mundo. El código abierto dejó de ser un pasatiempo y se convirtió en una opción seria y confiable.

**Años 2010: la era de la suscripción.** El software pasó de "compra una vez" a "paga cada mes". Esto bajó el precio de entrada pero sumó un nuevo tipo de costo que nunca termina. Las suscripciones hicieron fácil empezar y fácil perder la cuenta de lo que estabas pagando.

**Años 2020: la fiebre del oro de la IA.** Cientos de herramientas de IA aparecieron casi de la noche a la mañana, muchas con gran financiamiento y promesas aún mayores. La brecha entre lo que muestra una demo y lo que una herramienta entrega en el trabajo real nunca ha sido más amplia. Elegir bien es hoy una habilidad central del negocio, no un extra agradable.

El arco: de lo hecho a medida, a lo empaquetado, a lo suscripto, a lo inundado. Las herramientas siguen cambiando. La necesidad de elegir con cuidado nunca lo hace.

## Curiosidad

### 17.6 El libro "Headcount Zero" — una empresa sin empleados

¿Hasta dónde puede llevarse la idea de "no se necesita gente"? Hay un libro que la lleva al extremo. Se llama **"Headcount Zero: cómo construir una empresa gestionada por IA con Paperclip"**, de **Anthony David Adams**. Está publicado como un libro de código abierto en GitHub (el repositorio `AnthonyDavidAdams/zero-employee-company-book`), así que cualquiera puede leerlo gratis.

La pregunta que plantea el libro es: *¿y si nunca tuvieras que contratar a nadie?* En lugar de empleados, el fundador dirige una empresa hecha de **agentes de IA** —programas que pueden realizar tareas por su cuenta—. El fundador se convierte en una especie de gerente de un organigrama lleno de trabajadores de IA, coordinados por una plataforma de código abierto que el libro llama **Paperclip**.

Este no es un plan que la mayoría de los pequeños negocios deba seguir mañana. Una empresa con literalmente cero humanos es un experimento mental extremo, y tiene límites obvios: ¿quién responde cuando algo sale mal? ¿Quién tiene la responsabilidad legal? ¿Quién entiende la necesidad no dicha de un cliente? (Estas son exactamente los roles humanos que se discuten en el [Capítulo 15](ch15-people-roles-and-culture.md).)

Pero como lente, "Headcount Zero" es útil. Fuerza una pregunta honesta: **¿cuánto de tu trabajo es realmente humano y cuánto es rutina que una máquina podría asumir?** La mayoría de los negocios descubre que una parte sorprendente de las tareas diarias es rutinaria. Eso no significa despedir a todos. Significa liberar a las personas de las partes aburridas para que puedan hacer el juicio, las relaciones y el trabajo creativo que las máquinas no pueden. Lee el libro como una provocación, no como una instrucción. Te muestra el borde de lo posible, y el borde es donde viven las preguntas interesantes.

## Un ejemplo de negocio real

*Lo siguiente es una composición ilustrativa de patrones reales comunes, no una empresa concreta con nombre.*

Una pequeña firma de contabilidad quería "automatizar con IA". Un proveedor dio una demo deslumbrante: la herramienta leía una pila de recibos y producía un resumen ordenado en segundos. El dueño firmó un contrato de dos años en el acto, deslumbrado.

Seis meses después, la realidad se veía distinto. La demo había usado un puñado de recibos limpios y perfectos. Los recibos reales de la firma estaban arrugados, borrosos, en tres idiomas y llenos de casos límite. La herramienta fallaba con la frecuencia suficiente como para que el personal tuviera que volver a revisar todo, lo que hacía que el "ahorro" fuera mínimo. El contrato de dos años los dejó atrapados. La suscripción seguía facturando. La herramienta se convirtió en un adorno caro.

Una segunda firma eligió distinto. Antes de firmar nada, le pidió al proveedor una **prueba con sus propios datos desordenados**, no con el conjunto limpio de la demo del proveedor. Hizo una prueba piloto de dos semanas con recibos reales. La herramienta manejó bien alrededor del 70% y falló en el resto. Ese número —70%— le permitió a la firma tomar una decisión clara: quedarse con la herramienta para el 70% fácil, mantener humanos en el 30% difícil, y firmar solo un contrato de un año con una salida clara. La misma herramienta, elegida con disciplina en lugar de deslumbramiento, se convirtió en una ayuda genuina.

La diferencia no fue el software. Fue que la segunda firma se negó a dejarse engañar por una demo y primero probó con su propia realidad.

## Cómo hacerlo

### 17.1 Software de estante, desarrollo a medida o hazlo tú mismo

Cuando necesitas una herramienta, tienes tres caminos amplios. Cada uno tiene su lugar.

**De estante (cómpralo ya hecho).** Es un software al que te suscribes o que compras tal cual, como un servicio de chatbot o una app para resumir documentos. Es la forma más rápida y normalmente la más barata de empezar. Lo tienes hoy, funciona desde el primer momento y alguien más lo mantiene. El intercambio: hace lo que *ella* fue construida para hacer, no exactamente lo que *tú* querías. Si tu necesidad es común, una herramienta de estante casi siempre es la primera elección correcta.

**A medida (paga a alguien para que lo construya).** Un desarrollador escribe software solo para ti. Esto se ajusta perfectamente a tus necesidades. Pero es lento, caro, y ahora eres dueño de algo que necesita mantenimiento para siempre. Los desarrollos a medida tienen sentido solo cuando tu necesidad es especial y ninguna herramienta ya hecho la cubre —y cuando el valor es lo bastante alto para justificar el costo—. Para la mayoría de los pequeños negocios, el desarrollo a medida rara vez es la primera jugada.

**Hazlo tú mismo (lo construyes tú, con herramientas no-code o ligeras).** Herramientas de automatización te permiten conectar servicios por tu cuenta sin escribir código. Esto es barato y flexible, y aprendes mucho. El intercambio: consume tu tiempo, y si te vas, lo que construiste puede ser difícil de mantener para otra persona. El "hazlo tú mismo" es genial para pequeñas automatizaciones que puedes controlar y mantener simples.

Una regla simple: **empieza con algo de estante. Pasa al "hazlo tú mismo" para el pequeño trabajo de pegamento entre herramientas. Ve a lo a medida solo cuando nada más encaje y el premio es grande.** La mayoría de los negocios vive feliz con los dos primeros.

### 17.2 Preguntas que hacerle al proveedor

Nunca te quedes con la palabra del proveedor. Haz preguntas directas y escucha con atención las respuestas —sobre todo lo que esquiva—. Ten estas listas:

- **¿Qué hace exactamente esto, y qué NO hace?** Oblígalos a ir más allá del marketing. Un seguro "maneja todo" es una señal de alerta.
- **¿Cómo se ve cuando falla?** Toda herramienta falla en algún punto. Un proveedor honesto puede nombrar sus puntos débiles. Un proveedor que dice "nunca falla" miente o no tiene idea.
- **¿Cuál es el costo total durante tres años, no solo el primer mes?** Haz que digan el número completo en voz alta.
- **¿Qué pasa con mis datos?** Dónde se almacenan, quién puede verlos y si entrenan su IA con ellos. (Esto importa para la privacidad —mira el [Capítulo 10](ch10-privacy-and-gdpr.md)—.)
- **¿Puedo sacar mis datos, y en qué formato?** Esta es tu salida de emergencia. Si no puedes irte limpiamente, estás atrapado.
- **¿Qué soporte recibo, y qué tan rápido?** Tiempos de respuesta, canales y si el soporte está incluido o cuesta extra.
- **¿Quién más usa esto en mi industria, y puedo hablar con ellos?** Una referencia real vale diez demos.
- **¿Cuál es tu hoja de ruta y qué tan estable es la empresa?** Una herramienta de una startup inestable puede desaparecer. Pregunta cuánto tiempo llevan en el negocio y quién los financia.
- **¿Cuál es el contrato, y cómo lo cancelo?** Lee las condiciones de salida antes de firmar, no después.

Escribe las respuestas. Compara proveedores con las mismas preguntas. El proveedor que responde con claridad y honestidad se destaca del que solo gesticula y encanta.

### 17.3 Costos ocultos y suscripciones

El precio de etiqueta es el costo más pequeño. El costo real se esconde en lugares donde la mayoría nunca mira. (El método de costo completo está en el [Capítulo 16](ch16-goals-costs-and-return-on-investment.md); aquí está la versión específica del proveedor.)

Vigila esto:

- **Precio por usuario.** Muchas herramientas cobran por usuario. Una herramienta "barata" se vuelve cara cuando sumas a todo tu equipo. Cuenta los puestos antes de firmar.
- **Tarifas por uso.** Algunas herramientas de IA cobran por tarea, por mensaje o por documento. Un mes ocupado puede producir una factura sorpresa. Pregunta exactamente cómo se mide el uso.
- **Costos de configuración e incorporación.** Empezar puede costar extra, a veces más que el primer año de suscripción.
- **Costos de integración.** Conectar la herramienta a tus sistemas actuales puede necesitar ayuda paga.
- **Funciones premium tras un muro de pago.** La función que te vendió puede estar en un nivel superior. Revisa qué nivel necesitas realmente.
- **Capacitación y soporte como complementos.** "Soporte incluido" a menudo significa un artículo de ayuda, no una persona. La ayuda real puede costar más.
- **La suscripción interminable.** Una tarifa mensual parece pequeña pero nunca se detiene. Multiplícala por tres o cinco años para ver el peso verdadero.
- **Costos de salida y de cambio.** Cancelar puede ser difícil, y mover tus datos a otro lado puede requerir trabajo pago.

Antes de firmar, calcula un **costo total a tres años** para cada opción. Suma cada uno de estos. El precio mensual del proveedor suele ser solo un tercio del número real a tres años.

### 17.4 Demos y proyectos piloto

Una demo es una actuación. Muestra la herramienta en su mejor momento, con datos elegidos para ganarte. Nunca decidas solo por una demo.

Un **proyecto piloto** es la alternativa honesta. Un piloto es una prueba pequeña y con tiempo limitado de la herramienta sobre *tu* trabajo real, con *tus* datos desordenados reales, midiendo *tu* resultado real. Donde una demo te muestra un resumen de momentos estelares, un piloto te muestra la verdad.

Cómo hacer un buen piloto:

- **Usa tus propios datos, incluidos los casos desordenados.** No aceptes la muestra limpia del proveedor.
- **Mantenlo pequeño y corto.** De dos a cuatro semanas en un proceso bastan para aprender mucho.
- **Define el éxito antes de empezar.** ¿Qué número debe alcanzar la herramienta para contar como aprobado? (Esto se conecta con el método de piloto en el [Capítulo 18](ch18-your-first-pilot-project.md).)
- **Prueba el fallo, no solo el éxito.** Empújala con casos difíciles a propósito.
- **Prueba el soporte.** Envía una solicitud de soporte durante el piloto y mira qué tan rápidos y útiles son.
- **Prueba la salida.** Intenta exportar tus datos. Asegúrate de poder irte.

Un proveedor que se niega a un piloto real con tus datos te está diciendo algo. Un proveedor que lo recibe con gusto está seguro por una buena razón.

### 17.5 Herramientas de código abierto: una alternativa asequible y flexible

**Código abierto** significa que el código fuente del software —las instrucciones que lo hacen funcionar— es libre para que cualquiera lo vea, use y modifique. No lo estás "pirateando"; el código abierto es una forma legal, común y a menudo excelente de hacer software. Es probable que la web que estás usando ahora funcione con software de código abierto.

Por qué considerarlo para IA:

- **Costo de licencia bajo o nulo.** Muchas herramientas de código abierto son gratis de usar.
- **Sin cautiverio.** Como puedes ver y cambiar el código, no quedas atrapado con un proveedor.
- **Puedes ejecutarlo tú mismo.** Los modelos de IA de código abierto pueden correr en tus propias máquinas, lo que mantiene tus datos bajo tu control (esto es **autoalojamiento**, tratado en el [Capítulo 8](ch08-self-hosting-keep-your-data-under-control.md)).
- **Una comunidad detrás.** Los proyectos populares mejoran rápido y tienen muchos usuarios de quienes aprender.

Los intercambios:

- **Puede que necesites más habilidad para configurarlo.** El código abierto a menudo da por hecho que puedes configurar cosas, o contratar a alguien que pueda.
- **El soporte es comunitario.** Puede que no haya a quién llamar. Depende de la documentación y los foros.
- **Tú eres dueño del mantenimiento.** Si lo ejecutas tú mismo, mantenerlo actualizado y seguro recae en ti.

El balance honesto: el código abierto es un camino poderoso y asequible, sobre todo cuando el control de los datos importa. Pero cambia dinero por esfuerzo y habilidad. Si no tienes ninguno de los dos, una herramienta de estante de pago puede ser el comienzo más sensato. Si tienes un poco de ayuda técnica, el código abierto puede ahorrarte mucho y liberarte del cautiverio.

## Ética y responsabilidad

Elegir herramientas no es éticamente neutro. Tus decisiones afectan a tus clientes, a tu personal y a tus datos.

**Protege los datos de tus clientes en la propia elección.** Antes de que cualquier herramienta toque datos de clientes, sabe a dónde van y quién puede verlos. Una herramienta que entrena su IA con la información privada de tus clientes sin consentimiento puede violar la ley (mira el [Capítulo 10](ch10-privacy-and-gdpr.md)).

**No dejes que el bombo del proveedor impulse una decisión que afecta a personas.** Si una herramienta va a cambiar los puestos de tu personal, elígela por razones honestas e involucra a tu gente, no porque un vendedor creó una falsa urgencia.

**Prefiere herramientas que puedas auditar y abandonar.** Una herramienta que esconde cómo funciona, o atrapa tus datos, es una mala elección ética además de un mal negocio. La transparencia y una salida limpia son señales de un proveedor que te respeta.

**Sé honesto en tus propias afirmaciones.** Si compras una herramienta de IA y dices a los clientes "nuestro servicio usa IA", asegúrate de que sea verdad y no un marketing exagerado.

**Considera la ética del propio proveedor.** ¿Dónde viven sus datos? ¿Respetan las leyes de privacidad? ¿Son estables y honestos? Te estás asociando con ellos; elige un socio en el que confiarías tu nombre.

Una herramienta es una relación. Elige al socio con tanto cuidado como elegirías a un socio de negocios.

## Errores a evitar

### 17.7 Errores comunes

**Comprar por la demo.** Decidir a partir de una actuación pulida con datos limpios. Haz siempre un piloto con tu propia realidad desordenada.

**Ignorar el costo a tres años.** Mirar el precio mensual y no el total. La suscripción nunca se detiene.

**Caer en la urgencia.** "El precio termina el viernes" es un truco de ventas. Una buena herramienta sobrevive a una semana de reflexión.

**Sin plan de salida.** Firmar sin revisar cómo sacar tus datos. Así es como ocurre el cautiverio.

**Comprar antes de definir el problema.** Conseguir una herramienta y luego buscarle un uso. Define primero el problema, luego busca la herramienta.

**Confundir popularidad con ajuste.** Una herramienta usada por miles puede aun así no encajar con *tu* flujo de trabajo.

**Saltarse la prueba de soporte.** No revisar cómo se comporta el proveedor después de la venta. Prueba el soporte durante el piloto.

**Sobrepersonalizar demasiado pronto.** Pagar por un desarrollo a medida cuando una herramienta de estante cubriría el 80% de la necesidad.

**Subestimar el mantenimiento del "hazlo tú mismo".** Construirlo tú mismo y olvidar que ahora tienes que mantenerlo vivo.

**Confiar en "maneja todo".** Ninguna herramienta lo hace. Un proveedor que afirma lo contrario no te dice la verdad.

**No leer el contrato.** Firmar sin leer la cancelación y las condiciones de datos. Lee antes, no después.

**Elegir la etiqueta más barata.** El precio mensual más bajo puede esconder el costo total más alto.

## Ejercicio práctico

### 17.8 Ejercicio: una cuadrícula de evaluación

Construye una simple cuadrícula de puntuación para comparar herramientas lado a lado. Esto convierte una decisión difusa en una clara.

**Paso 1 — Lista tus opciones.** Anota dos o tres herramientas candidatas (o caminos: de estante, hazlo tú mismo, código abierto).

**Paso 2 — Lista los criterios.** Usa estos, o añade los tuyos:

- Se ajusta a mi problema real (0–5)
- Maneja bien mis datos desordenados (0–5)
- Costo total a tres años (más bajo es mejor — puntúalo)
- Facilidad de uso para mi personal (0–5)
- Privacidad y control de datos (0–5)
- Facilidad de salida / sin cautiverio (0–5)
- Calidad del soporte (0–5)
- Estabilidad del proveedor (0–5)

**Paso 3 — Puntúa cada herramienta.** Da un número para cada criterio. Sé honesto, no esperanzado.

**Paso 4 — Pondera lo que más importa.** Si la privacidad de datos es crítica para ti, duplica su peso. Si el costo importa más, ponle un peso mayor.

**Paso 5 — Suma todo.** La herramienta con la puntuación ponderada más alta es tu favorita.

**Paso 6 — Prueba la favorita con un piloto.** La cuadrícula reduce el campo; el piloto lo confirma. No te saltes el piloto.

Pon la cuadrícula en una sola página. Hace la decisión visible y defendible, y evita que un vendedor encantador anule tu juicio con su encanto.

## Lista de verificación

### 17.9 Lista de verificación para evaluar a un proveedor

Antes de firmar con cualquier proveedor de IA, marca cada casilla.

- [ ] **Puedo enunciar el problema exacto que esta herramienta resuelve para mí.**
- [ ] **Sé lo que la herramienta NO hace, y dónde falla.**
- [ ] **Tengo un costo total a tres años, no solo el precio mensual.**
- [ ] **Sé cómo funciona el precio** — por puesto, por uso, niveles, tarifas de configuración.
- [ ] **Sé dónde se almacenan mis datos y quién puede verlos.**
- [ ] **Sé si el proveedor entrena su IA con mis datos, y consiento o me niego.**
- [ ] **He probado la herramienta con mis propios datos desordenados, no con el conjunto de demo del proveedor.**
- [ ] **He hecho un pequeño piloto con un número de éxito definido.**
- [ ] **He probado el soporte del proveedor durante la prueba.**
- [ ] **He probado exportar mis datos fuera de la herramienta.**
- [ ] **He leído las condiciones de cancelación antes de firmar.**
- [ ] **Tengo una referencia de otro negocio de mi ramo, o intenté conseguirla.**
- [ ] **Revisé la estabilidad del proveedor y cuánto tiempo lleva en el negocio.**
- [ ] **Resistí la urgencia y me tomé tiempo para pensar.**
- [ ] **Comparé al menos dos opciones con los mismos criterios.**

Si una casilla está vacía, no has terminado de evaluar. Llénala antes de firmar. Una herramienta elegida con la cabeza clara vale mucho más que una comprada en un deslumbramiento.

## Puntos clave

- No estás comprando una herramienta, estás comprando un resultado — conecta cada decisión con un problema real y un número real.
- Una demo es una actuación con datos limpios; un piloto con tus propios datos desordenados es la única prueba honesta.
- El precio mensual es solo una fracción del costo — siempre calcula un total a tres años que incluya puestos, uso, configuración, soporte y salida.
- El código abierto es un camino real, asequible y libre de cautiverio, pero cambia dinero por esfuerzo y habilidad; elígelo cuando tengas la ayuda para ejecutarlo.
- Rechaza la urgencia: una buena herramienta sobrevive a una semana de reflexión cuidadosa, y un proveedor que recibe con gusto un piloto real está seguro por una buena razón.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Comparar productos antes de comprar

![Una comparación de productos lado a lado](../../assets/examples/product-compare.png)
*Una comparación de productos lado a lado*

**Lo que pides:** `Compara estas dos impresoras para una pequeña oficina: precio, costo de operación y confiabilidad.`

El agente investiga ambos productos y presenta una comparación clara para que puedas elegir la mejor opción según tu presupuesto y tu uso.

*Consejo: Pide el costo total de propiedad, no solo el precio de etiqueta.*

<!-- END agentbridge-examples -->
