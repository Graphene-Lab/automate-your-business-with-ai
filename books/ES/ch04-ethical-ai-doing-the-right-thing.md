# Capítulo 4 — IA ética: hacer lo correcto

## En palabras simples

La IA ética no es una clase de filosofía. Es un conjunto de decisiones prácticas que tomas antes de encender un sistema.

La idea es sencilla. Un sistema de IA toma decisiones, o ayuda a las personas a tomarlas. Esas decisiones afectan a personas reales: clientes, empleados, candidatos, pacientes. Cuando una máquina influye en la vida de alguien, alguien debe responder por ello. Ese alguien eres tú, la empresa que decidió usarla.

Muchos dueños ven la ética como un lujo. Algo para las grandes empresas con equipos legales, o una frase de relleno para el informe anual. Este capítulo sostiene lo contrario. La ética es una necesidad, por tres razones simples.

Primero, **la IA poco ética cuesta dinero**. Una herramienta de contratación sesgada, un chatbot que miente, un sistema que filtra datos privados: cada uno puede terminar en una demanda, una multa o una pérdida pública de confianza que tarda años en repararse.

Segundo, **la IA poco ética suele ser mala IA**. Una herramienta que discrimina es también una herramienta que descarta buenos candidatos. Una herramienta que no puede explicarse es también una herramienta que no puedes depurar. La corrección ética y la corrección de calidad suelen ser la misma corrección.

Tercero, **la ley ya lo exige**. En la Unión Europea, las normas sobre alfabetización en IA y sobre sistemas de alto riesgo ya están en vigor o llegan según un calendario fijo. El [Capítulo 5](ch05-rules-and-legal-responsibility.md) cubre esas normas en detalle. Este capítulo cubre el razonamiento que hay detrás.

Una idea recorre todo lo que aquí se dice: **no puedes cederle a una máquina tu responsabilidad, pero sí puedes cederle tu trabajo.** La máquina hace el esfuerzo pesado. Tú conservas el juicio, la supervisión y la culpa.

## Un poco de historia

La ética y la tecnología se han encontrado muchas veces antes, y cada encuentro produjo una regla.

En 1942 el escritor Isaac Asimov publicó sus "Tres leyes de la robótica" en un cuento de ciencia ficción: un robot no puede dañar a un humano, debe obedecer las órdenes y debe protegerse a sí mismo, en ese orden. Las leyes son ficción, pero plantearon una pregunta real que aún impulsa este campo: ¿cómo haces que una máquina se comporte bien?

La conversación moderna y seria comenzó en **2017 en Asilomar**, California. Investigadores en inteligencia artificial se reunieron y escribieron una larga lista de principios para una IA segura y beneficiosa. No era una ley. Era una advertencia de las mismas personas que construían la tecnología: esa tecnología necesitaba barreras de contención.

El trabajo institucional llegó rápido. El **IEEE**, un organismo profesional de ingenieros, inició un proyecto sobre diseño ético de sistemas autónomos. La **OCDE** publicó principios acordados sobre IA en 2019. En 2021 la **UNESCO** adoptó una recomendación mundial de ética, aprobada por 193 países. La Unión Europea pasó de los principios a las reglas obligatorias: en 2018 formó un grupo de expertos cuya lista de "IA confiable" se convirtió en la base de la Ley de IA de la UE.

Fíjate en la forma de esta historia. Pasó de los cuentos, a los principios, a las listas de verificación, a la ley. Cada paso hizo más concreto y más exigible el anterior. Hoy una pequeña empresa está al final de esa línea. El debate abstracto terminó. Lo que queda es un conjunto de expectativas que se espera que cumplas.

## Curiosidad

### 4.7 La ley ahora exige que tu personal entienda la IA

Aquí hay un dato que sorprende a la mayoría de los dueños. Desde el **2 de febrero de 2025**, una empresa europea que usa IA tiene el deber legal de asegurarse de que su gente la entienda.

Esto viene del **Artículo 4 de la Ley de IA de la UE**, que trata de la "alfabetización en IA". En palabras simples, la ley dice que los proveedores y los responsables de la implantación de sistemas de IA deben tomar medidas para garantizar, en la mayor medida posible, un nivel suficiente de alfabetización en IA entre su personal y cualquier persona que opere un sistema de IA en su nombre.

