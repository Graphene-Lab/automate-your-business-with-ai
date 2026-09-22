# Capítulo 10 — Privacidad y RGPD: lo que realmente necesitas saber

## En palabras simples

RGPD significa Reglamento General de Protección de Datos. Es el reglamento de la Unión Europea para manejar datos personales —cualquier información sobre una persona viva que pueda ser identificada—. Es una de las leyes de privacidad más estrictas del mundo, y afecta a muchas más empresas de las que la mayoría de los dueños espera.

Toda la ley puede reducirse a una idea: **si guardas información sobre una persona, debes tratarla de forma justa, por una razón clara, guardar solo lo que necesitas, mantenerla segura y respetar lo que esa persona te pida hacer con ella.**

Te afecta si estás en la UE, y también si estás fuera de la UE pero ofreces bienes o servicios a personas en la UE, o vigilas su comportamiento. Una pequeña tienda online en otro país que vende a clientes en Francia está dentro del alcance del RGPD. Esto se llama alcance extraterritorial, y sorprende a muchos negocios.

¿Por qué importa esto para la IA? Porque la IA funciona con datos, y gran parte de esos datos son personales. Nombres de clientes, correos de soporte, currículums, registros de empleados, visitantes del sitio web —todo datos personales. Cuando introduces cualquiera de ellos en una herramienta de IA, estás tratando datos personales, y las reglas se aplican. Si envías esos datos a un servicio de terceros, las reglas lo siguen por la puerta. Ese es el enlace con el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).

Este capítulo es el hogar profundo del RGPD en este libro. Explica los principios, los tipos de datos, las bases legales, tus obligaciones y los derechos que las personas tienen sobre ti. La Ley de IA de la UE —una ley separada sobre los propios sistemas de IA— se trata por completo en el [Capítulo 5](ch05-rules-and-legal-responsibility.md); aquí solo miramos dónde toca la privacidad. El lado de seguridad para proteger los datos está en el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).

Una nota honesta: esta es una guía clara, no asesoramiento legal. Para decisiones reales, especialmente a través de fronteras, habla con un profesional de protección de datos.

## Un poco de historia

**1995: la primera regla de la UE.** La Directiva de Protección de Datos fijó estándares tempranos en toda Europa, pero cada país la implementó de forma distinta, creando un mosaico.

**27 de abril de 2016: se adopta el RGPD.** La UE reemplazó el mosaico con un solo reglamento, diseñado para aplicarse igual en cada estado miembro y modernizar las reglas para la era de internet.

**25 de mayo de 2018: el RGPD se aplica.** Esta es la fecha que importa. Desde este día, las reglas estuvieron plenamente en vigor, con multas cuantiosas por brechas graves. Empresas de todo el mundo tuvieron que cumplirlas o arriesgarse a ellas.

**2018 a 2023: la era de la aplicación.** Las autoridades nacionales de protección de datos emitieron multas, algunas muy grandes, por brechas y malas prácticas. La privacidad se convirtió en un tema de consejo de administración, no solo un problema de abogados.

**2018: el CEPD.** Se creó el Comité Europeo de Protección de Datos para coordinar las autoridades nacionales y emitir orientación para que la ley se aplique de forma coherente en toda la UE. Su orientación es a donde miras cuando la ley no está clara.

**1 de agosto de 2024: entra en vigor la Ley de IA de la UE.** Una ley separada, el Reglamento (UE) 2024/1689, comenzó su despliegue por fases. Regula los sistemas de IA por riesgo. No reemplaza al RGPD. Donde un sistema de IA usa datos personales, ambas leyes se aplican a la vez.

## Curiosidad

### 10.9 Lo que los reguladores de privacidad de Europa dijeron sobre los modelos de IA

En diciembre de 2024 el Comité Europeo de Protección de Datos (CEPD) —el organismo que coordina a todos los reguladores nacionales de privacidad de la UE— adoptó la **Opinión 28/2024**, sobre la protección de datos personales en el contexto de los modelos de IA. Es la declaración de privacidad más importante hasta ahora sobre cómo encaja la IA con el RGPD.

