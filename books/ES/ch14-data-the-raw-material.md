# Capítulo 14 — Datos: la materia prima

## En palabras simples

La IA no piensa por sí sola. Funciona con datos, igual que una cocina funciona con ingredientes. La calidad del plato depende de la calidad de lo que pones. Ningún chef, por hábil que sea, puede hacer un buen plato con verduras podridas. La IA es igual: buenos datos entran, resultados útiles salen; malos datos entran, resultados inútiles o dañinos salen.

Esta es la verdad más importante sobre la IA que los dueños de negocio pasan por alto. Se enfocan en el modelo —qué tan listo es, qué marca comprar— e ignoran los datos sobre los que funciona. Pero el modelo es solo el chef. Los datos son la comida. La mayoría de los proyectos de IA fallan no porque el modelo fuera débil, sino porque los datos eran desordenados, incompletos o incorrectos.

Datos, en palabras simples, es información registrada. Nombres de clientes, historiales de pedidos, facturas, correos, hojas de cálculo, registros de empleados, clics en el sitio web, lecturas de máquinas —todo datos. Algo de ello está ordenado, sentado en tablas prolijas. La mayoría está desordenado, disperso por archivos, bandejas de entrada y papel. Tu trabajo es saber qué tienes, dónde está, y si es suficientemente bueno para construir sobre él.

Este capítulo trata de tratar tus datos como la materia valiosa que son. Cubre qué datos tienes y dónde viven, cómo saber si están limpios y al día, las reglas básicas para datos personales, cómo mantenerlos seguros, y cómo organizarlos sin patas arriba todo tu negocio. El tratamiento legal profundo de la privacidad está en el [Capítulo 10](ch10-privacy-and-gdpr.md); este capítulo te da los fundamentos de trabajo para que prepares tus datos para la IA.

Una imagen simple para llevar: antes de cocinar, revisas la despensa. Encuentras lo que tienes, tiras lo que está echado a perder, y anotas lo que falta. Eso es exactamente lo que haces con los datos antes de cualquier proyecto de IA.

## Un poco de historia

**Años 60 y 70: los datos viven en bases de datos.** Las empresas guardaban información en bases de datos estructuradas —tablas prolijas de números y texto corto—. Esto era limpio por diseño, pero cubría solo una pequeña porción de lo que el negocio sabía. La mayor parte del conocimiento vivía en papel o en la cabeza de las personas.

**Años 80 y 90: hojas de cálculo y archivos.** Las computadoras personales esparcieron los datos por todas partes. Hojas de cálculo, unidades compartidas, adjuntos de correo. Los datos se volvieron abundantes pero dispersos e inconsistentes. El desorden que todos conocemos hoy empezó aquí.

**Años 2000: "big data".** Internet y los sistemas digitales produjeron datos a una escala que nadie había visto. Las empresas empezaron a hablar de "big data" como un activo. Pero el volumen sin calidad creó un nuevo problema: océanos de datos, poca de ello fiable.

**Años 2010: la calidad de los datos se vuelve el cuello de botella.** A medida que crecían la analítica y el aprendizaje automático, surgió una verdad dura: la mayoría de los proyectos pasaban el 80% de su tiempo limpiando datos, no modelándolos. "Basura entra, basura sale" se convirtió en la lección definitoria de la era. La preparación de datos, no los algoritmos ingeniosos, era el trabajo real.

**2018: el RGPD eleva la apuesta.** La ley de privacidad de Europa hizo del manejo de datos un deber legal, no solo un tema de calidad. Ahora los datos desordenados no eran solo inútiles; los datos personales maltratados eran punibles. El gobierno de datos se volvió un tema de consejo de administración.

**Años 2020: la IA generativa hace que el alcance de los datos importe.** La IA moderna puede leer texto e imágenes desordenados, así que necesita datos menos prolijos que los sistemas viejos. Pero sigue dependiendo de tener los datos correctos disponibles y fiables. La lección se mantiene: el modelo es solo tan bueno como lo que le das.