Un **responsable de la implantación** es simplemente una empresa que usa un sistema de IA, a diferencia de un **proveedor** que lo construye. La mayoría de las pequeñas y medianas empresas son responsables de la implantación. Eso significa que el Artículo 4 se aplica a ti aunque nunca escribas una línea de código.

La ley es cuidadosa con lo que significa "suficiente". Debe adaptarse al conocimiento técnico, la experiencia y la educación de cada persona, y al contexto donde se usa la IA y a las personas a las que afecta. Un agente de atención al cliente que usa un chatbot necesita un nivel de comprensión distinto al del gerente que aprueba su uso.

Lo crucial es que la ley establece que esta obligación **no te exige garantizar ningún nivel específico de alfabetización para ninguna persona en particular.** Es un deber de esfuerzo, no una promesa de resultado. Debes demostrar que tomaste medidas razonables: formación, orientación, roles claros. No tienes que certificar que todos aprobaron un examen.

¿Por qué es interesante esto para un dueño de negocio? Porque convierte la "ética de la IA" de un valor vago en una tarea concreta con fecha límite. Un regulador, un cliente o un tribunal pueden preguntarte: "¿qué hiciste para asegurarte de que tu gente entendiera la IA que pusiste frente a ellos?". "La compramos y cruzamos los dedos" no es una respuesta. Una sesión breve de formación, una política escrita y un responsable con nombre sí lo son. El deber de alfabetización es la parte más barata del cumplimiento y la de efecto más amplio: un personal que entiende que un modelo puede equivocarse es un personal que detecta los problemas a tiempo.

## Un ejemplo real de negocio

### La herramienta de contratación que aprendió a despreciar a las mujeres

En julio de 2018 la agencia de noticias Reuters informó de que Amazon había construido un sistema de IA para filtrar solicitudes de empleo y tenía un defecto grave: favorecía a los hombres.

La historia es una lección limpia sobre el sesgo. Amazon entrenó la herramienta con diez años de currículums que había recibido. Durante la mayor parte de esos años, la mayoría de los candidatos a puestos técnicos eran hombres. El sistema aprendió, a partir de esa historia, que "un buen candidato" se parecía a los candidatos que ya había contratado: sobre todo hombres.

Fue más allá de las señales evidentes. Empezó a penalizar los currículums que contenían la palabra "mujeres", como en "capitana del club de ajedrez femenino". Rebajó a las graduadas de dos universidades solo de mujeres. Premió un lenguaje más común en los currículums de hombres, como "ejecuté" y "logré", y castigó las frases más suaves más comunes en los de las mujeres.

Los ingenieros de Amazon intentaron arreglarlo. Eliminaron los términos vinculados al género. Pero el sistema seguía encontrando otros sustitutos: señales indirectas que hacían las veces del género. No podían estar seguros de que la herramienta fuera justa. Amazon terminó por disolver el equipo y dejó de usar el sistema como su filtro principal.

Dos lecciones destacan.

Primera, **el sesgo no estaba en el código. Estaba en los datos.** Nadie escribió "prefieran a los hombres". El modelo absorbió un desequilibrio del pasado y lo reprodujo a gran escala. Un reclutador humano con el mismo prejuicio afecta a unos pocos candidatos. Un modelo con ese prejuicio afecta a todos los candidatos, al instante, y parece objetivo mientras lo hace.

Segunda, **la empresa lo detectó antes de causar un desastre público** y decidió detenerse. Esa fue la jugada ética, y también la sensata. Una herramienta que rechaza en silencio a buenos candidatos por su género pierde talento y se expone a una demanda por discriminación. La corrección ética y la corrección de negocio apuntaban en la misma dirección. Si usas IA para clasificar, filtrar, puntuar u ordenar personas de cualquier forma, la misma trampa se aplica.

## Cómo hacerlo

### 4.3 Los seis principios para una adopción responsable

Los marcos de trabajo solo son útiles si puedes actuar sobre ellos. Estos seis principios están ordenados de modo que cada uno responde a una pregunta que debes resolver realmente antes y durante un proyecto.

**Principio 1: Decide quién es el responsable.** Antes que nada, nombra a una persona. No un equipo, no un proveedor: un ser humano con nombre propio que sea dueño de este sistema de IA y responda por sus resultados. Si no puedes nombrar a esa persona, no estás listo para implantar. La responsabilidad que es de todos, no es de nadie.

