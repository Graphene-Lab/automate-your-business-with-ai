# Capítulo 28 — Recursos humanos y personas

## En palabras simples

Los recursos humanos son el lugar donde una empresa se encuentra con su gente. Contratar, formar, ayudar a que el nuevo personal se adapte y entender por qué la gente se va: todo esto da forma a toda la empresa. También están llenos de trabajo repetitivo: leer cientos de currículums, responder las mismas preguntas de incorporación, organizar la formación por puesto y rebuscar en viejos archivos para descubrir por qué el personal renuncia. La IA puede quedarse con la parte repetitiva de cada tarea y dejar la parte humana —el criterio, la equidad y el cuidado— donde corresponde.

Piensa en recursos humanos como un embudo y un jardín al mismo tiempo. El embudo es la contratación: entran muchas personas por arriba y los vas reduciendo hasta unos pocos que encajan bien. El jardín es toda la gente que ya tienes: la riegas con formación, vigilas las señales de problemas e intentas que sigan creciendo. La IA ayuda en ambos extremos. En el embudo, ordena y hace listas de candidatos más rápido de lo que una persona puede leer. En el jardín, detecta patrones en mil pequeñas señales que ningún gestor podría tener en la cabeza.

Este capítulo trata cuatro tareas: filtrar currículums y solicitudes, incorporar a los nuevos empleados, formación personalizada y análisis de la rotación. Cada una es un lugar donde una pequeña empresa puede ahorrar tiempo y tomar mejores decisiones sobre las personas.

Una idea honesta antes de empezar: las personas no son facturas. Un número equivocado en una factura cuesta dinero; una decisión equivocada sobre una persona cuesta una vida, una carrera y tu reputación. Por eso la IA en recursos humanos es una *ayudante*, nunca la *jueza*. Lee, ordena, sugiere y avisa. Una persona sigue decidiendo quién consigue el trabajo, quién recibe el ascenso y por qué se despide a alguien. Y en Europa, la contratación y la gestión de los trabajadores se consideran usos de alto riesgo de la IA, con obligaciones legales reales. El tratamiento completo de la Ley de IA de la UE está en el [Capítulo 5 — Reglas y responsabilidad legal](ch05-rules-and-legal-responsibility.md); este capítulo te muestra qué automatizar y cómo, y dónde traza la ley una línea. El método para juzgar si todo esto compensa está en el [Capítulo 16 — Metas, costes y retorno de la inversión](ch16-goals-costs-and-return-on-investment.md).

## Un poco de historia

**Años 80–90: la base de datos de recursos humanos.** El primer gran cambio en el trabajo de recursos humanos fue el expediente de personal informatizado. En lugar de carpetas de papel en un archivador, los registros de los empleados vivían en una base de datos. La nómina, la asistencia y los datos personales se volvieron consultables. Fue la primera vez que un software tocaba el núcleo de recursos humanos, y marcó el patrón: guardar los datos y dejar al humano al mando de las decisiones.

**Años 90–2000: el sistema de seguimiento de candidatos.** Cuando las solicitudes de empleo se trasladaron a internet, las empresas adoptaron el sistema de seguimiento de candidatos, o ATS —un software que recoge las solicitudes, las guarda y permite a los reclutadores buscarlas y ordenarlas. Un reclutador podía ahora ver todos los candidatos de una vacante en un solo lugar y filtrar por palabras clave. Esto puso orden en la avalancha de solicitudes en línea, pero el filtrado era simple: hacía coincidir palabras, no personas.

**Años 2000: la formación en línea y el sistema de gestión del aprendizaje.** La formación pasó del aula a la pantalla. El sistema de gestión del aprendizaje, o LMS, ofrecía cursos en línea y registraba quién completaba qué. Esto hizo la formación escalable, pero las primeras versiones eran de talla única: todos veían el mismo vídeo, sin importar lo que ya supieran.

**Años 2010: analítica de personas.** Las empresas empezaron a analizar los datos de recursos humanos como analizaban los datos de ventas. Miraban qué contrataciones se quedaban, qué equipos rendían y qué señales predecían que alguien se iría. La analítica de personas convirtió recursos humanos de una función de papeleo en una función de datos. Pero necesitaba grandes conjuntos de datos y analistas cualificados, así que sobre todo las grandes empresas podían hacerlo.

