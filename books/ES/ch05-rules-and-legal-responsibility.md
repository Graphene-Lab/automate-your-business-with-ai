# Capítulo 5 — Reglas y responsabilidad legal: la Ley de IA de la UE

## En palabras simples

Cada herramienta nueva trae reglas. Los coches trajeron las normas de tráfico. Los bancos trajeron reglas sobre el manejo del dinero. Ahora la IA está teniendo su propio reglamento, y si haces negocios en Europa o con Europa, ese reglamento es la **Ley de IA de la UE**.

Este capítulo es su guía en lenguaje sencillo. No hace falta formación legal. El objetivo es simple: que puedas decir si una herramienta que quieres usar está poco regulada, muy regulada o directamente prohibida, y qué debes hacer al respecto.

Dos ideas explican casi toda la ley.

La primera es el **riesgo**. La Ley de IA no trata toda la IA igual. Clasifica los sistemas de IA por niveles según el daño que puedan causar. Un filtro de spam casi no se toca. Un sistema que decide quién consigue un préstamo o un trabajo se vigila de cerca. Un puñado de prácticas están simplemente prohibidas. Cuanto mayor es el riesgo, más debes hacer.

La segunda es **tu papel**. La ley separa al **proveedor** (quien construye o marca un sistema de IA y lo pone en el mercado) del **responsable de la implantación** (quien lo usa). La mayoría de las pequeñas y medianas empresas son responsables de la implantación. Tus deberes son distintos a los del proveedor, pero son reales, y son tuyos.

Una nota sobre el alcance. La Ley de IA es ley europea. Si estás fuera de la UE pero tu IA afecta a personas dentro de la UE, partes de ella aún pueden alcanzarte. Consulta con un profesional si atiendes a clientes europeos.

### 5.1 El RGPD en palabras simples: lo que debes saber

El **RGPD** (Reglamento General de Protección de Datos) es la ley europea sobre datos personales. Se aplica desde 2018 y aún rige todo lo que hagas con información sobre personas identificables —incluidos los datos que introduces en una IA.

En un párrafo: si recoges, almacenas o procesas datos personales de personas en la UE, necesitas un motivo legal para hacerlo, debes decir a la gente para qué usas sus datos, mantenerlos seguros, guardar solo lo que necesitas, permitir que las personas los consulten o borren a petición, y no conservarlos más tiempo del necesario. Las infracciones pueden traer multas grandes. La IA no cambia estos deberes; solo te da más formas de incumplirlos, porque los modelos necesitan datos y los datos son personales. El tratamiento completo y detallado del RGPD —bases legales, derechos de las personas y cómo cumplir— es el hogar del [Capítulo 10](ch10-privacy-and-gdpr.md). Lee ese capítulo antes de procesar cualquier dato de clientes con IA. El punto aquí es solo que la Ley de IA y el RGPD se aplican juntos, uno encima del otro, no en lugar del otro.

### 5.2 Datos personales frente a datos sensibles: la diferencia que importa

El RGPD traza una línea que importa mucho para la IA, porque la categoría más alta conlleva reglas más estrictas.

**Dato personal** es cualquier información sobre una persona viva que pueda ser identificada, directa o indirectamente. Un nombre, un correo, un teléfono, una ubicación, un identificador en línea. Incluso una combinación de hechos corrientes que apunte a una persona cuenta.

**Dato sensible** (la ley lo llama "categorías especiales") es un conjunto más pequeño de hechos más delicados: origen racial o étnico, opiniones políticas, creencias religiosas o filosóficas, afiliación sindical, datos genéticos, datos biométricos usados para identificar a alguien, datos de salud, y datos sobre la vida sexual u orientación sexual de una persona.

Por qué importa esta línea para ti: procesar datos sensibles necesita un fundamento legal más fuerte y más protección. Es también el dato más probable a causar discriminación si moldea una decisión de IA. Muchas de las reglas más estrictas de la Ley de IA existen porque la IA puede convertir datos corrientes en inferencias sensibles, o usar datos sensibles para clasificar personas. Para las definiciones y reglas de manejo completas, mira el [Capítulo 10](ch10-privacy-and-gdpr.md).