**Principio 2: Comprende los impactos y planifica.** Anota a quién toca este sistema y cómo. ¿A quién se aplica? ¿Qué decide sobre esas personas? ¿Cuál es el peor daño realista? Un bot de atención al cliente que da una respuesta equivocada sobre un reembolso molesta a alguien. Una herramienta de crédito que rechaza por error a un solicitante le niega dinero. Planifica para el peor caso, no solo para el caso promedio.

**Principio 3: Mide y gestiona los riesgos.** Un riesgo que no puedes ver es un riesgo que no puedes arreglar. Decide cómo probarás el sistema antes del lanzamiento y cómo lo vigilarás después. Revisa una muestra de sus decisiones. Registra las quejas. Fija un umbral que active una revisión humana. La medición convierte una esperanza en un control.

**Principio 4: Sé transparente y explicable.** Las personas deben saber cuándo están tratando con IA, y deben poder obtener una razón clara de una decisión que las afecta. "Lo dijo el modelo" no es una razón. Si no puedes explicar una decisión en una frase, no deberías dejar que esa decisión se sostenga sola. Ver la sección 4.5.

**Principio 5: Protege la privacidad y los datos.** Los datos personales son el combustible de la mayoría de las IA. Trátalos con cuidado: recoge solo lo que necesitas, sabe a dónde van y nunca introduzcas detalles de clientes en una herramienta que no hayas revisado. El aspecto legal se cubre en el [Capítulo 10](ch10-privacy-and-gdpr.md); el de seguridad, en el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).

**Principio 6: Mantén a los humanos al mando.** Para cualquier decisión que importe, un humano debe poder revisar, anular y detener el sistema. "Humano en el bucle" significa que el humano es un verdadero tomador de decisiones, no un sello de goma. Diseña el flujo de trabajo para que una persona pueda decir que no, y para que decir que no sea fácil y esperado.

Usa estos seis como lista de verificación en cada proyecto. Si no puedes cumplir uno, detente y arréglalo antes de seguir. Son baratos de aplicar al principio y caros de añadir después.

## Ética y responsabilidad

### 4.1 Por qué la ética no es un lujo sino una necesidad

Trata la ética como un centro de costos y la recortarás. Trátala como control de riesgo y no lo harás. Aquí está el argumento honesto de negocio.

**El riesgo de equivocarse es grande y concreto.** Las denuncias por discriminación, las filtraciones de datos, las multas por resultados engañosos y el daño reputacional cuestan dinero real y tiempo real. Un solo sistema sesgado que tome la decisión equivocada sobre un grupo protegido puede desencadenar investigaciones sobre todos los casos que tocó.

**La ventaja de hacerlo bien es operativa, no solo moral.** Los sistemas explicables son más fáciles de depurar. Los sistemas justos amplían tu grupo de candidatos y clientes en lugar de reducirlo. La disciplina con los datos privados reduce tu exposición a las filtraciones. El diseño ético y el buen diseño se solapan casi por completo.

**La confianza es tu producto real.** Las pequeñas empresas ganan por confianza. Un cliente que cree que tratas sus datos y su solicitud con justicia es un cliente que vuelve. Un cliente que sospecha que una caja negra tomó una decisión fría e inexplicable sobre él, no. La ética es la forma de conservar la confianza de la que dependen las empresas pequeñas y que a las grandes a menudo falta.

Así que la ética no es una decoración que añades cuando te sobra presupuesto. Es el suelo que sostiene todo. Saltártela no es ahorrar dinero; es pedir prestados problemas a un interés muy alto.

### 4.2 Los cuatro pilares de la gobernanza ética

¿Cómo haces que la ética se sostenga en toda una empresa, y no solo en un proyecto? La gobernanza se apoya en cuatro pilares. Quita uno y la estructura se ladea.

**Pilar 1: Principios.** Una breve declaración escrita de lo que tu empresa cree sobre la IA: justicia, honestidad, control humano, privacidad. Esta es tu brújula interna. Debe caber en una página y la debe leer todo el que toque la IA. Los principios sin los otros tres pilares son carteles en una pared.