**Años 2020: los grandes modelos de lenguaje leen y escriben sobre personas.** Los grandes modelos de lenguaje —IA entrenada con enormes cantidades de texto— ahora pueden leer un currículum y una descripción de puesto y juzgar cuánto coinciden, redactar un plan de formación personalizado y responder a la pregunta de recursos humanos de un empleado en lenguaje claro. Este es el paso más reciente: una IA que lee las palabras que escriben las personas y razona sobre ellas. Es poderosa, y precisamente porque es poderosa, es el área donde la ley es más estricta.

El arco: de las carpetas de papel, a bases de datos consultables, a filtros de palabras clave, a analítica, a una IA que lee y razona sobre las personas. Cada paso quitó más trabajo repetitivo de las manos humanas —y cada paso elevó lo que estaba en juego en cuanto a equidad, porque las decisiones son sobre vidas humanas.

## Curiosidad

### 28.5 La ley dice: avisa a tus trabajadores antes de que la IA toque sus empleos

He aquí un dato que todo empleador europeo debería conocer antes de activar cualquier herramienta de recursos humanos que afecte al personal.

La Ley de IA de la UE tiene una regla específica sobre los trabajadores. En palabras simples: si usas un sistema de IA de alto riesgo en el lugar de trabajo —uno que afecte a las decisiones sobre tus empleados—, debes informar a tus trabajadores y a sus representantes *antes* de empezar a usarlo. La ley lo establece directamente en el Artículo 26(7): "Antes de poner en servicio o utilizar un sistema de IA de alto riesgo en el lugar de trabajo, los despliegues que sean empleadores informarán a los representantes de los trabajadores y a los trabajadores afectados de que estarán sujetos al uso del sistema de IA de alto riesgo".

Aquí importan dos cosas. Primera, no es opcional. Es una obligación legal, no una cortesía. Segunda, es *antes*, no después. No puedes desplegar una herramienta de IA para filtrar y avisar a la gente un mes después. Se lo dices primero.

¿Por qué existe esta regla? Porque las personas tienen derecho a saber cuándo una máquina está dando forma a su vida laboral —si una herramienta está leyendo su solicitud, clasificando su rendimiento o decidiendo sus tareas. El secretismo sobre la IA en el trabajo erosiona la confianza y puede ocultar injusticias. Decirlo abiertamente es lo mínimo que hace un empleador justo.

Una advertencia relacionada: la misma ley *prohíbe* el reconocimiento de emociones en el lugar de trabajo —usar IA para leer los sentimientos de un trabajador desde su cara o su voz está prohibido, salvo por razones médicas o de seguridad. Una herramienta que "detecte" si un agente de un centro de llamadas está contento o estresado para puntuarlo está claramente prohibida. La lista completa de prácticas prohibidas y las fechas escalonadas están en el [Capítulo 5](ch05-rules-and-legal-responsibility.md). El punto aquí es simple: sé abierto sobre la IA que usas con las personas, y nunca leas en secreto sus emociones.

## Un ejemplo real de negocio

**Una empresa mediana que automatizó la contratación y la incorporación —un escenario ilustrativo.**

Este ejemplo es ilustrativo. Es un caso compuesto realista, no el resultado reportado de una empresa, construido para mostrar cómo encajan las cuatro tareas de recursos humanos y dónde sitúan el humano y la ley.

Imagina una empresa de 400 personas que contrata unos 80 empleados al año, sobre todo para unos pocos puestos recurrentes: ventas, atención y back-office. Cada vacante trae de 200 a 400 solicitudes. Los dos empleados de recursos humanos estaban desbordados: leer currículums tardaba días, las preguntas de incorporación se repetían todo el día y nadie sabía por qué la gente se iba tras un año.

Cambiaron tres cosas.

Primero, **filtrado de currículums con una comprobación humana.** Usaron una herramienta de IA para leer cada solicitud contra la descripción del puesto y producir una lista de candidatos con una breve razón para cada coincidencia. El personal de recursos humanos no dejó que la herramienta rechazara a nadie. Revisaron la lista y, además, cada semana tomaban una muestra de las solicitudes rechazadas para comprobar que la herramienta no estaba descartando injustamente a buenos candidatos. La herramienta redujo el tiempo de filtrado de días a horas. La decisión siguió siendo humana.