Unos pocos puntos de ella importan a un dueño de negocio:

**Un modelo puede mirarse en tres etapas.** El CEPD separa la vida de un modelo de IA en desarrollo (entrenarlo), despliegue (ponerlo a trabajar) y uso (personas interactuando con él). Cada etapa puede involucrar datos personales, y cada una tiene sus propias preguntas de privacidad. Esto es útil porque te dice que hagas la pregunta en cada etapa, no solo al principio.

**El interés legítimo puede ser una base legal, pero no es un pase libre.** La opinión dice que una empresa puede apoyarse en el "interés legítimo" para desarrollar o usar un modelo de IA, pero solo si el tratamiento es genuinamente necesario y una prueba de balance muestra que no pesa más que los derechos de las personas. No puedes simplemente declarar un interés e ignorar a las personas involucradas.

**Un modelo solo es "anónimo" si no puedes sacarle datos personales.** Esta es la parte afilada. El CEPD dice que para que un modelo se trate como anónimo —y por tanto fuera del RGPD— debe ser muy improbable que alguien pueda extraer datos personales de él haciéndole preguntas. Si un modelo puede ser engañado para repetir detalles personales que memorizó durante el entrenamiento, no es verdaderamente anónimo, y las reglas de protección de datos siguen mordiendo.

**Los malos datos de entrenamiento pueden seguir al modelo.** La opinión advierte que si un modelo fue entrenado con datos personales tratados ilegalmente, eso puede afectar la legalidad de desplegarlo después, a menos que el modelo haya sido debidamente anonimizado. En palabras llanas: un modelo construido con datos sucios puede quedarse sucio, y usarlo puede arrastrar ese problema a tu negocio.

El mensaje práctico para una pequeña empresa es claro. Cuando eliges un proveedor de IA, la pregunta de privacidad no es solo "qué hacen con mis datos ahora", sino "¿con qué datos fue entrenado este modelo, y pueden sacarse de él datos personales?". Esa pregunta pertenece a tu lista de comprobación de proveedores.

## Un ejemplo real de negocio

### La herramienta de RRHH y la solicitud de acceso

Una empresa mediana con 120 empleados adopta una herramienta de IA para filtrar solicitudes de empleo. Sube currículums y cartas de presentación —todo datos personales, algo de ello sensible, porque los currículums pueden revelar lagunas de salud, edad, nacionalidad y actividad sindical—. La herramienta clasifica a los candidatos.

Tres meses después, una solicitante que fue rechazada escribe a la empresa. Hace una **solicitud de acceso del interesado**: bajo el RGPD tiene derecho a saber qué datos personales guarda la empresa sobre ella y cómo se usaron. La empresa debe responder, normalmente dentro de un mes y sin coste.

Ahora la empresa debe responder preguntas difíciles que nunca se hizo. ¿Dónde están su currículum y la clasificación de la IA? ¿Puede producir los datos y explicar la lógica? ¿Hubo una base legal para tratar su currículum con esta herramienta? ¿Hizo primero una evaluación de riesgos? Si la herramienta era un servicio de terceros, ¿cubrió el contrato todo esto? Si la clasificación de la IA cuenta como toma de decisiones automatizada con un efecto serio sobre ella, se aplican reglas extra, incluido su derecho a no estar sujeta a una decisión puramente automatizada con impacto legal o similarmente significativo.

La empresa se afana porque adoptó la herramienta antes de pensar en los datos. La lección es el orden de las operaciones: debes entender los datos y la base legal **antes** de encender la herramienta, no cuando llega una solicitud. El resto de este capítulo te da las piezas para hacerlo.

## Cómo hacerlo

### 10.1 El RGPD en una página: los principios básicos

El RGPD se apoya en unos pocos principios. Si los respetas, estás respetando la mayor parte de la ley.