## Un poco de historia

Europa escribió primero su reglamento de privacidad y después su reglamento de IA, y el orden explica ambos.

El **RGPD** se adoptó en 2016 y pasó a ser directamente exigible en mayo de 2018. Fue la ley de privacidad de datos más completa de su época, y como tantas empresas globales tratan con europeos, fijó un estándar mundial. Su idea central —que las personas son dueñas de sus datos personales y necesitas un motivo legal para usarlos— se convirtió en la plantilla de las leyes de privacidad en otras partes.

Para la IA, Europa tomó un camino de principios primero. En 2018 la Comisión Europea creó un Grupo de Expertos de Alto Nivel sobre IA, que en 2019 publicó directrices éticas voluntarias construidas en torno a la "IA confiable". La Comisión convirtió luego los principios en ley, proponiendo la Ley de IA en abril de 2021. Tras años de negociación, se publicó en el Diario Oficial de la Unión Europea el **12 de julio de 2024** y entró en vigor el **1 de agosto de 2024**. Es la primera ley integral y horizontal sobre inteligencia artificial del mundo —"horizontal" significa que cubre la IA en todos los sectores, no una industria a la vez.

La ley no arranca toda de golpe. Se enciende por etapas, dando tiempo a las empresas para prepararse. Ese calendario escalonado es lo más práctico de este capítulo, y aparece en la sección 5.3. La historia muestra la dirección: de directrices éticas blandas a obligaciones duras y con fecha. El debate terminó. El reloj corre.

## Curiosidad

### La primera ley de IA del mundo —y multas que superan al RGPD

Aquí hay un dato que conviene conocer antes de cualquier conversación sobre "cumplir es demasiado caro".

La Ley de IA de la UE es la primera ley integral sobre IA en cualquier parte. Ninguna otra gran economía tiene una que iguale su amplitud. Eso la convierte en un caso de prueba, y también le da una especie de peso: las empresas de todo el mundo suelen construir según la regla más estricta a la que puedan enfrentarse, así que una norma europea puede volverse en silencio un estándar global. A esto lo llaman el "efecto Bruselas".

El otro dato llamativo es el tamaño de las sanciones. La multa máxima del RGPD es de hasta el 4% del volumen de negocios anual total a escala mundial de una empresa. La Ley de IA va más alto para las peores violaciones. Para las prácticas prohibidas de la sección 5.5, las multas pueden llegar a **35 millones de euros o el 7% del volumen de negocios anual total a escala mundial, lo que sea mayor.** Para la mayoría de las demás infracciones de la Ley, el tope ronda los 15 millones de euros o el 3%. Por dar información inexacta a las autoridades, unos 7,5 millones de euros o el 1%. (Para las pequeñas y medianas empresas la ley limita las multas a la cifra menor de las dos, así que la carga se reduce —pero sigue siendo real.)

La lección es tajante. La práctica que la ley más teme —los usos prohibidos— lleva la multa más pesada de la regulación digital europea, más pesada que el RGPD. Eso te dice exactamente dónde está la línea, y te dice que "no lo sabíamos" no es una excusa barata.

## Un ejemplo real de negocio

### Un pequeño prestamista que puntúa el crédito con IA

Este ejemplo es ilustrativo. Es un escenario realista, no el resultado reportado de una empresa, construido para mostrar cómo funcionan los niveles en la práctica.

Imagina una pequeña empresa de préstamos al consumo que quiere usar un modelo de IA para decidir si aprueba un préstamo personal.

El paso uno es encontrar el nivel. La Ley de IA enumera categorías de IA de alto riesgo en un anexo. Una categoría cubre los **servicios privados y públicos esenciales**, e incluye explícitamente la **evaluación de la solvencia** —decidir si una persona consigue crédito. Así que este modelo de préstamos es de **alto riesgo**. No está prohibido, pero se sienta en el nivel de trabajo más regulado.

Qué significa eso para la empresa, en términos simples:

- Debe gestionar un **sistema de gestión de riesgos** a lo largo de toda la vida del modelo, no solo una vez.
- Debe gobernar sus **datos**: los datos usados para entrenar y probar el modelo deben ser relevantes, representativos y lo más libres de error posible para el propósito. Un modelo entrenado sobre todo con un tipo de prestatario tratará injustamente a los demás.
- Debe mantener **documentación técnica** y **registros automáticos** del funcionamiento del sistema.
- Debe diseñar para la **supervisión humana**: una persona debe poder revisar y anular una decisión.
- Debe garantizar **precisión, robustez y ciberseguridad**.
- Antes de ponerlo en el mercado para su uso, debe completar una **evaluación de conformidad**, redactar una **Declaración UE de Conformidad**, adjuntar un **marcado CE** y **registrar el sistema en la base de datos de la UE** para IA de alto riesgo.

Ahora cambia un detalle y cambia el nivel. Supón que en vez de eso la empresa usa la IA solo para redactar correos amables de recordatorio sobre préstamos existentes, sin ninguna decisión sobre la aprobación. Eso no es una función de alto riesgo. Cae en un nivel ligero, donde el deber principal es la transparencia: la gente debe saber que hay medios automatizados involucrados donde sea requerido.

Misma empresa, mismo proveedor de tecnología, dos cargas legales muy distintas —porque el *uso* determina el nivel, no la herramienta. Esa es toda la lógica de la Ley en una sola escena.

## Cómo hacerlo

### 5.3 La Ley de IA de la UE: qué cambia para las empresas

La Ley clasifica la IA en cuatro niveles de riesgo, más una vía aparte para los grandes modelos de propósito general que hay detrás de los chatbots.

**Nivel 1 — Inaceptable (prohibido).** Un pequeño conjunto de prácticas está prohibido por completo. Mira la sección 5.5. Si tu uso cae aquí, no puedes hacerlo en absoluto.

**Nivel 2 — Alto riesgo.** Sistemas que pueden dañar gravemente la salud, la seguridad o los derechos fundamentales. Estos conllevan el régimen de cumplimiento completo: gestión de riesgos, gobernanza de datos, documentación, registros, transparencia hacia los usuarios, supervisión humana, precisión y seguridad, evaluación de conformidad, marcado CE y registro. Los usos de alto riesgo están listados en dos anexos: el Anexo I (IA como componente de seguridad en productos regulados) y el Anexo III (usos sensibles listados).

**Nivel 3 — Riesgo limitado / de transparencia.** Sistemas que no son de alto riesgo pero que interactúan con personas o generan contenido. El deber principal es la divulgación: decir a la gente que está tratando con una IA, y etiquetar el contenido sintético. Mira la sección 5.6.

**Nivel 4 — Riesgo mínimo.** Todo lo demás —filtros de spam, previsión de inventario, la mayoría de las herramientas internas de productividad. Ninguna obligación nueva más allá de la ley existente.

Las **categorías de alto riesgo del Anexo III** son las que un dueño de negocio es más probable que encuentre. Incluyen: biometría (donde no esté prohibida); componentes de seguridad de infraestructuras críticas; educación y formación (admisiones, evaluación del aprendizaje); **empleo y gestión de trabajadores** (reclutamiento, filtrado de solicitudes, promoción, despido, asignación de tareas, monitorización del desempeño); **servicios esenciales** (elegibilidad para prestaciones, solvencia, triaje de llamadas de emergencia, riesgo y tarificación de seguros); aplicación de la ley; migración y control de fronteras; y administración de justicia y procesos democráticos.

Una excepción útil: un sistema del Anexo III **no** es de alto riesgo si solo hace una tarea procesal estrecha, mejora algo que un humano ya hizo, detecta patrones sin reemplazar la evaluación humana, o da un paso puramente preparatorio. Pero es **siempre de alto riesgo si perfila a una persona.** Perfilar significa usar datos para evaluar o predecir aspectos sobre un individuo.

**Tu papel decide tus deberes.** Un proveedor carga con las pesadas obligaciones del lado de la construcción. Un responsable de la implantación (la mayoría de las empresas) carga con deberes del lado del uso: usar el sistema según lo indicado, asegurar la supervisión humana, monitorizar, guardar ciertos registros, y en algunos casos hacer una comprobación de derechos fundamentales. Si solo *usas* una herramienta de alto riesgo de un proveedor, no haces la evaluación de conformidad —la hace el proveedor—, pero aun así debes implantarla correcta y responsablemente.