Segundo, **un asistente de incorporación.** Construyeron un chatbot entrenado con su propio manual, sus políticas y sus preguntas frecuentes. Los nuevos empleados podían preguntar "¿Cómo pido vacaciones?" o "¿Cuál es la política de gastos?" y obtener una respuesta al instante, de día o de noche. Los dos empleados de recursos humanos dejaron de responder las mismas diez preguntas cada día y dedicaron su tiempo a los nuevos empleados que de verdad necesitaban a un humano —los nerviosos, los que tenían situaciones poco comunes.

Tercero, **una revisión de la rotación.** Reunieron dos años de registros de recursos humanos en un análisis simple: quién se fue, de qué puesto, tras cuánto tiempo y qué decía su última encuesta de compromiso. El patrón era claro —el personal de atención se iba más a menudo tras 12 a 18 meses, y sus comentarios de salida se agrupaban en torno al sueldo y la falta de un camino claro para crecer. Ese único hallazgo les dio una solución concreta: una revisión salarial y un camino de ascenso definido para atención. No necesitaban una IA sofisticada para actuar; necesitaban que el patrón saliera a la luz, y el análisis lo hizo.

Fíjate en la forma. La IA hizo la lectura, las respuestas y la clasificación. Los humanos hicieron las decisiones, el cuidado y la acción. Y como la herramienta de filtrado afectaba a la contratación —un uso de alto riesgo—, la empresa informó a sus trabajadores y a sus representantes antes de activarla, como exige la ley. Ese es el modelo a copiar.

## Cómo hacerlo

### 28.1 Filtrado de currículums

Filtrar currículums es el clásico pozo de tiempo de recursos humanos. Una sola vacante puede traer cientos de solicitudes, y leer cada una lleva minutos. La IA puede leerlas todas y producir una lista de candidatos, de modo que un humano revise un montón manejable en lugar de una montaña.

**Qué hace la IA.** Lee cada currículum y la descripción del puesto, y luego clasifica u ordena las solicitudes según cuánto coincidan. Mira habilidades, experiencia y palabras clave. Las herramientas modernas leen el significado, no solo las palabras, así que "dirigí un equipo de cinco" puede coincidir con "experiencia de liderazgo".

**La advertencia de alto riesgo.** En la UE, usar IA para filtrar solicitudes de empleo o seleccionar candidatos es un uso de **alto riesgo** según la Ley de IA, porque afecta el sustento de una persona. Eso trae obligaciones reales: transparencia, supervisión humana y cuidado contra el sesgo. Lee el [Capítulo 5](ch05-rules-and-legal-responsibility.md) antes de desplegar cualquier herramienta de filtrado. No trates un filtrador de currículums como "solo un software".

**El sesgo es el peligro central.** Una IA entrenada con contrataciones pasadas aprende los patrones de las contrataciones pasadas —incluida cualquier injusticia pasada. Si tu empresa históricamente contrató sobre todo hombres para un puesto, la herramienta puede aprender a bajar la clasificación de las mujeres. Si aprendió a favorecer una universidad, puede descartar candidatos igual de buenos de otros sitios. Esto no es hipotético; ha ocurrido en sistemas reales. Protégete contra ello: revisa la lista de candidatos y el montón de rechazados buscando patrones, prueba la herramienta con ejemplos diversos y nunca dejes que rechace de forma automática.

**Mantén la decisión humana.** Usa la IA para hacer la lista y para explicar *por qué* coincidió. Una persona toma la decisión. Una lista con razones es mucho mejor que un simple ranking, porque permite al revisor ver la lógica de la herramienta y detectar una mala coincidencia.

**Informa a candidatos y trabajadores.** Sé abierto en que la IA asiste en el filtrado, e informa a tus trabajadores y a sus representantes antes de activarla, como exige la ley. Los datos de los candidatos son datos personales; trátalos según las normas de privacidad del [Capítulo 10 — Privacidad y RGPD](ch10-privacy-and-gdpr.md).

### 28.2 Incorporación

La incorporación es la primera experiencia real que un nuevo empleado tiene de tu empresa. Una buena incorporación hace que una persona se sienta bienvenida, clara y preparada. Una mala la deja confundida y ansiosa. La IA ayuda respondiendo al instante las interminables preguntas de rutina, de modo que el lado humano de la incorporación —la bienvenida, las presentaciones, la tranquilidad— reciba más tiempo, no menos.