**Licitud, equidad y transparencia.** Necesitas una razón legal válida para tratar datos personales, no debes usarlos de formas que la gente consideraría injustas, y debes decir a las personas qué estás haciendo.

**Limitación del propósito.** Recoge datos para un propósito claro y declarado. No los reutilices después para algo no relacionado sin una nueva base legal.

**Minimización de datos.** Recoge solo lo que realmente necesitas. Si no necesitas un teléfono, no lo pidas. Esto importa para la IA: no vuelques toda tu base de datos en una herramienta cuando bastaría una pequeña porción.

**Exactitud.** Mantén los datos correctos y actualízalos. Las personas pueden exigir correcciones.

**Limitación del almacenamiento.** No guardes datos personales más tiempo del que necesitas. Ten un calendario de borrado.

**Integridad y confidencialidad.** Mantenlos seguros frente a brechas. El cómo se hace está en el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md).

**Responsabilidad proactiva.** Debes poder *demostrar* que cumples —con registros, políticas y documentos—. Por eso el papeleo de la sección de Lista de comprobación no es opcional.

### 10.2 Datos personales, datos sensibles, datos anónimos: las diferencias que importan

**Dato personal** es cualquier información sobre una persona viva que pueda ser identificada, directa o indirectamente. Un nombre, un correo, un teléfono, una foto, un número de identificación, una ubicación, un identificador online como un ID de cookie. Incluso una combinación de detalles que destaque a alguien cuenta. Si puedes señalar a una persona, es un dato personal.

**Dato sensible** (la ley lo llama "categorías especiales") recibe protección más fuerte. Incluye: origen racial o étnico, opiniones políticas, creencias religiosas o filosóficas, afiliación sindical, datos genéticos, datos biométricos usados para identificar a una persona, datos de salud, y datos sobre la vida sexual u orientación sexual de una persona. La regla es que tratar estos está prohibido salvo que se aplique una condición específica, como consentimiento explícito o un requisito legal claro. En IA, vigila que se escondan dentro de currículums, tickets de soporte y archivos de RRHH. Un chatbot que aprende "este cliente está en quimioterapia" ha tocado datos de salud.

**Dato anónimo** es información que ya no puede identificar a una persona, incluso combinándola con otros datos. Los datos verdaderamente anónimos están fuera del RGPD, porque no hay una persona identificable. Pero el anonimato verdadero es difícil de lograr. Si pudieras reidentificar a alguien, no es anónimo. Esta es la diferencia que atrapa a la gente, y es el foco de la sección 10.8.

La regla práctica: trata casi todo lo relativo a un cliente, empleado o solicitante como dato personal por defecto. Trata cualquier cosa que toque salud, creencias o identidad como sensible y manéjalo con cuidado extra. Solo llama a un dato anónimo si has eliminado de verdad la capacidad de identificar a alguien.

### 10.3 Consentimiento: cuándo se necesita y cuándo no

El consentimiento es una base legal para el tratamiento, no la única, y a menudo se malinterpreta.

Para que el consentimiento sea válido, debe ser **libre, específico, informado e inequívoco**, y dado por una acción clara. Una casilla ya marcada no es consentimiento. Cláusulas enterradas no son consentimiento. El consentimiento para "márketing y todo lo demás" no es un consentimiento válido.

Necesitas consentimiento cuando ninguna otra base encaja, y siempre para datos sensibles en la mayoría de los casos, y para ciertas cosas como correos de márketing a consumidores en muchos países de la UE.

A menudo **no** necesitas consentimiento cuando se aplica otra base. Si tratas datos para cumplir un contrato que tienes con el cliente, esa es la base de "contrato", no consentimiento. Si una ley te exige guardar registros, eso es "obligación legal". Pedir consentimiento cuando ya tienes un contrato puede en realidad crear problemas, porque el consentimiento puede retirarse en cualquier momento, y entonces no puedes entregar lo que prometiste.