**Pilar 2: Regulación.** Las reglas externas que debes cumplir: la Ley de IA de la UE, el RGPD, la ley de protección al consumidor, la ley antidiscriminación. Tú no las eliges; se aplican a ti. El [Capítulo 5](ch05-rules-and-legal-responsibility.md) es el hogar profundo de la Ley de IA, y el [Capítulo 10](ch10-privacy-and-gdpr.md) del RGPD. Sabe qué reglas atan tus casos de uso.

**Pilar 3: Estándares técnicos.** Las formas acordadas de construir y probar que convierten los principios en práctica: pruebas de sesgo, registro de decisiones, documentación de modelos, estándares de seguridad, gestión de calidad. Los estándares son la forma en que "sé justo" se convierte en "ejecuta esta prueba y registra el resultado". Hacen la ética auditable.

**Pilar 4: Autorregulación.** Lo que haces porque elegiste hacerlo, más allá del mínimo que exige la ley: un comité interno de revisión, un código de conducta, una persona que pueda vetar un uso dañino, la costumbre de preguntar "¿debemos?" y no solo "¿podemos?". La autorregulación es la cultura que llena los huecos que la ley deja.

Una empresa sana tiene los cuatro. Los principios marcan el camino. La regulación fija el suelo. Los estándares lo hacen medible. La autorregulación te mantiene honesto cuando nadie mira.

### 4.4 Sesgo y discriminación: cómo reconocerlos y evitarlos

**Sesgo** es cuando un sistema trata a algunas personas peor que otras de forma sistemática, no por accidente, sino por cómo fue construido o entrenado. Cuando ese patrón coincide con una característica protegida —género, raza, edad, discapacidad, religión y otras—, se convierte en **discriminación** ilegal en muchos lugares.

El sesgo suele entrar por los datos, como mostró el ejemplo de Amazon. Si tus decisiones pasadas favorecieron a un grupo, un modelo entrenado con ellas aprende a favorecer a ese grupo. El modelo es un espejo. Refleja los ejemplos, incluidos sus defectos.

**Cómo reconocerlo.** Haz tres preguntas a cualquier sistema que ordene o puntúe personas:

1. **¿Quién está en los datos de entrenamiento y quién falta?** Si un grupo estuvo históricamente subrepresentado, es probable que el sistema lo atienda peor.
2. **¿El sistema usa sustitutos?** Puedes quitar el campo de género y seguir teniendo sesgo, porque los cargos, las escuelas, los pasatiempos o los huecos en un currículum pueden hacer las veces del género. Busca señales que se correlacionen con un rasgo protegido.
3. **¿Los resultados son desiguales por grupo?** La prueba más simple: toma las decisiones del sistema y agrúpalas por género, edad o etnia. Si un grupo es rechazado a una tasa mucho mayor, investiga por qué. La brecha es la luz de advertencia.

**Cómo evitarlo.** Usa datos que representen a las personas a las que realmente sirves. Prueba los resultados por grupo antes del lanzamiento, no después. Mantén a un humano revisando las decisiones límite. Documenta lo que revisaste, para poder demostrar la debida diligencia. Y recuerda que quitar una etiqueta no quita un sustituto: tienes que buscar las señales indirectas a propósito.

El sesgo no es una falla moral de la máquina. Es una falla de los humanos que eligieron los datos y se saltaron la prueba. Eso es una buena noticia: las fallas humanas se arreglan con procesos humanos.

### 4.5 Transparencia y explicabilidad: por qué importa saber cómo decide la IA

**Transparencia** significa que las personas saben cuándo la IA está involucrada y más o menos qué está haciendo. **Explicabilidad** significa que puedes dar una razón clara de una decisión específica.

Importan por tres razones.

**Confianza.** Una persona acepta más fácilmente una decisión cuando la entiende. "Su solicitud no fue seleccionada porque el puesto requiere X y su perfil muestra Y" es difícil de aceptar pero fácil de entender. "Rechazado por IA" sin razón alguna se siente arbitrario e invita a la ira y a las quejas.

**Control.** No puedes arreglar lo que no puedes ver. Si un modelo toma una mala decisión y nadie puede decir por qué, no puedes corregirla, y volverá a ocurrir. Un sistema explicable te permite rastrear la causa y eliminarla. Uno opaco esconde sus propios defectos hasta que causan daño.