**El asistente de incorporación.** Un chatbot entrenado con tu manual, tus políticas y las preguntas comunes puede responder a un nuevo empleado a las 9 de la noche de la víspera de su primer día: "¿A qué hora debo llegar?", "¿Qué llevo?", "¿Cómo se configura la nómina?". Esto elimina las pequeñas confusiones que hacen estresante el primer día.

**Una lista de comprobación guiada.** La IA puede generar un plan de incorporación personalizado para cada puesto: las cuentas que abrir, los sistemas a los que acceder, las personas que conocer, la formación que terminar. En lugar de una lista genérica única, cada nuevo empleado recibe un camino que se ajusta a su trabajo. La herramienta sigue el progreso y avisa lo que falta.

**Redacta los materiales de bienvenida.** La IA puede redactar el correo de bienvenida, la presentación al equipo y el horario de la primera semana, de modo que el gestor parta de un buen borrador en lugar de una página en blanco. El gestor lo personaliza. El toque humano se mantiene, pero el trabajo pesado se reduce.

**Lo que la IA no puede reemplazar.** El café de bienvenida, el mentor, el gestor que se pasa a saludar el tercer día. La incorporación es tan emocional como práctica. Usa la IA para la información y la lista de comprobación; mantén una persona para la bienvenida. Un nuevo empleado que solo habla con un bot se siente como un número.

**Mide los primeros 90 días.** Registra cuánto tarda un nuevo empleado en ser productivo y cómo se siente a los 30, 60 y 90 días. Si la incorporación con IA funciona, el tiempo de adaptación baja y la satisfacción temprana sube. Si no, el bot no es la respuesta —lo es el proceso.

### 28.3 Formación personalizada

La formación antigua era de talla única: todos veían el mismo curso. La formación personalizada usa la IA para adaptar el aprendizaje a lo que cada persona ya sabe y a lo que su puesto necesita. Es la diferencia entre una clase magistral y un tutor que sabe dónde estás atascado.

**Adáptate a la persona.** La IA puede hacer un pequeño test inicial, ver qué sabe ya una persona y saltarse lo que ya domina. Dedica tiempo solo a las lagunas. Esto respeta el tiempo del alumno y hace la formación más rápida y relevante.

**Adáptate al puesto.** Un empleado de atención necesita una formación distinta que uno de ventas, incluso en la misma empresa. La IA puede armar un camino de aprendizaje desde tu biblioteca de contenido que se ajuste al puesto, al nivel y al ritmo de la persona.

**Redacta el contenido.** La IA puede convertir tus documentos existentes —una política, una guía de producto, una reunión grabada— en un módulo de formación corto con preguntas para comprobar la comprensión. Esto convierte conocimiento que ya existe en formación que la gente puede usar de verdad, sin que un especialista construya cada curso.

**Responde preguntas mientras se aprende.** Un alumno puede preguntarle a la IA sobre un punto difícil y obtener una explicación en palabras claras, como un tutor. Aquí es donde los grandes modelos de lenguaje brillan: explican, reformulan y dan ejemplos al momento.

**Manténlo honesto y revisado.** La formación generada por IA debe ser revisada por un humano experto antes de salir. Un módulo de formación seguro de sí mismo pero equivocado difunde errores rápido. Comprueba los hechos, comprueba el tono y mantén una persona disponible para las preguntas que importan. La formación da forma a cómo trabaja la gente; debe ser correcta.

### 28.4 Análisis de la rotación

La rotación significa que la gente deja tu empresa. Una rotación alta es cara —pierdes habilidades, vuelves a contratar, vuelves a formar. El análisis de la rotación usa la IA para mirar tus datos de recursos humanos y descubrir *por qué* se va la gente, para que puedas arreglar la causa en lugar de adivinar.

**Qué mira la IA.** Combina registros: quién se fue, de qué puesto, tras cuánto tiempo, su sueldo, su gestor, su última encuesta de compromiso, si fue ascendido, con qué frecuencia llegaba tarde. Por separado, cada dato es pequeño. Juntos, forman un patrón.

**El valor está en el patrón.** La IA puede sacar algo como: "Las personas en el puesto X que no han sido ascendidas en 18 meses se van a un ritmo tres veces superior al normal". Ese es un hallazgo en el que puedes actuar. Ningún gestor podría tener mil registros en la cabeza y verlo; el análisis sí puede.