El arco es claro. Pasamos de muy pocos datos estructurados a demasiados datos dispersos. La habilidad nunca cambió: encontrarlos, limpiarlos y saber en qué puedes confiar.

## Curiosidad

### 14.6 El modelo que escribía Python desde libros de los años 30

Aquí hay un hecho llamativo sobre cómo los datos dan forma a lo que un modelo puede hacer: investigadores entrenaron un modelo de lenguaje solo con libros de antes de 1931 —sin computadoras, sin internet y sin código de programación, porque Python aún no existía— y aun así podía escribir un poco de Python, copiando la estructura de los ejemplos puestos delante de él.

Ese experimento, y lo que enseña sobre datos y estructura, se cuenta por completo en el [Capítulo 3](ch03-the-words-of-ai-without-the-big-words.md), el hogar canónico del mismo. El punto para este capítulo es una línea: **lo que un modelo puede hacer depende por completo de lo que se le dio.** Cambia los datos, y cambias la capacidad. Por eso tus propios datos son la materia prima que vale la pena cuidar.

## Un ejemplo real de negocio

### El mayorista cuyos "datos" eran tres hojas de cálculo en conflicto

Un mayorista de materiales de construcción creía que tenía buenos datos de clientes. Cuando intentó usar IA para predecir qué productos pediría cada cliente, el proyecto se estancó en la primera semana. La razón fueron los datos, no el modelo.

La información de clientes vivía en tres lugares: un viejo sistema de contabilidad, una hoja de cálculo de ventas que llevaba un comercial, y una lista de correo en un programa de email. El mismo cliente aparecía tres veces con tres grafías y direcciones distintas. Los historiales de pedidos no coincidían entre sistemas. La mitad de los registros no tenía teléfono. Los datos no eran exactamente incorrectos —estaban fragmentados e inconsistentes, lo cual es igual de malo—.

La solución no fue de alta tecnología. Eligieron un sistema como única fuente de verdad para los registros de clientes. Fusionaron los duplicados a mano. Fijaron una regla simple: cada cliente nuevo entra en el único sistema, una vez. Llevó unas semanas de trabajo poco glamuroso. Después de eso, el proyecto de predicción funcionó, porque por primera vez había un conjunto fiable de datos sobre el que construir.

La lección: la IA estaba lista. Los datos no. La mayoría de los proyectos de IA esperan por los datos, no por las herramientas.

## Cómo hacerlo

### 14.1 Qué datos tienes y dónde están

No puedes usar lo que no puedes encontrar. El primer paso es un inventario de datos: una lista simple de cada lugar donde tu negocio guarda información.

Recorre tu negocio y enumera cada fuente de datos. Las típicas:

- **Sistemas de negocio.** Software de contabilidad, CRM, inventario, plataforma de comercio electrónico, sistema de RRHH.
- **Archivos y hojas de cálculo.** Unidades compartidas, portátiles personales, Google Drive, archivos de Excel.
- **Correo y mensajes.** Bandejas de entrada, herramientas de chat, hilos guardados.
- **Papel.** Archivos físicos, formularios firmados, notas.
- **Web y rastros digitales.** Analítica del sitio web, registros de aplicaciones, actividad del portal de clientes.
- **Datos externos.** Feeds de proveedores, datos de mercado, registros públicos.

Para cada fuente, anota cuatro cosas: qué guarda, quién es su dueño, aproximadamente cuánto hay, y qué tan actual está. No apuntes a la perfección; apunta a un mapa. Quieres ver todo el panorama para saber dónde están los buenos datos y dónde están los huecos.

Espera sorpresas. La mayoría de los dueños descubren datos que olvidaron que existían y huecos que asumían rellenos. El inventario en sí es valioso porque convierte una vaga sensación de "tenemos datos en algún sitio" en una imagen clara.

Un buen inventario es una tabla. Mantenlo simple y actualízalo sobre la marcha. Se convierte en la referencia para cada futuro proyecto de IA.