**Ley y justicia.** En varios ámbitos legales, incluido el RGPD para ciertas decisiones automatizadas, una persona tiene derecho a una explicación. Más allá de la ley, una decisión inexplicable sobre una persona es difícil de defender como justa. Si no puedes articular la razón, no puedes probar que no hubo sesgo.

Una regla práctica: **para cualquier decisión que afecte de forma importante a una persona, debes poder producir una razón en una frase que entienda un no experto.** Si no puedes, esa decisión necesita un humano detrás, no una máquina delante de esa persona. Ten cuidado con los proveedores que afirman que su sistema es "totalmente explicable". Pídeles que te lo muestren, en un caso real, durante la reunión. Una afirmación que no puedes ver demostrada es una afirmación en la que no deberías confiar.

### 4.6 Responsabilidad humana: ¿quién responde si la IA comete un error?

Esta es la pregunta que hace todo dueño. La respuesta es simple e incómoda: **tú.**

Un sistema de IA es una herramienta. Las herramientas no cargan con responsabilidad legal; las personas que las usan, sí. Si un repartidor que empleas se salta un semáforo en rojo, tú respondes como empleador. Si una IA que implantas toma una decisión dañina, la misma lógica se aplica. La máquina no puede ser demandada, multificada ni avergonzada. Tú sí.

Algunos puntos que lo hacen concreto:

- **"La IA del proveedor lo hizo" no es una defensa.** Tú elegiste la herramienta, la pusiste frente a las personas y mantuviste o eliminaste la revisión humana. Esas son tus decisiones, y ahí es donde reside la responsabilidad.
- **La automatización no transfiere la responsabilidad; la concentra.** Un humano que toma 50 decisiones al día reparte el riesgo. Un sistema que toma 5.000 decisiones idénticas lo concentra. Una sola regla defectuosa ahora daña a miles a la vez, y esa regla es tuya.
- **La supervisión humana es tu principal protección.** Donde un humano cualificado puede revisar y anular una decisión, tu responsabilidad baja. Donde dejas que el sistema actúe solo en algo importante, tu responsabilidad sube. Mantener a los humanos al mando (Principio 6) no es solo ético; es cómo te proteges.
- **Documentar tu proceso es tu evidencia.** Si te impugnan, querrás demostrar que evaluaste el riesgo, probaste el sesgo, mantuviste un humano en el bucle y actuaste de forma razonable. Un rastro de papel de buen proceso es tu mejor defensa.

La forma limpia de sostener esto: **la IA decide rápido y a gran escala; un humano decide si dejarla, y asume la culpa cuando algo sale mal.** Nunca dejes que la comodidad de la automatización borre esa línea.

## Errores a evitar

**Error 1: Tratar la ética como un paso posterior.** Añádela después del lanzamiento y encontrarás los problemas demasiado tarde y los arreglarás en público.

**Error 2: Asumir que el proveedor se encarga.** El proveedor construye la herramienta; tú la implantas, y la responsabilidad de cómo toca a tu gente es tuya.

**Error 3: Creer que quitar una etiqueta quita el sesgo.** Saca el campo de género y el modelo encuentra un sustituto; busca las señales indirectas a propósito.

**Error 4: Dejar que "lo dijo el modelo" sea la respuesta final.** Si no puedes explicar una decisión en una frase simple, no la dejes sostenerse sola.

**Error 5: Sellar con goma.** Un humano "en el bucle" que siempre está de acuerdo con la IA no es supervisión; haz que la revisión sea real y que decir que no sea fácil.

**Error 6: Saltarse el rastro de papel.** Sin documentación no hay prueba de que actuaste de forma responsable cuando te impugnen.

**Error 7: Confundir una declaración de valores con gobernanza.** Un cartel sobre "IA responsable" sin un responsable con nombre, sin prueba y sin veto es decoración, no gobernanza.

**Error 8: Ignorar el deber de alfabetización en IA porque parece blando.** El Artículo 4 es ley desde febrero de 2025; un personal formado es a la vez una respuesta legal y tu control más barato.

## Ejercicio práctico

### 4.8 Evalúa los riesgos éticos de un proyecto de IA en tu empresa

Elige un proyecto de IA que estés considerando, o uno que ya tengas en marcha. Trabájalo en papel. Toma alrededor de una hora y sacará a la luz la mayoría de los riesgos graves.