Para la IA, el consentimiento es delicado. Si quieres usar datos de clientes para entrenar un modelo, un vago "podemos usar tus datos para mejorar nuestros servicios" normalmente no basta. Debes ser específico, y debes permitir a la gente decir que no sin perder el servicio. El camino más seguro es evitar necesitar un consentimiento amplio en absoluto: minimiza los datos, úsalos solo donde exista una base real, y prefiere entradas no personales o anonimizadas para el entrenamiento.

### 10.4 Interés legítimo: cuándo puedes usar datos sin consentimiento explícito

El interés legítimo es la base más flexible y más mal usada. Te permite tratar datos personales sin consentimiento cuando tienes una razón de negocio genuina y legal —pero solo después de una prueba cuidadosa—.

La prueba tiene tres partes. **Propósito:** ¿es tu razón legítima? Mejorar la detección de fraude o la seguridad de la red normalmente lo es. **Necesidad:** ¿es realmente necesario tratar el dato personal para lograrlo, o podrías hacerlo con menos o con datos anónimos? **Balance:** ¿pesan tus intereses más que los derechos y expectativas de la persona? ¿Se sorprendería o dañaría una persona razonable?

Debes documentar esta prueba de balance. No es un sentimiento; es una evaluación escrita que puedes mostrar.

Para la IA, el interés legítimo puede cubrir algunos usos —por ejemplo, usar datos de soporte al cliente para mejorar la calidad del servicio, si es necesario y equilibrado—. Pero no te permite hacer nada que un cliente encontraría intrusivo. Entrenar un modelo con datos sensibles bajo "interés legítimo" es muy difícil de justificar. Y como dice la opinión del CEPD en la sección Curiosidad, las pruebas de necesidad y balance deben pasar de verdad.

La regla práctica: si te sentirías incómodo explicando el uso a la persona en voz alta, el interés legítimo probablemente no lo cubre.

### 10.5 Derechos del interesado: acceso, rectificación, supresión, portabilidad

Las personas tienen derechos sobre sus datos, y debes poder honrarlos. Los principales:

**Derecho a ser informado.** Debes decir a las personas, con claridad, qué datos recoges y por qué, normalmente en un aviso de privacidad.

**Derecho de acceso.** Una persona puede preguntar qué datos guardas sobre ella y cómo los usas. Esta es la solicitud de acceso del interesado del ejemplo. Debes proporcionar una copia, normalmente dentro de un mes, sin coste.

**Derecho de rectificación.** Si el dato es incorrecto, pueden hacerlo corregir.

**Derecho a la supresión ("derecho al olvido").** Pueden pedirte que borres sus datos, y debes hacerlo, salvo que una razón legal para conservarlo lo anule —por ejemplo, un registro fiscal que estás obligado a retener—.

**Derecho a la limitación del tratamiento.** Pueden pausar cómo usas los datos en ciertas situaciones mientras se resuelve una disputa.

**Derecho a la portabilidad de datos.** Pueden pedir sus datos en un formato estructurado, común y legible por máquina para poder moverlos a otro sitio. Esto conecta con el problema de dependencia del proveedor del [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).

**Derecho de oposición.** Pueden oponerse al tratamiento basado en interés legítimo, y al márketing directo.

**Derechos sobre las decisiones automatizadas.** Bajo el Artículo 22, una persona tiene derecho a no estar sujeta a una decisión basada puramente en tratamiento automatizado que tenga efecto legal o similarmente significativo sobre ella, con excepciones limitadas, y el derecho a la intervención humana. Esto es crítico para la IA que filtra personas para empleos, crédito o servicios.

Construye un proceso simple y escrito para recibir y responder estas solicitudes a tiempo. Cuando usas una IA de terceros, asegúrate de que el proveedor pueda ayudarte a producir y borrar los datos, o no podrás honrar la solicitud.

### 10.6 La Ley de IA de la UE: qué cambia para la privacidad

La Ley de IA de la UE es una ley separada del RGPD, y se trata por completo en el [Capítulo 5](ch05-rules-and-legal-responsibility.md). Aquí está solo el ángulo de privacidad, para que las dos no se confundan.