**El calendario escalonado.** Memoriza estas fechas si tocas la IA en Europa:

| Fecha | Qué se aplica |
|---|---|
| 1 ago 2024 | La Ley entra en vigor |
| 2 feb 2025 | Se aplican las prácticas prohibidas (Art. 5) y el deber de alfabetización en IA (Art. 4) |
| 2 ago 2025 | Reglas para modelos de IA de propósito general, órganos de gobernanza y marco de sanciones |
| 2 ago 2026 | Obligaciones de alto riesgo para los usos del Anexo III (empleo, crédito, educación, servicios esenciales, etc.) |
| 2 ago 2027 | Obligaciones de alto riesgo para los productos del Anexo I (componentes de seguridad de IA en productos regulados) |

La UE ha propuesto algunas simplificaciones desde entonces, a veces llamadas un "paquete ómnibus digital", y las fechas o detalles pueden moverse. Toma la tabla como línea base de trabajo y confirma las fechas actuales contra el texto oficial antes de depender de un plazo.

### 5.4 Obligaciones para los sistemas de alto riesgo: evaluación de conformidad y documentación técnica

Si tu uso es de alto riesgo, estas son las cosas concretas requeridas. Como responsable de la implantación no necesitas realizarlas todas tú mismo, pero debes entenderlas para elegir un proveedor y para implantar correctamente.

**Gestión de riesgos.** Un proceso continuo, a lo largo de toda la vida del sistema, que encuentra, evalúa y reduce los riesgos para la salud, la seguridad y los derechos fundamentales. No un formulario de una sola vez.

**Gobernanza de datos.** Los datos de entrenamiento, validación y prueba deben ser relevantes, representativos y tan libres de errores y completos como el propósito lo permita. Aquí es donde el sesgo se detecta o se pasa por alto.

**Documentación técnica.** Un registro escrito que muestra que el sistema cumple y que permite a las autoridades comprobarlo. Cubre cómo funciona el sistema, con qué se entrenó, cómo se probó y cómo usarlo. Guárdala, junto con cualquier decisión de evaluación y cambios aprobados.

**Registro de datos (logging).** El sistema debe registrar automáticamente los eventos relevantes para los riesgos y para los cambios, para que su comportamiento pueda revisarse después. Los registros son tu evidencia.

**Transparencia hacia los responsables de la implantación.** Instrucciones de uso claras para que las personas que operan el sistema puedan cumplir sus propios deberes.

**Supervisión humana.** El sistema debe estar diseñado para que un humano pueda entenderlo, monitorizarlo, interpretar su resultado e intervenir o detenerlo.

**Precisión, robustez, ciberseguridad.** El sistema debe alcanzar niveles apropiados de los tres y ser resistente al error y al ataque.

**Gestión de la calidad y accesibilidad.** Un sistema para mantener el cumplimiento en el tiempo, y requisitos de accesibilidad cumplidos.

**Evaluación de conformidad, marcado CE, registro.** Antes de que un sistema de alto riesgo se ponga en el mercado, el proveedor realiza una **evaluación de conformidad** (una comprobación independiente por un "organismo notificado" donde la ley lo exige). Al aprobar, el proveedor redacta una **Declaración UE de Conformidad**, adjunta un **marcado CE** y **registra el sistema en la base de datos de la UE**. Como responsable de la implantación, debes pedir ver esto antes de comprar. Si un proveedor no puede mostrar una vía de conformidad para un uso de alto riesgo, eso es una señal de alarma grave.

### 5.5 Prácticas prohibidas: lo que absolutamente no puedes hacer con IA

Esto está prohibido en toda la UE desde el 2 de febrero de 2025. Si un caso de uso encaja, descártalo. Las multas aquí son las más pesadas de la ley.