### 14.2 Datos limpios, completos y actualizados

Una vez que sabes qué tienes, juzga su calidad. Los buenos datos tienen tres cualidades.

**Limpio.** Libre de errores, duplicados e inconsistencias. El mismo cliente no está escrito de tres maneras. Los números son realmente números, no texto. Las fechas son fechas reales. Limpiar significa arreglar o eliminar los malos registros.

**Completo.** Tiene los campos que necesitas rellenos. Si necesitas la región de un cliente para predecir la demanda, pero la mitad de los registros no tiene región, los datos son incompletos. Completitud significa que los campos importantes están rellenos.

**Actualizado.** Refleja la realidad ahora, no hace tres años. Una lista de clientes donde la mitad de las empresas se han mudado o cerrado está rancia. Los datos rancios llevan a conclusiones erróneas, no importa qué limpios que parezcan.

Cómo comprobar la calidad sin herramientas especiales:

- **Muestreo.** Saca 20 registros al azar y busca errores, duplicados y huecos. La tasa de error que ves es aproximadamente la tasa de error que tienes.
- **Cuenta los huecos.** Para los campos que necesitas, ¿qué proporción están vacíos? Muchos huecos significan baja completitud.
- **Revisa las fechas.** ¿Cuándo se actualizó por última vez cada fuente? Viejo significa rancio.

No necesitas datos perfectos. Necesitas datos suficientemente buenos para la tarea específica. Una predicción aproximada tolera más ruido que una factura de cliente. Ajusta el listón de calidad al trabajo. Pero sabe dónde estás antes de construir.

Limpiar es trabajo real y a menudo tedioso. Presupuesta para ello. Es el 80% del proyecto que todos olvidan planificar.

### 14.3 Datos personales y RGPD: reglas básicas

Algunos de tus datos son datos personales —cualquier información sobre una persona viva que pueda ser identificada: nombres, correos, teléfonos, direcciones, IDs de cliente, incluso una dirección IP—. Los datos personales llevan deberes legales, y el tratamiento completo está en el [Capítulo 10](ch10-privacy-and-gdpr.md). Aquí están los fundamentos de trabajo que necesitas antes de usarlos con IA.

**Sabe qué es personal.** Marca, en tu inventario, cada fuente que guarda datos personales. No puedes proteger lo que no has identificado.

**Ten una razón legal.** Bajo el RGPD, solo puedes tratar datos personales sobre una base legal válida —por ejemplo, un contrato con la persona, su consentimiento, o un interés legítimo que no anule sus derechos—. Sabes en qué base te apoyas antes de meter los datos en la IA.

**Usa solo lo que necesitas.** No viertas todos tus datos personales en una herramienta de IA cuando la tarea solo necesita un poco. Minimiza lo que usas.

**Vigila a dónde va.** Si envías datos personales a un servicio de IA de terceros, los datos salen de tu control y el RGPD los sigue por la puerta. El manejo del proveedor se vuelve tu responsabilidad. Los riesgos de terceros están en el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).

**Respeta los derechos de las personas.** Las personas pueden pedir ver, corregir o borrar sus datos. Tu uso de la IA no debe hacer eso imposible.

Esta es una guía clara, no asesoramiento legal. Para decisiones reales, especialmente a través de fronteras, consulta a un profesional de protección de datos. Pero el hábito —marcar datos personales, conocer tu base, usar el mínimo— es tuyo para construirlo ahora.

### 14.4 Seguridad, copia de seguridad y acceso

Los datos son un activo, y los activos necesitan protección. Tres fundamentos cubren la mayor parte del riesgo.

**Seguridad.** Protege los datos de atacantes y filtraciones. Usa contraseñas fuertes y autenticación de múltiples factores, mantén los sistemas actualizados, cifra los datos sensibles, y ten cuidado con los adjuntos y enlaces de correo. El panorama de seguridad completo, incluidas las amenazas específicas de la IA, está en el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).