Piénsalo así. **El RGPD gobierna el dato personal que fluye a través de un sistema de IA. La Ley de IA gobierna el sistema de IA en sí —su nivel de riesgo, sus obligaciones, y cómo puede usarse—.** Si tu sistema de IA usa datos personales, ambos se aplican al mismo tiempo. No son alternativas; se apilan.

Para un sistema de IA de alto riesgo que trata datos personales, acabas haciendo dos trabajos relacionados. Bajo la Ley de IA, sigues un proceso de riesgo y conformidad para el sistema. Bajo el RGPD, necesitas una base legal para el dato personal y, donde el riesgo es alto, una Evaluación de Impacto en la Protección de Datos. La buena noticia es que el trabajo se solapa: entender tus datos, documentar tu proceso y evaluar el riesgo sirven a ambas leyes.

La Ley de IA también presiona sobre la calidad de los datos para los sistemas de alto riesgo —los datos de entrenamiento y prueba deben ser relevantes y representativos, y tan libres de errores como sea apropiado—. Eso encaja con el principio de exactitud del RGPD. Y los deberes de transparencia de la Ley de IA —decir a las personas que están interactuando con IA— se sientan junto a los deberes de transparencia del RGPD.

El punto práctico: no trates la Ley de IA y el RGPD como una sola lista de comprobación. Haz dos preguntas sobre cada sistema de IA. *¿Cuál es el riesgo del sistema bajo la Ley de IA?* Y *qué datos personales fluyen a través de él, y es eso legal bajo el RGPD?* La primera es el trabajo del Capítulo 5; la segunda es el de este capítulo.

### 10.7 Evaluación de Impacto en la Protección de Datos (EIPD): cuándo es obligatoria y cómo hacerla

Una Evaluación de Impacto en la Protección de Datos es una revisión estructurada que haces **antes** de iniciar una actividad de tratamiento que probablemente sea de alto riesgo para las personas. Para la IA, a menudo necesitarás una.

Debes hacer una EIPD cuando el tratamiento es de alto riesgo. Disparadores claros incluyen: evaluación sistemática y extensa de personas basada en tratamiento automatizado que produce efectos significativos (esto cubre la IA que puntúa, clasifica o perfila personas); tratamiento a gran escala de datos sensibles; y vigilancia sistemática a gran escala de zonas accesibles al público. Las nuevas tecnologías usadas de formas nuevas también elevan el riesgo.

Cómo hacer una, en pasos claros:

1. **Describe el tratamiento.** Qué datos, qué propósito, cuánto tiempo, quién los ve, dónde se almacenan, y si un tercero o la IA está involucrado.
2. **Comprueba necesidad y proporcionalidad.** ¿Es esta la forma menos intrusiva de alcanzar tu objetivo?
3. **Evalúa los riesgos para las personas.** No el riesgo para tu empresa —el riesgo para su privacidad, equidad y derechos—. Piensa en sesgo, error, recolección excesiva y reidentificación.
4. **Enumera las medidas para reducir esos riesgos.** Minimiza datos, anonimiza donde sea posible, añade revisión humana, asegura el sistema, fija una retención corta.
5. **Decide.** Si un alto riesgo persiste tras tus medidas, debes consultar a tu autoridad nacional de protección de datos antes de proceder.
6. **Documenta y revisita.** Escríbelo y revísalo cuando el sistema cambie.

Una EIPD no es un formulario para marcar. Es un ejercicio de pensamiento que, hecho con honestidad, a menudo cambia tu diseño para mejor.

### 10.8 Anonimización y seudonimización: qué son y por qué importan

Estas dos palabras suenan parecido y son muy diferentes. Confundirlas causa problemas reales.

**Seudonimización** significa que reemplazas identificadores directos con un sustituto, como un código, y guardas la clave que enlaza el código con la persona por separado y de forma segura. "Cliente 4471" en vez de "Maria Rossi", con la tabla de correspondencia bajo llave. Los datos seudonimizados **siguen siendo datos personales** bajo el RGPD, porque con la clave puedes reidentificar a la persona. Es una medida de seguridad valiosa —reduce el riesgo si los datos son robados— pero no te saca de la ley.