**Predice el riesgo, no la persona.** Algunas herramientas señalan qué empleados actuales muestran patrones similares a los de los que se fueron. Usa esto para *iniciar una conversación* —un seguimiento, un plan de desarrollo—, nunca para marcar en silencio a alguien como "probable de irse" y tratarlo de forma distinta. Una predicción es una razón para cuidar, no una razón para actuar contra alguien.

**Vigila las pequeñas señales.** Las encuestas de compromiso, una caída en el rendimiento, un ascenso perdido, un cambio de gestor —estas son las pequeñas señales que a menudo preceden a una renuncia. La IA es buena notándolas en muchas personas a la vez. El trabajo humano es responder con una conversación real.

**La privacidad primero.** El análisis de la rotación usa datos personales sensibles. Trátalo según las normas de privacidad del [Capítulo 10](ch10-privacy-and-gdpr.md), mantenlo seguro y úsalo para mejorar las condiciones del grupo, no para espiar a individuos. La meta es un mejor lugar de trabajo, no un sistema de vigilancia.

## Ética y responsabilidad

Recursos humanos es el lugar más delicado para usar IA, porque el resultado es una decisión sobre una vida humana. El listón ético aquí es más alto que en cualquier otro punto de este libro.

**Una persona decide sobre las personas.** La IA lee, ordena y sugiere. Un humano toma cada decisión de contratación, ascenso y despido. Nunca dejes que una herramienta rechace automáticamente a un candidato o despida automáticamente a un trabajador. El humano debe ser dueño del resultado y poder explicarlo.

**Combate el sesgo activamente.** La IA de recursos humanos hereda los sesgos de sus datos de entrenamiento. Revisa los resultados entre grupos —género, edad, origen— y busca patrones injustos. Prueba la herramienta antes de confiar en ella, y sigue probándola después. La equidad no es un ajuste que enciendes una vez; es un hábito que compruebas.

**Sé abierto con los trabajadores.** Informa a tus trabajadores y a sus representantes antes de que cualquier IA de alto riesgo toque sus empleos, como exige la ley. El secretismo sobre la IA en el trabajo rompe la confianza y oculta injusticias. La apertura es a la vez la ley y lo correcto.

**Nunca leas emociones en el trabajo.** El reconocimiento de emociones en el lugar de trabajo está prohibido por la Ley de IA de la UE. No compres ni uses una herramienta que puntúe al personal leyendo sus caras o voces. Está prohibido, y está mal.

**Protege los datos personales.** Los datos de recursos humanos están entre los más sensibles que guarda una empresa —sueldo, notas de salud, rendimiento, circunstancias personales. Guárdalos, limita quién los ve y sigue el [Capítulo 10](ch10-privacy-and-gdpr.md). No introduzcas datos de empleados en herramientas de IA públicas sin comprobar las implicaciones de seguridad (ver [Capítulo 6 — Ciberseguridad en la era de la IA](ch06-cybersecurity-in-the-ai-era.md)).

**Usa los datos para ayudar, no para castigar.** Las predicciones de rotación y los datos de compromiso deben hacerte un mejor empleador —mejor sueldo, mejores caminos de crecimiento, mejores condiciones. Nunca deben convertirse en una herramienta para vigilar, clasificar o castigar a individuos. Mide el lugar de trabajo, no a la persona como un objetivo.

**Mantén el humano en la bienvenida.** En la incorporación y en el día a día de recursos humanos, la IA maneja la información; los humanos manejan el cuidado. Una empresa que externaliza todo el contacto humano a un bot pierde la confianza que hace que un lugar de trabajo funcione.

## Errores a evitar

**Dejar que la IA rechace candidatos.** El peor error de recursos humanos. Una herramienta que rechaza automáticamente oculta el sesgo y mata buenas contrataciones. Mantén siempre una decisión humana.

**Ignorar el sesgo.** No comprobar si la herramienta trata a los grupos de forma injusta. El sesgo de contratación del pasado se convierte en sesgo de contratación futuro si no miras. Prueba y revisa.

**Activar en secreto una herramienta de alto riesgo.** No informar a los trabajadores y a sus representantes antes de usar IA que les afecta. Eso rompe la ley y la confianza.

**Comprar una herramienta de reconocimiento de emociones.** Está prohibida en el lugar de trabajo. Un discurso de ventas de "detección de estado de ánimo" sobre el personal es una trampa.