**Paso 1 — Nombra al responsable.** Escribe un nombre: la persona responsable de este sistema. Si dudas, ese es tu primer hallazgo.

**Paso 2 — Mapea a las personas afectadas.** Enumera cada grupo que el sistema toca: clientes, solicitantes, empleados, otros. Para cada uno, escribe qué decide o influye el sistema sobre ellos.

**Paso 3 — El peor daño realista.** Para la decisión más seria, escribe el peor resultado plausible para una persona real. Sé específico. "A una madre soltera se le niega un crédito para el que califica" es un hallazgo; "un mal resultado" no lo es.

**Paso 4 — Prueba de sesgo.** Haz las tres preguntas: quién falta en los datos, qué sustitutos podrían hacer las veces de un rasgo protegido, y si los resultados son desiguales por grupo. Si el sistema ordena personas, debes poder responder las tres.

**Paso 5 — Prueba de explicabilidad.** Toma una decisión que tome el sistema y escribe la razón en una frase que entendería un no experto. Si no puedes, márcalo: esta decisión necesita un humano.

**Paso 6 — Control humano.** Describe exactamente dónde un humano revisa, puede anular y puede apagar el sistema. Si la respuesta es "en ninguna parte", ese es tu arreglo más urgente.

**Paso 7 — Datos y privacidad.** Escribe a dónde van los datos, quién puede verlos y si algún dato personal escapa de tu control. Contrástalo con el [Capítulo 10](ch10-privacy-and-gdpr.md).

**Paso 8 — Alfabetización.** Anota qué personal necesita formación para usar este sistema de forma responsable, y qué harás al respecto.

**Paso 9 — Decide.** Para cada señal de alarma, escribe una acción y un responsable. Un proyecto está listo para avanzar cuando cada daño grave tiene un control y un nombre asociados.

Guarda esta página. Es el primer borrador de tu registro de ética y tu defensa si algún día te lo piden.

## Lista de verificación

### 4.9 Tu política de ética en IA

- [ ] Tengo una declaración de una página con nuestros principios de IA: justicia, honestidad, control humano, privacidad.
- [ ] Cada sistema de IA tiene un único responsable humano con nombre, no un equipo ni un proveedor.
- [ ] Para cada sistema, he mapeado a quién afecta y qué decide sobre ellos.
- [ ] He escrito el peor daño realista para cada decisión seria.
- [ ] Para cualquier sistema que ordene o puntúe personas, he revisado si hay grupos ausentes, sustitutos y resultados desiguales.
- [ ] Para cada decisión que afecta a una persona, puedo producir una razón clara en una frase.
- [ ] Un humano cualificado puede revisar, anular y detener cada decisión importante.
- [ ] Sé a dónde van nuestros datos y quién puede verlos, y nunca doy datos personales a herramientas sin revisar.
- [ ] Tengo un plan para elevar la alfabetización en IA entre el personal que usa nuestros sistemas (deber del Artículo 4).
- [ ] Sé qué reglas externas nos atan: la Ley de IA de la UE, el RGPD, la ley de consumidores y la ley antidiscriminación.
- [ ] Uso estándares técnicos: pruebas, registros, documentación, seguridad.
- [ ] Tengo una costumbre de autorregulación: alguien puede vetar un uso que es legal pero incorrecto.
- [ ] Guardo un registro escrito de la evaluación de riesgos de cada sistema.
- [ ] Entiendo que la empresa, no el proveedor ni la máquina, es responsable de los resultados.
- [ ] Reviso cada sistema periódicamente, no solo en el lanzamiento.

## Puntos clave

- La IA ética es un control práctico de riesgo, no filosofía: ahorra dinero, mejora la calidad y protege la confianza de la que viven las pequeñas empresas.
- La gobernanza se apoya en cuatro pilares —principios, regulación, estándares técnicos y autorregulación— y la estructura se ladea si sueltas uno.
- Los seis principios de adopción ponen un humano con nombre, un plan de daños, una medida de riesgo, una explicación, protección de datos y control humano en cada proyecto.
- El sesgo viene de los datos y se esconde en los sustitutos; lo eliminas probando los resultados por grupo, no borrando una etiqueta.
- La responsabilidad nunca se transfiere a la máquina ni al proveedor: la empresa que implanta un sistema de IA es dueña de sus resultados, y un humano en el bucle más un rastro de papel son tu mejor protección.