1. **Técnicas subliminales o manipulativas** que vayan más allá de la conciencia de una persona y distorsionen materialmente su comportamiento de un modo que cause, o sea probable que cause, un daño significativo.
2. **Explotar vulnerabilidades** de personas por su edad, discapacidad o situación social o económica, para distorsionar su comportamiento y causar un daño significativo.
3. **Puntuación social** por parte de autoridades públicas —puntuar sistemáticamente a las personas por su comportamiento social o rasgos personales de formas que lleven a un trato dañino no relacionado con el contexto, o desproporcionado al comportamiento.
4. **Raspado sin objetivo de imágenes faciales** de internet o de circuitos cerrados de televisión para construir bases de datos de reconocimiento facial.
5. **Reconocimiento de emociones en el lugar de trabajo y en la educación** —inferir las emociones de trabajadores o estudiantes, salvo por razones médicas o de seguridad. (Una herramienta que "lee" el ánimo de un agente de un centro de llamadas para puntuarlo cae de lleno en esta prohibición.)
6. **Categorización biométrica que infiera atributos sensibles** —usar datos biométricos para adivinar raza, opiniones políticas, afiliación sindical, creencias religiosas o filosóficas, vida sexual u orientación sexual.
7. **Identificación biométrica remota en tiempo real en espacios públicos para la aplicación de la ley**, prohibida salvo unas pocas situaciones estrechas y autorizadas como buscar personas desaparecidas o prevenir una amenaza grave e inminente específica.

La mayoría de las pequeñas empresas nunca tocará estas. Pero dos toman a la gente por sorpresa: **el reconocimiento de emociones en el trabajo** y **el diseño manipulativo que explota la vulnerabilidad**. Si un proveedor te vende "IA que detecta las emociones de clientes o empleados", sabe que en un entorno de trabajo o escolar está prohibido.

### 5.6 Obligaciones de transparencia: cuándo debes informar a clientes y empleados

Para los sistemas que no son de alto riesgo pero que interactúan con personas o crean contenido, el deber principal es ser abierto. Estas reglas de transparencia se aplican desde el 2 de agosto de 2026.

**Di a la gente que está hablando con una IA.** Si un sistema de IA interactúa directamente con una persona —un chatbot, por ejemplo—, esa persona debe ser consciente de que está tratando con una IA, salvo que sea obvio. Un bot de atención al cliente debería decirlo.

**Etiqueta el contenido sintético y los deepfakes.** El audio, las imágenes, el vídeo o el texto generados o manipulados por IA deben marcarse como generados o manipulados artificialmente. Esto apunta a los deepfakes y a los medios hechos a máquina.

**Divulga el reconocimiento de emociones y la categorización biométrica.** Donde tales sistemas se usen legalmente (fuera de los casos prohibidos de trabajo y educación), las personas expuestas a ellos deben ser informadas.

Una pequeña nota de margen: los sistemas ya puestos en el mercado antes del 2 de agosto de 2026 tienen una breve ventana hasta finales de 2026 para cumplir la regla de etiquetado de contenido sintético. Planifica cumplir de todos modos.

Para un negocio, la jugada práctica es simple y barata: pon un aviso claro en tu chatbot ("Estás chateando con un asistente automatizado"), etiqueta cualquier medio generado por IA que publiques, y nunca hagas análisis oculto de emociones o biométrico sobre las personas.

### 5.7 Documentar las decisiones importantes

A través de cada nivel, un hábito te protege: **anota tus decisiones y tu razonamiento.**

Una buena documentación no es burocracia. Es tu memoria y tu defensa. Cuando un regulador, un cliente o un tribunal te pregunte por qué usaste un sistema de cierta manera, el registro escrito es tu respuesta.

Para cada sistema de IA, guarda un archivo simple que registre:

- **Qué hace y quién es su dueño.** El caso de uso, el nivel en que lo colocaste, y el propietario con nombre.
- **Por qué lo elegiste.** La razón de negocio y las alternativas que consideraste.
- **Cómo evaluaste el riesgo.** La revisión de riesgo ético y legal, incluido cualquier chequeo de sesgo y cualquier comprobación de derechos fundamentales.
- **Qué controles pusiste.** Supervisión humana, registros, avisos de transparencia, límites de datos.
- **Qué probaste y cuándo.** Resultados de pruebas, fechas, y quién los revisó.
- **Cambios en el tiempo.** Cualquier modificación al sistema o a su uso, con la razón y la fecha.
- **Incidentes y correcciones.** Todo lo que salió mal y qué hiciste al respecto.