**Tratar una predicción como un veredicto.** Actuar contra un empleado porque un modelo lo marcó como "probable de irse". Una predicción es una razón para hablar, no para castigar.

**Vigilar al personal.** Usar los datos de recursos humanos para vigilar y clasificar a individuos en lugar de mejorar las condiciones del grupo. Esto envenena la confianza.

**Una incorporación solo con bot.** Un nuevo empleado que nunca habla con un humano se siente como un número. Mantén la bienvenida humana.

**Formación de IA sin revisar.** Publicar formación generada por IA que está equivocada con total seguridad. Un humano experto debe revisarla.

**Automatizar un mal proceso de recursos humanos.** Si tu contratación o incorporación está rota, la IA hace un proceso roto más rápido. Arregla primero el proceso.

**Filtrar datos de empleados.** Poner datos sensibles de recursos humanos en herramientas de IA inseguras. Comprueba primero la seguridad y la privacidad.

**Sin línea base.** No medir el tiempo de contratación, el tiempo de adaptación ni la rotación antes, de modo que no puedes probar la mejora. Mide primero (ver [Capítulo 22 — Medir resultados y ROI](ch22-measuring-results-and-roi.md)).

**Olvidar que la ley es el suelo.** Cumplir con la Ley de IA no hace justo a un herramienta de contratación. La ética está por encima del cumplimiento, y es tuya (ver [Capítulo 4 — IA ética](ch04-ethical-ai-doing-the-right-thing.md)).

## Ejercicio práctico

### 28.7 Ejercicio: planifica una automatización de recursos humanos de forma responsable

Elige una tarea de recursos humanos y planifica su asistencia con IA de principio a fin, con el humano y la ley integrados.

**Paso 1 — Elige la tarea.** Elige una: filtrado de currículums, incorporación, formación o análisis de la rotación. Haz una, no todas.

**Paso 2 — Define la meta y la métrica.** ¿Tiempo de contratación más rápido? ¿Adaptación del nuevo empleado más rápida? ¿Menor rotación? Elige un número que medir.

**Paso 3 — Mide la línea base.** ¿Cuál es ese número ahora? ¿Cuánto tarda el filtrado? ¿Cuánto se tarda en adaptarse? ¿Cuál es tu tasa de rotación? Escríbelo.

**Paso 4 — Clasifica el riesgo.** ¿Es este un uso de alto riesgo según la Ley de IA? El filtrado y la gestión de trabajadores lo son. Si sí, tienes obligaciones legales: transparencia, supervisión humana, cuidado contra el sesgo. Anótalas (ver [Capítulo 5](ch05-rules-and-legal-responsibility.md)).

**Paso 5 — Marca cada paso.** Para cada paso, márcalo: **la IA lo hace** (leer, ordenar, redactar, sacar a la luz), **el humano lo revisa** (comprobar la lista, revisar la formación) o **el humano lo decide** (la contratación, el ascenso, la solución). Cada decisión sobre una persona debe ser humana.

**Paso 6 — Construye la comprobación de sesgo.** Decide cómo probarás los patrones injustos entre grupos, y con qué frecuencia revisarás el montón de rechazados y los resultados.

**Paso 7 — Planifica el aviso a los trabajadores.** Escribe cómo y cuándo informarás a los trabajadores y a sus representantes antes de activar la herramienta, como exige la ley.

**Paso 8 — Lanza a pequeña escala y mide.** Ejecútalo primero en un puesto o un equipo. Compara la métrica con la línea base. Escala solo lo que demuestre que ayuda y trata a las personas con justicia.

Haz bien una tarea. La comprobación de sesgo y el aviso a los trabajadores que construyas en los pasos 6 y 7 valen por sí solos —te obligan a ver tus propios patrones de contratación, lo cual es útil incluso más allá de la herramienta.

## Lista de comprobación

### 28.8 Lista de comprobación de recursos humanos y personas

Antes de usar IA con personas, comprueba esto.