**Copia de seguridad.** Guarda copias de tus datos que estén a salvo del sistema principal. Si un sistema se cae, es golpeado por un ransomware, o se borra un archivo, una copia de seguridad es la diferencia entre un mal día y perder el negocio. Sigue una regla simple: guarda copias en más de un lugar, haz copias con regularidad, y prueba que realmente puedes restaurar. Una copia de seguridad que nunca has probado restaurar es solo una esperanza.

**Acceso.** Controla quién puede ver y cambiar qué. No todos necesitan acceso a todo. Da a las personas el acceso mínimo que su rol requiere. Registra quién accede a datos sensibles. Limitar el acceso limita tanto los accidentes como el robo.

Estos tres funcionan juntos. La seguridad mantiene fuera a los de afuera. La copia de seguridad te salva cuando algo sale mal de todos modos. El acceso limita el daño que cualquier persona o error puede hacer. Ninguno de ellos es opcional.

Un hábito práctico: haz copias automáticamente, revisa la copia cada mes, y revisa quién tiene acceso cada trimestre. Pequeñas rutinas, repetidas, previenen desastres.

### 14.5 Cómo organizar los datos sin dar la vuelta a todo

El mayor miedo sobre el trabajo con datos es que signifique una revisión enorme y disruptiva. No es así. Puedes mejorar tus datos paso a paso sin detener el negocio.

**Elige una fuente de verdad por cosa.** Para cada tipo importante de dato —clientes, productos, pedidos— elige un sistema para que sea el oficial. Todo lo demás se vuelve una copia o una vista. Esta sola regla arregla la mayor confusión sin cambiar tus herramientas.

**Arregla en el punto de entrada.** El momento más barato para limpiar datos es cuando se crean. Fija reglas simples para que los nuevos registros vayan al lugar correcto, una vez, con los campos clave rellenos. Detener el desorden nuevo gana a limpiar el desorden viejo para siempre.

**No intentes beberse el océano.** No intentes limpiarlo todo. Limpia solo los datos que tus primeros proyectos de IA necesitan. Datos perfectos que nunca usas son esfuerzo desperdiciado. Una limpieza dirigida que sirve a un proyecto real vale la pena hacerla.

**Estandariza un poco, no perfectamente.** Acuerda unos pocos formatos simples —cómo escribir una fecha, un teléfono, un nombre de cliente— y aplícalos de aquí en adelante. No necesitas un gran estándar, solo consistencia para los campos que importan.

**Mejora sobre la marcha.** Trata la calidad de los datos como un hábito, no un proyecto. Cada pequeña corrección hace el siguiente uso de IA más fácil. En un año, pequeñas mejoras constantes se suman a una base de datos sólida.

La mentalidad: no estás reconstruyendo la casa. Estás ordenando la despensa, estante por estante, para que el próximo plato sea más fácil de cocinar. Empieza con el estante que tu primer proyecto necesita.

## Ética y responsabilidad

Los datos llevan peso ético más allá de la calidad y la ley.

**Los datos personales son personas.** Detrás de cada registro hay una persona con derechos y sentimientos. Mánégalo teniendo eso en mente, no solo como un recurso que extraer. Los principios están en el [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md).

**El sesgo vive en los datos.** Si tus datos representan poco a algún grupo, la IA entrenada con ellos tratará mal a ese grupo. Un conjunto de datos de contratación con mayormente un tipo de candidato sesgará a la IA de la misma manera. Revisa los datos de quién faltan, no solo si los datos están limpios.

**No uses datos que la gente no esperaba.** El hecho de que guardes datos no significa que debas usarlos para cualquier propósito. Usar datos de clientes de una forma a la que nunca acordaron rompe la confianza, incluso si es legal. Mantente dentro de las expectativas razonables.

**Sé honesto sobre qué recoges y por qué.** Di a las personas qué datos reúnes y cómo los usas. La recolección oculta es una ruptura de confianza y a menudo de la ley.

**Protégelo como si fuera tuyo.** Una brecha daña a personas reales, no solo a tu reputación. Trata la seguridad como un deber hacia las personas en tus datos, no solo una casilla para marcar.