**Anonimización** significa que eliminas la información identificadora tan a fondo que nadie puede reidentificar a una persona, incluso combinando los datos con otras fuentes. La ley pregunta si la reidentificación es "razonablemente probable", considerando coste, tiempo y tecnología actual. Los datos verdaderamente anónimos están **fuera del RGPD**, porque no hay una persona identificable. Pero el anonimato verdadero es genuinamente difícil. Conjuntos de datos que parecían anónimos han sido reidentificados cruzando otros datos públicos.

Por qué importa para la IA: si quieres entrenar un modelo con datos sin que se aplique el RGPD, necesitas anonimato real, no seudonimización. Y como advierte la opinión del CEPD, incluso un modelo entrenado puede no ser anónimo si pueden extraerse datos personales de él mediante preguntas astutas. Así que "anonimizamos los datos de entrenamiento" es una afirmación que debes poder defender, no solo afirmar.

La regla de trabajo segura: trata los datos seudonimizados como datos personales, porque lo son. Solo trata un dato como anónimo si has probado que la reidentificación no es razonablemente posible. Ante la duda, mantén las protecciones del RGPD puestas.

## Ética y responsabilidad

El RGPD es el suelo, no el techo. Cumplir significa que evitas multas; la ética significa que haces lo correcto incluso donde la ley calla.

**Respeta a la persona detrás del dato.** Cada registro es la vida privada de alguien. Pregúntate si tu uso te parecería justo si fueras tú quien está siendo perfilado por una IA.

**No te escondas detrás de "el modelo lo hizo."** Si una IA toma una decisión injusta sobre una persona usando tus datos, tú eres responsable. Mantén un humano que sea dueño del resultado, como expone el [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md).

**Sé transparente sobre la IA.** Di a las personas cuando una IA toca sus datos y qué hace. Las sorpresas erosionan la confianza más rápido que cualquier fallo técnico.

**Minimiza como hábito moral.** Recoger menos no es solo una regla legal; es respeto. Cada campo que no recoges es un campo que no puede filtrarse ni malusarse.

**Protege a los vulnerables.** Los datos sensibles sobre salud, creencias o finanzas merecen el máximo cuidado. Si una herramienta no puede garantizarlo, no los metas en la herramienta.

## Errores a evitar

1. **"Somos demasiado pequeños para el RGPD."** El tamaño no te exime. Si tratas datos personales de personas en la UE, las reglas se aplican.
2. **Pensar que el consentimiento siempre se necesita, o nunca.** Es una base entre seis. Usa la correcta y documenta por qué.
3. **Confundir seudonimización con anonimato.** Los datos seudonimizados siguen siendo datos personales y siguen dentro del alcance.
4. **Vuelcar toda tu base de datos en una herramienta de IA.** Eso rompe la minimización de datos y dispersa el riesgo.
5. **Sin base legal para entrenar con datos personales.** "Mejorar nuestros servicios" normalmente no basta.
6. **Ignorar los datos sensibles escondidos en currículums y tickets.** Salud, creencias y actividad sindical pueden estar dentro de documentos corrientes.
7. **Sin EIPD antes de un despliegue de IA de alto riesgo.** Hazla antes, no después de una queja.
8. **Sin proceso para solicitudes de acceso y borrado.** Si no puedes encontrar y borrar los datos, no puedes honrar el derecho.
9. **Perder el control de los datos ante un tercero.** Si el proveedor no puede ayudarte a borrar o exportar, estás expuesto. Ver [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).
10. **Tratar la ley como un proyecto de una sola vez.** El RGPD es continuo. La retención, las brechas y las solicitudes siguen llegando.

## Ejercicio práctico

### 10.10 Tu lista de comprobación de cumplimiento del RGPD para IA

Toma media jornada y trabaja esto para un caso de uso de IA que toque datos personales.