- [ ] **Mediste la línea base** —tiempo de contratación, tiempo de adaptación, tasa de rotación.
- [ ] **Un humano toma cada decisión sobre una persona** —sin rechazo automático, sin despido automático.
- [ ] **Clasificaste el riesgo** —el filtrado y la gestión de trabajadores son de alto riesgo según la Ley de IA.
- [ ] **Informaste a los trabajadores y a sus representantes antes de activar** cualquier IA de alto riesgo que les afecte (Art. 26(7)).
- [ ] **Pruebas el sesgo** entre género, edad y origen, y revisas el montón de rechazados.
- [ ] **Nunca usas reconocimiento de emociones** con los trabajadores —está prohibido.
- [ ] **La herramienta explica sus coincidencias** para que un revisor pueda ver la lógica.
- [ ] **La incorporación mantiene una bienvenida humana** —el bot responde, una persona da la bienvenida.
- [ ] **La formación generada por IA es revisada por un humano experto** antes de salir.
- [ ] **Las predicciones de rotación inician una conversación**, no un castigo.
- [ ] **Los datos de recursos humanos se mantienen seguros** y siguen las normas de privacidad (ver [Capítulo 10](ch10-privacy-and-gdpr.md)).
- [ ] **Usas los datos para mejorar las condiciones del grupo**, no para vigilar a individuos.
- [ ] **Arreglas el proceso de recursos humanos antes de automatizarlo.**
- [ ] **Tratas el cumplimiento como el suelo** y tu propia equidad como el estándar por encima.

Si una casilla está vacía, una persona puede sentirlo —y la ley puede alcanzarla. Rellena cada casilla antes de dejar que la IA se acerque a tu gente.

## Puntos clave

- La IA en recursos humanos se queda con el trabajo repetitivo —leer currículums, responder preguntas de incorporación, ordenar formación, sacar a la luz patrones de rotación— y deja a los humanos las decisiones, el cuidado y la acción.
- La contratación y la gestión de trabajadores son usos de alto riesgo según la Ley de IA de la UE: una persona debe decidir, debes protegerte contra el sesgo y debes informar a los trabajadores y a sus representantes antes de activar cualquier IA de alto riesgo que les afecte.
- El reconocimiento de emociones en el lugar de trabajo está prohibido; nunca compres ni uses una herramienta que puntúe al personal leyendo sus sentimientos.
- Usa los datos de recursos humanos para mejorar el lugar de trabajo para el grupo, nunca para vigilar o castigar a individuos, y mantén la bienvenida humana en la incorporación.
- Mide la línea base, mantén un humano en cada decisión sobre personas, y trata la ley como el suelo y la equidad como el estándar por encima.

<!-- BEGIN agentbridge-examples -->

## Pruébalo con AgentBridge

Así se ve el mismo trabajo con AgentBridge. Cada caja muestra el resultado terminado y la única línea que escribes para obtenerlo.

### Un manual de personal sencillo

![Un manual de personal amable, listo para compartir](../../assets/examples/employee-handbook.png)
*Un manual de personal amable, listo para compartir*

**Lo que pides:** `Escribe un breve manual de empleado que cubra horario de trabajo, vacaciones, reglas de trabajo remoto y a quién pedir ayuda.`

El agente escribe un manual claro y amable en lenguaje sencillo, con cada tema en su propia página. Actualízalo cuando quieras preguntando —'añade una línea sobre la nueva norma de aparcamiento'.

*Consejo: Guárdalo en tu área de documentos para que el agente pueda responder preguntas a partir de él más adelante.*

---

### Un parte de horas semanal

![Un parte de horas semanal con totales por persona](../../assets/examples/timesheet.png)
*Un parte de horas semanal con totales por persona*

**Lo que pides:** `Crea un parte de horas semanal con personas, proyectos, horas por día y un total por persona.`

El agente construye la cuadrícula del parte con columnas diarias y totales automáticos. Rellénalo o adjunta tus horas aproximadas y deja que las ordene.

*Consejo: Multiplica las horas por cada tarifa y tendrás también una hoja de facturación —solo pídelo.*

---

### Forma a tu equipo rápido

![Una diapositiva de formación paso a paso](../../assets/examples/training-deck.png)
*Una diapositiva de formación paso a paso*

**Lo que pides:** `Haz una presentación de formación sobre cómo gestionar un reembolso a un cliente, paso a paso.`

El agente convierte el proceso en diapositivas claras, un paso en cada una, fáciles de seguir. Úsalo para la incorporación y los repasos.

*Consejo: Añade una diapositiva final con 'a quién preguntar' para que la gente sepa dónde conseguir ayuda.*

<!-- END agentbridge-examples -->