## Errores a evitar

### 14.7 Errores comunes con los datos

1. **Ignorar los datos hasta que el proyecto falla.** El error más común. Revisa tus datos antes de empezar, no después de que se estanque.
2. **Suponer que tienes datos cuando tienes fragmentos.** Tres hojas de cálculo en conflicto no son un conjunto de datos. Encuentra la verdad primero.
3. **Confundir volumen con calidad.** Muchos datos no son buenos datos. Un pequeño conjunto limpio gana a uno grande desordenado.
4. **No planificar el tiempo de limpieza.** La preparación de datos es la mayor parte del trabajo. Presupuesta para ello o el proyecto se retrasa.
5. **Sin única fuente de verdad.** Múltiples versiones "oficiales" garantizan confusión. Elige una.
6. **Usar datos personales sin una base legal.** Un riesgo legal y un riesgo de confianza. Conoce tu base primero.
7. **Enviar datos personales a IA de terceros sin cuidado.** El RGPD sigue a los datos por la puerta.
8. **Copias de seguridad sin probar.** Una copia que no puede restaurar no es una copia. Pruébala.
9. **Todos tienen acceso a todo.** El acceso amplio significa riesgo amplio. Limítalo al rol.
10. **Intentar limpiarlo todo a la vez.** Parálisis por revisión. Limpia solo lo que tu proyecto necesita.
11. **Ignorar los datos rancios.** Los datos limpios pero viejos siguen dando respuestas equivocadas. Revisa las fechas.
12. **Olvidar el sesgo en los datos.** Un hueco en quién está representado se vuelve un sesgo en el resultado.

## Ejercicio práctico

### 14.8 Inventario de datos

Pasa una tarde construyendo un inventario de datos simple. Esta es la preparación más útil que puedes hacer para la IA.

Haz una tabla con una fila por fuente de datos. Para cada una, rellena:

- **Fuente** —el sistema, archivo o lugar (p. ej., "software de contabilidad", "hoja de cálculo de ventas", "bandeja de entrada de correo")—.
- **Qué guarda** —clientes, pedidos, facturas, currículums, etc.—.
- **Dueño** —quién es responsable de ello—.
- **Volumen** —aproximadamente cuánto (filas, archivos, GB)—.
- **¿Datos personales?** —Sí / No—.
- **Calidad** —muestrea 20 registros; anota huecos, duplicados, errores. Califícalo limpio / mixto / pobre—.
- **¿Actual?** —cuándo se actualizó por última vez—.
- **¿Fuente de verdad única?** —Sí / No / candidata—.

Rellena cada fuente que puedas encontrar. Cuando termines, mira el panorama:

- ¿Qué fuentes están limpias y actualizadas? Esas son tu mejor material de partida.
- ¿Cuáles guardan datos personales? Márcalas para los fundamentos del RGPD en 14.3.
- ¿Dónde tienes duplicados sin una única fuente de verdad? Esos son tus primeros objetivos de limpieza.
- ¿Qué falta que tu primer proyecto de IA necesita? Esos son huecos a rellenar.

Esta tabla te dice, honestamente, si estás listo para empezar un proyecto de IA o necesitas arreglar los datos primero. Guárdala y actualízala. Es la lista de la despensa para todo lo que construyas después.

## Lista de comprobación

### 14.9 Lista de comprobación de datos

Antes de meter datos en cualquier proyecto de IA, comprueba esto.