1. **Mapea los datos.** Enumera exactamente qué datos personales fluyen hacia la IA. Nombra cada campo. Marca cualquier categoría sensible. (Una plantilla de inventario de datos está en los apéndices.)
2. **Nombra la base legal.** Para cada uso, escribe cuál de las seis bases se aplica y por qué. Si no puedes nombrar una, para y reconsidera.
3. **Busca datos sensibles.** Si hay algún dato de categoría especial presente, confirma que una condición específica lo permite, o elimínalo.
4. **Aplica la minimización.** Corta cada campo que no necesites estrictamente.
5. **Decide el destino.** ¿Van los datos a un tercero? Si es así, ejecuta las preguntas de proveedor del [Capítulo 9](ch09-third-party-services-and-shadow-ai.md).
6. **Haz una EIPD.** Si el uso es de alto riesgo —perfilado, datos sensibles a gran escala, decisiones automatizadas— completa los pasos de la EIPD de la sección 10.7.
7. **Planifica los derechos.** Escribe cómo manejarás las solicitudes de acceso, corrección y borrado para estos datos, incluidos los datos en poder del proveedor.
8. **Fija la retención.** Decide cuánto tiempo guardas los datos y cuándo los borras.
9. **Revisa las reglas de decisión automatizada.** Si la IA decide sobre personas con efecto significativo, asegúrate de que exista una vía de revisión humana.
10. **Documenta todo.** Escribe las respuestas. La responsabilidad proactiva significa que puedes mostrar tu trabajo.

Si algún paso deja un hueco que no puedes rellenar, ese hueco es tu lista de tareas.

## Lista de comprobación

### 10.11 Los documentos que debes tener

Para un sistema de IA que toca datos personales, mantén estos documentos listos y al día.

- [ ] **Aviso de privacidad** que explique con claridad qué datos recoges, por qué, y cómo interviene la IA.
- [ ] **Registro de actividades de tratamiento** que describa cada uso de datos personales.
- [ ] **Declaración de base legal** para cada propósito de tratamiento, escrita.
- [ ] **Inventario de datos** que enumere cada campo de datos personales y dónde vive.
- [ ] **EIPD** para cualquier tratamiento de IA de alto riesgo, con la decisión de riesgo residual.
- [ ] **Prueba de balance** si te apoyas en el interés legítimo.
- [ ] **Acuerdo de tratamiento de datos** con cada proveedor que maneje tus datos.
- [ ] **Calendario de retención** que indique cuánto tiempo se guarda cada tipo de dato y cuándo se borra.
- [ ] **Procedimiento de solicitud del interesado** para acceso, rectificación, supresión y portabilidad, con un reloj de un mes.
- [ ] **Plan de respuesta a brechas** que incluya notificar a la autoridad dentro de 72 horas y a las personas afectadas cuando se requiera.
- [ ] **Garantías de decisión automatizada** con una vía de revisión humana para decisiones significativas.
- [ ] **Contacto del Delegado de Protección de Datos**, si tu tratamiento requiere uno.

Mantén estos vivos. Un documento que nunca actualizas es un documento que te fallará cuando un regulador o un cliente pregunte.

## Puntos clave

- El RGPD se aplica a cualquier dato personal sobre personas identificables en la UE, incluso cuando fluye a través de una herramienta de IA, y alcanza a empresas fuera de la UE que sirven a clientes de la UE.
- Necesitas una base legal para cada uso; el consentimiento es solo una de seis, y los datos sensibles necesitan una condición específica encima.
- Las personas tienen derechos reales —acceso, corrección, supresión, portabilidad— y debes poder honrarlos, incluso para datos en poder de un proveedor tercero.
- La seudonimización no es anonimato; solo los datos que no pueden razonablemente reidentificarse salen del RGPD, y un modelo que filtra datos personales no es anónimo.
- Para IA de alto riesgo, haz una EIPD antes de empezar, y recuerda que la Ley de IA y el RGPD se aplican juntos, no en lugar del otro.