Este archivo se conecta directamente con el trabajo de ética en el [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md). La evaluación de riesgo que haces allí se convierte parte de tu registro legal aquí. Un documento, dos propósitos.

Una regla práctica: **si importaba y no lo anotaste, prepárate para que te lo cuestionen y para que no tengas respuesta.**

## Ética y responsabilidad

El cumplimiento es el suelo, no el techo. Cumplir la letra de la Ley de IA no hace ético un uso, y no elimina tu responsabilidad. La ley te dice qué no debes hacer y qué requieren los usos de alto riesgo. No te dice si un uso es justo o sensato. Ese es tu juicio, cubierto en el [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md). Un sistema puede ser totalmente conforme y aun así dañar la confianza si lo implantas con descuido.

Tu papel moldea tu deber. Como **responsable de la implantación**, eres responsable de usar un sistema según lo indicado, mantener un humano al control donde se requiera, monitorizar cómo se comporta, y ser honesto con las personas a las que toca. No puedes señalar al proveedor e irte. Una postura práctica: **trata cada requisito legal como el mínimo, y deja que tu propia ética fije el estándar por encima.** Cuando puedas mostrar que hiciste más que el mínimo, ganas credibilidad —y para una pequeña empresa, la credibilidad vale más que cualquier automatización suelta.

## Errores a evitar

**Error 1: Asumir que tu herramienta es "solo un chatbot" y no está regulada.** El nivel depende de lo que decide, no de cómo se llame. Un chatbot que influye en el crédito o la contratación es de alto riesgo.

**Error 2: No conocer tu papel.** Proveedor y responsable de la implantación tienen deberes distintos. Si solo usas una herramienta de alto riesgo de un proveedor, aún tienes deberes de responsable de la implantación. Sabes cuál eres.

**Error 3: Perder las fechas escalonadas.** Las prohibiciones y el deber de alfabetización en IA ya están vigentes (febrero de 2025). Los deberes de alto riesgo llegan en 2026 y 2027. No trates toda la ley como "más adelante".

**Error 4: Comprar una herramienta de alto riesgo sin vía de conformidad.** Si un proveedor no puede mostrar una evaluación de conformidad, una Declaración de Conformidad y un registro para un uso de alto riesgo, no lo compres.

**Error 5: Ejecutar reconocimiento de emociones en el trabajo.** Está prohibido en lugares de trabajo y escuelas. Un discurso de ventas de "detección de ánimo" sobre el personal es una trampa.

**Error 6: Olvidar el deber de alfabetización en IA.** El Artículo 4 ya es ley. Debes tomar medidas razonables para formar a las personas que usan tu IA.

**Error 7: Confundir el RGPD con la Ley de IA.** Son leyes separadas que se apilan. Cumplir una no cubre la otra. Lee el [Capítulo 10](ch10-privacy-and-gdpr.md) para el lado de la privacidad.

**Error 8: No documentar.** Ningún registro escrito significa ninguna defensa cuando te pidan explicar una decisión.

**Error 9: Tratar el cumplimiento como la meta final.** La ley es el suelo. La ética y la confianza están por encima, y sigues siendo dueño de ellas.

## Ejercicio práctico

### 5.8 Tu lista de verificación de cumplimiento

Toma un sistema de IA que uses o planees usar y clasifícalo. Esto toma cerca de una hora y te dice qué reglas te atan.

**Paso 1 — ¿Está prohibido?** Lee las siete prácticas prohibidas en la sección 5.5. Si tu uso encaja en alguna, para. No continúes.

**Paso 2 — ¿Es de alto riesgo?** Revisa las categorías del Anexo III: biometría, infraestructura crítica, educación, **empleo y gestión de trabajadores**, **servicios esenciales (crédito, prestaciones, seguros)**, aplicación de la ley, migración, justicia. ¿Encaja tu uso en una? Si sí, es de alto riesgo salvo que aplique la excepción estrecha —y es siempre de alto riesgo si perfila a una persona.