- [ ] **Tienes un inventario de datos** que enumera cada fuente y qué guarda.
- [ ] **Sabes dónde están los buenos datos** y dónde están los huecos.
- [ ] **Tienes una única fuente de verdad** para cada tipo clave de dato.
- [ ] **Has muestreado la calidad** y conoces la tasa de error y de huecos.
- [ ] **Los datos están suficientemente limpios para la tarea específica** que estás haciendo.
- [ ] **Los datos están actualizados** y reflejan la realidad actual.
- [ ] **Has marcado todos los datos personales** en el inventario.
- [ ] **Tienes una base legal** para cualquier dato personal que uses (ver [Capítulo 10](ch10-privacy-and-gdpr.md)).
- [ ] **Usas solo el mínimo de datos personales** que la tarea necesita.
- [ ] **Sabes a dónde van los datos** si un servicio de IA de terceros los toca.
- [ ] **Los fundamentos de seguridad están en su lugar** —autenticación fuerte, actualizaciones, cifrado para datos sensibles—.
- [ ] **Las copias de seguridad existen, son recientes, y se han probado para restaurar.**
- [ ] **El acceso está limitado** a los roles que lo necesitan, con registro en datos sensibles.
- [ ] **Estás arreglando los datos nuevos en el punto de entrada**, no solo limpiando datos viejos.
- [ ] **Has comprobado el sesgo** —¿los datos de quién faltan?—.

Si una casilla está vacía y tu proyecto depende de ella, arréglalo antes de construir. Los buenos datos no son un detalle; son la materia prima sobre la que funciona todo lo demás.

## Puntos clave

- Los datos son la materia prima de la IA: buenos datos entran, resultados útiles salen; malos datos entran, resultados inútiles o dañinos salen —el modelo es solo el chef—.
- Empieza con un inventario de datos: no puedes usar lo que no puedes encontrar, y la mayoría de los dueños se sorprenden por lo que tienen y lo que falta.
- La calidad significa limpio, completo y actualizado; planifica el tiempo de limpieza, porque es la mayor parte del trabajo que todos olvidan.
- Los datos personales llevan deberes legales —márcalos, conoce tu base legal, usa el mínimo, y recuerda que el RGPD los sigue a cualquier servicio de terceros—.
- Puedes mejorar los datos paso a paso sin una revisión general: elige una fuente de verdad, arregla en el punto de entrada, y limpia solo lo que tu proyecto necesita.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Haz preguntas sobre tus propios archivos

![El agente respondiendo desde tus propios documentos](../../assets/examples/ask-your-documents.png)
*El agente respondiendo desde tus propios documentos*

**Qué preguntas:** `¿Cuál es nuestra política de cancelación con el proveedor de imprenta?`

El agente busca en tu área de documentos y responde con lo que tus propios archivos realmente dicen, apuntando a la fuente.

*Consejo: Mantén tus archivos de negocio en el área de documentos y se convierten en conocimiento buscable.*

---

### Encuentra ese viejo documento

![Una búsqueda en tu archivo indexado](../../assets/examples/find-in-archive.png)
*Una búsqueda en tu archivo indexado*

**Qué preguntas:** `Encuentra la propuesta que envié al hotel la primavera pasada sobre el rediseño del vestíbulo.`

El agente busca en tu archivo indexado y trae de vuelta el documento que querías, incluso cuando solo lo recuerdas a medias.

*Consejo: El índice se actualiza a medida que añades archivos, así que el archivo siempre está al día.*

---

### Recuerda cómo te gustan las cosas

![El agente aplicando tus preferencias guardadas](../../assets/examples/remember-preferences.png)
*El agente aplicando tus preferencias guardadas*

**Qué preguntas:** `Haz una factura —ya sabes cómo me gustan.`

El agente recuerda tu estilo y ajustes de antes y los aplica sin que tengas que repetirlo.

*Consejo: Puedes corregirlo en cualquier momento; actualiza lo que recuerda.*

---

### Nada se pierde jamás

![El historial de versiones te permite volver con seguridad](../../assets/examples/version-history.png)
*El historial de versiones te permite volver con seguridad*

**Qué preguntas:** `Muéstrame la versión anterior del contrato y restáurala.`

Cada versión que el agente hizo se guarda. Puedes ver el borrador anterior y traerlo de vuelta, así editar es siempre seguro.

*Consejo: Esta es la razón por la que puedes dejar que el agente reescriba cosas libremente —el historial te protege—.*

<!-- END agentbridge-examples -->