**Paso 3 — ¿Es un caso de transparencia?** ¿Interactúa con personas o genera contenido? Si sí, debes divulgar el uso de IA y etiquetar el contenido sintético.

**Paso 4 — ¿Mínimo?** Si nada de lo anterior, estás en el nivel mínimo. Ningún deber nuevo de la Ley de IA, pero la ley existente y tu propia ética aún se aplican.

**Paso 5 — ¿Cuál es tu papel?** ¿Proveedor o responsable de la implantación? Anótalo. Enumera los deberes que se derivan de ese papel.

**Paso 6 — Si es de alto riesgo, reúne la prueba del proveedor.** Pide la evaluación de conformidad, la Declaración UE de Conformidad, el marcado CE y el registro en la base de datos de la UE. Anota qué falta.

**Paso 7 — Mapea tus deberes de responsable de la implantación.** Supervisión humana, monitorización, registros, avisos de transparencia, y cualquier comprobación de derechos fundamentales que te aplique.

**Paso 8 — Revisa el calendario.** ¿Cuáles de tus obligaciones ya están vigentes (alfabetización, prohibiciones) y cuáles llegan en 2026 o 2027? Ponles fecha.

**Paso 9 — Abre el archivo.** Empieza el archivo de documentación de la sección 5.7 con tu clasificación y tu plan.

Si no puedes colocar un sistema en un nivel con seguridad, eso es en sí el hallazgo: busca ayuda experta antes de implantar.

## Lista de verificación

### 5.9 Tu política legal para la IA

- [ ] Conozco los cuatro niveles de riesgo: prohibido, alto riesgo, transparencia, mínimo.
- [ ] Sé nombrar las categorías de alto riesgo del Anexo III, especialmente empleo y servicios esenciales (crédito, seguros).
- [ ] Sé que perfilar a una persona hace que un uso del Anexo III sea siempre de alto riesgo.
- [ ] Conozco las siete prácticas prohibidas y que el reconocimiento de emociones en el trabajo/escuela es una.
- [ ] Conozco mi papel para cada sistema: proveedor o responsable de la implantación.
- [ ] Conozco las fechas escalonadas: prohibiciones y alfabetización en IA vigentes desde el 2 feb 2025; alto riesgo del Anexo III en ago 2026; productos del Anexo I en ago 2027.
- [ ] Para herramientas de alto riesgo, exijo la evaluación de conformidad del proveedor, la Declaración de Conformidad, el marcado CE y el registro en la base de datos de la UE.
- [ ] Divulgo la interacción con IA a los clientes y etiqueto el contenido generado por IA.
- [ ] Mantengo supervisión humana y registros donde el nivel lo requiera.
- [ ] Tengo un plan para cumplir el deber de alfabetización en IA para el personal que usa nuestros sistemas.
- [ ] Entiendo que el RGPD se aplica encima de la Ley de IA, y he leído el [Capítulo 10](ch10-privacy-and-gdpr.md).
- [ ] Guardo un archivo de documentación para cada sistema: uso, nivel, dueño, evaluación de riesgo, controles, pruebas, cambios, incidentes.
- [ ] Trato el cumplimiento como el suelo y mi propia ética como el estándar por encima.
- [ ] Busco ayuda experta para cualquier sistema que no pueda clasificar con seguridad.

## Puntos clave

- La Ley de IA de la UE clasifica la IA por riesgo —prohibido, alto riesgo, transparencia, mínimo— y cuanto mayor es el riesgo, más debes hacer.
- El empleo y los servicios esenciales como el crédito y los seguros son de alto riesgo; perfilar a una persona hace siempre de alto riesgo un uso del Anexo III.
- Siete prácticas están prohibidas por completo, incluido el reconocimiento de emociones en lugares de trabajo y escuelas, y conllevan las multas más pesadas de la ley digital europea.
- La ley se encendió por etapas: las prohibiciones y el deber de alfabetización en IA ya están vigentes, y los deberes de alto riesgo llegan en 2026 y 2027.
- Como responsable de la implantación aún cargas con deberes reales —supervisión, transparencia, alfabetización y documentación—, y el cumplimiento es el suelo, no el fin de tu responsabilidad.
