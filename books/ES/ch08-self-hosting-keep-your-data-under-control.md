# Capítulo 8 — Alojamiento propio: mantén tus datos bajo control

## En palabras simples

El alojamiento propio significa ejecutar el software en ordenadores que tú posees o controlas, en lugar de alquilarlo en los ordenadores de otra persona.

Tú ya conoces los dos lados de esto. Alquilar una habitación de hotel es la nube: otro limpia, repara y guarda una llave de repuesto. Tener una casa propia es el alojamiento propio: tú arreglas la caldera, pero nadie más tiene la llave.

Aplicado a la IA, el alojamiento propio significa que el modelo —el software que hace el pensamiento— se ejecuta en una máquina de tu oficina o en un servidor que tú controlas. Tus preguntas entran ahí. Las respuestas salen de ahí. Nada viaja por internet hasta una empresa que tú no elegiste.

Hace poco, esto no era posible para un pequeño negocio. Hasta 2022, los mejores modelos de lenguaje vivían solo dentro de enormes centros de datos, y solo podías llegar a ellos por una puerta de entrada alquilada llamada API: una interfaz estándar que una empresa abre para que otros programas puedan hacer preguntas a sus sistemas. Cada pregunta que escribías pasaba por esa puerta y terminaba en sus máquinas.

Luego cambiaron dos cosas. Primero, aparecieron modelos abiertos: modelos cuyos archivos ya entrenados cualquiera puede descargar y ejecutar. Segundo, las técnicas de compresión mejoraron lo suficiente como para que un modelo comprimido funcione en un ordenador de sobremesa potente y corriente, con solo una pequeña pérdida de calidad.

El intercambio es un triángulo, y no puedes tener los tres vértices a la vez.

- **Control.** Tú decides qué pasa con tus datos, qué modelo usas, cuándo cambia y quién puede verlo.
- **Capacidad.** Lo buena que es de verdad la IA en tareas difíciles.
- **Coste.** Lo que pagas, en dinero, tiempo y atención.

La IA en la nube da alta capacidad a cambio de poco esfuerzo y poco control. El alojamiento propio da mucho control, una capacidad moderada y un coste que pagas por adelantado en hardware y luego otra vez en tiempo continuo. La respuesta correcta depende de lo que estés haciendo.

Dos frases honestas antes de seguir. El alojamiento propio no es automáticamente más seguro: un servidor local mal configurado es peor que un servicio en la nube bien gestionado. Y tampoco es automáticamente más barato: a pequeña escala, alquilar suele ganar. Lo que el alojamiento propio compra es algo concreto y valioso: tus datos no se van, y nadie puede cambiar tu sistema sin que tú te enteres.

Temas relacionados en otras partes: el [Capítulo 11](ch11-digital-sovereignty.md) cubre la idea más amplia de controlar tus propias herramientas digitales, el [Capítulo 9](ch09-third-party-services-and-shadow-ai.md) cubre el patrón opuesto de servicios de terceros sin control, y el [Capítulo 6](ch06-cybersecurity-in-the-ai-era.md) cubre lo básico de seguridad que sigue aplicándose a una máquina de tu propia oficina.

## Un poco de historia

**Años 90 y 2000: todo en casa.** Un pequeño negocio tenía un servidor en un armario. El correo, los archivos y las cuentas estaban todos en las propias instalaciones. Tú eras el dueño de la máquina y de todos sus problemas.

**Años 2000 a 2018: la mudanza.** La banda ancha se volvió rápida y alquilar resultó más fácil que poseer. El correo se fue primero, luego los archivos, después la contabilidad y los registros de clientes. "La nube" se volvió la respuesta por defecto. El chiste entre ingenieros era exacto: no hay nube, es solo el ordenador de otro.

**2013: los contenedores.** Llegó Docker y empaquetó el software para que funcionara igual en todas partes. Esto hizo que el alojamiento propio volviera a ser fácil, en silencio, porque ya no necesitabas un especialista para reinstalar una aplicación en cada máquina nueva.

**2022: la IA solo se alquilaba.** Los mejores modelos de lenguaje existían solo dentro de un puñado de grandes empresas. Si querías IA, tenías que enviarles tu texto. No había alternativa que valiera la pena.

**2023: el año de los modelos abiertos.** Meta publicó Llama como modelo de investigación en febrero, y luego Llama 2 con pesos abiertos en julio. Mistral AI publicó en agosto un modelo potente de siete mil millones de parámetros. "Pesos abiertos" significa que los archivos ya entrenados se publican, así que cualquiera puede descargarlos y ejecutarlos. Ese mismo año, la cuantización —comprimir un modelo para que necesite mucha menos memoria— quedó lo bastante buena para el uso diario. De pronto, una IA capaz ya no estaba solo en un centro de datos.

**8 de julio de 2023: Ollama.** Se publicó una herramienta llamada Ollama, de código abierto con licencia MIT, escrita principalmente en Go con algo de C y TypeScript, por Jeffrey Morgan y Michael Chiang. Su trabajo era eliminar toda la fricción. Un solo comando descarga un modelo y lo ejecuta en local, con una interfaz simple y un servicio local con el que otros programas pueden hablar. Usaba el motor llama.cpp para el trabajo real sobre tu hardware.

**2024: "soberano" se vuelve un criterio de compra.** Empresas de sectores regulados y varios gobiernos europeos empezaron a pedir una IA que se quedara dentro del país y dentro de sus propias paredes. Los proveedores de nube respondieron con opciones de nube soberana, y el mercado de la IA local creció rápido.

**2026: un cliente empresarial de código abierto.** En abril de 2026, MZLA Technologies, una filial de Mozilla, anunció Thunderbolt, un cliente de IA de código abierto hecho para alojarse uno mismo. La sección Curiosidad lo cubre.

La forma de esta historia es un bucle. Empezamos con alojamiento propio, nos mudamos por comodidad, y ahora estamos volviendo por control, con herramientas mucho mejores que la primera vez.

## Curiosidad

### 8.7 El cliente de IA de código abierto de Mozilla para "una IA que tú controlas"

En abril de 2026, MZLA Technologies Corporation —una filial de propiedad total de Mozilla, la organización sin ánimo de lucro detrás de Firefox— anunció **Thunderbolt**. Es un cliente de IA de código abierto y multiplataforma, hecho para organizaciones que quieren ejecutar la IA bajo sus propias reglas.

Los detalles que importan para este capítulo:

- **Alojable por ti mismo.** Se ejecuta en la infraestructura del propio cliente. El proyecto describe soporte para instalaciones locales, nube soberana y entornos aislados —es decir, una red físicamente desconectada de internet—.
- **Independiente del modelo.** Funciona con cualquier agente que hable el Agent Client Protocol, y con cualquier modelo que ofrezca una API compatible con OpenAI. En la práctica, puedes apuntarlo a un modelo local, a tu propio servidor o a un proveedor comercial, y cambiar sin cambiar tus herramientas.
- **En todas partes.** Web, Windows, macOS, Linux, iOS y Android.
- **Conectado a tus sistemas.** Se integra con sistemas empresariales a través del Model Context Protocol —una forma estándar de permitir que una herramienta de IA acceda a tus datos y acciones internas— y admite automatizaciones reutilizables y una API extensible.
- **Auditable.** Como el código es abierto, tú o un tercero pueden leerlo y comprobar qué hace de verdad. El proyecto ha dicho que está pasando por una auditoría de seguridad.
- **Socio para la soberanía europea.** Se acompaña de Haystack, de deepset, una plataforma de orquestación de código abierto, para despliegues soberanos en Europa.
- **Soporte incluido.** Ofrecen soporte empresarial e ingeniería desplegada en el sitio, esa parte que la mayoría de los proyectos de código abierto te deja resolver solo.

Vale la pena notar cómo se posiciona. El mensaje es "una IA que tú controlas", y el argumento es que la IA es demasiado importante para subcontratarla por completo. Es el mismo argumento que usa un pequeño negocio cuando decide guardar los archivos de nómina en su propia máquina en vez de en un servicio que nunca inspeccionó.

Un ejemplo más pequeño y antiguo de la misma idea vive en una aplicación de correo que mucha gente ya usa. El complemento ThunderAI para Thunderbird añadió soporte para modelos locales a través de Ollama en la versión 2.1.1, publicada en agosto de 2024. Con esa configuración el modelo se ejecuta en tu propio ordenador, así que el texto del correo nunca sale de la máquina, y no hace falta cuenta en la nube ni clave de API. Es una función pequeña, y deja el punto claro: la IA local ya no es un proyecto de investigación. Es una opción dentro de un cliente de correo gratuito.

## Un ejemplo de negocio real

### Hasta Apple construyó su propia nube

Apple es una empresa que podría alquilar casi cualquier cosa. En junio de 2024 anunció un sistema llamado Private Cloud Compute, creado para las funciones de IA de sus dispositivos cuando una tarea es demasiado grande para el propio teléfono. La lección está en lo que eligió hacer con ese sistema.

Apple construyó sus propios servidores alrededor de sus propios chips, con un sistema operativo endurecido. Diseñó el sistema para inferencia sin estado: procesar la solicitud, devolver la respuesta y no guardar nada. E hizo una promesa inusual: publicaría la imagen de software de cada versión de producción para que investigadores de seguridad externos pudieran inspeccionar exactamente qué se está ejecutando, y comprobar que la máquina con la que hablan es de verdad lo que dice ser. En octubre de 2024 Apple publicó una guía de seguridad e invitó a investigadores a atacar el sistema.

De esto se siguen tres cosas para un pequeño negocio.

Primero, fíjate en el razonamiento. Apple no construyó una nube porque no pudiera alquilar una. La construyó porque alquilar habría significado guardar los datos de los usuarios bajo las reglas de otro, y toda su marca se basa en no hacer eso. El control de la máquina valía para ellos dinero de verdad.

Segundo, fíjate en la idea de verificación. Publicar el software para que otros puedan comprobarlo es el mismo instinto de la auditoría de código abierto. La confianza se reduce haciendo el sistema inspeccionable, no prometiendo que se es bueno.

Tercero, fíjate en el tamaño de la distancia. Apple gastó una fortuna para llegar a "nosotros no guardamos nada". La mayoría de los pequeños negocios no pueden copiar eso. Pero sí puedes copiar la pregunta: *¿quién dirige la máquina a la que van mis datos, qué guardan, y alguien puede comprobarlo?* Si no puedes responder esas tres preguntas sobre una herramienta, no deberías meterle datos sensibles. Y si la respuesta honesta es "no podemos comprobarlo", un modelo que se ejecuta en tu propia máquina se vuelve una opción seria.

## Cómo hacerlo

### 8.5 Cómo empezar: de herramientas de código abierto como Ollama a los modelos locales

**Paso 1: Elige una tarea y una persona.**
No compres hardware primero. Elige una tarea repetitiva que involucre datos sensibles: resumir contratos, redactar respuestas a consultas estándar, convertir notas de reuniones en listas de tareas. Dásela a una persona curiosa con un buen ordenador.

**Paso 2: Instala Ollama.**
Ollama funciona en Windows, macOS y Linux. Después de instalarlo, un solo comando descarga un modelo e inicia un chat en tu terminal. Por dentro arranca un pequeño servicio en tu propia máquina, en el puerto 11434, con el que otros programas pueden hablar. Ese servicio local es lo que luego te permite conectar el modelo a tus propias herramientas.

**Paso 3: Elige el modelo por tamaño, no por nombre.**
El tamaño de los modelos se cuenta en parámetros, una medida aproximada de lo grande y capaz que es el modelo. Como regla general:

- **1 a 3 mil millones** — rápido y ligero, funciona en un portátil corriente. Bueno para resúmenes cortos y redacción simple.
- **7 a 9 mil millones** — el punto medio práctico. Buena calidad general; necesita una máquina decente con memoria suficiente.
- **70 mil millones o más** — mucho más potente, pero necesita hardware serio y mucha memoria. Normalmente no es un punto de partida para un pequeño negocio.

Busca versiones **cuantizadas**. La cuantización comprime los números dentro del modelo para que necesite mucha menos memoria y funcione más rápido, a cambio de una pequeña caída de calidad. Para la mayoría de las tareas de oficina, esa caída es aceptable.

**Paso 4: Añade una interfaz amigable.**
La terminal está bien para probar. Para el uso diario, añade una interfaz de chat que funcione en local, o conecta el modelo a una aplicación que la gente ya use —el complemento de Thunderbird mencionado arriba es un ejemplo—. El objetivo es que un compañero sin formación técnica pueda usarlo sin ayuda. Si solo una persona puede manejarlo, nunca se adoptará.

**Paso 5: Mantén que sea realmente local.**
Aquí es donde la gente falla. El servicio local debe escuchar solo en tu propia máquina, no en toda la red. Los investigadores de seguridad han encontrado muchos servidores de Ollama expuestos a internet porque estaban configurados para aceptar conexiones desde cualquier dirección. Así que: mantén la vinculación local por defecto, pon un cortafuegos delante, no abras nunca el puerto 11434 a internet, y no lo ejecutes con derechos de administrador. Una herramienta local no es automáticamente una herramienta segura.

**Paso 6: Deja que lea tus propios archivos.**
El siguiente paso más útil es la recuperación, a menudo llamada RAG. En palabras simples: en lugar de reentrenar el modelo, pones tus documentos en un índice buscable. Cuando alguien hace una pregunta, el sistema encuentra los pasajes relevantes y se los pasa al modelo junto con la pregunta. El modelo responde desde tus documentos. Nada se entrena con tus datos, y todo puede funcionar en tu propia máquina. Así es como consigues "pregúntale a nuestro manual" sin enviar el manual a ninguna parte.

**Paso 7: Escala solo cuando la prueba haya funcionado.**
Si la prueba piloto es útil, entonces compra hardware. Una estación de trabajo con una buena tarjeta gráfica es la respuesta habitual, porque la memoria gráfica es lo que limita cuán grande puede ser el modelo que ejecutas. Las máquinas de Apple con memoria unificada son una opción común por la misma razón. Un pequeño servidor tiene sentido cuando varias personas lo necesitan al mismo tiempo.

**Paso 8: Decide la división.**
La mayoría de las empresas acaban en un modelo híbrido. Los datos sensibles y las tareas rutinarias de gran volumen se ejecutan en local. El razonamiento difícil, los documentos muy largos y las funciones especializadas usan un servicio en la nube con un contrato en regla. Escribe la regla: qué datos van a dónde, y quién decide.

### 8.6 Casos de uso ideales

**Datos personales sensibles.** Historiales de salud, expedientes de personal, nóminas, currículums de candidatos, datos financieros de clientes. Si los datos no deben salir, procesarlos en local elimina la pregunta por completo.

**Información propia.** Diseños, planos, código fuente, documentos de licitaciones y ofertas, modelos de precios, planes estratégicos. Son los archivos que más dolerían si un proveedor se los quedara o los filtrara.

**Sectores regulados.** Sanidad, despachos legales, banca y seguros, gobierno y defensa, y cualquier negocio bajo reglas de residencia de datos que exijan que los datos se queden dentro de un país o región. El alojamiento propio convierte una conversación difícil de cumplimiento en una simple.

**Conectividad mala o nula.** Obras de campo, fábricas, barcos, minas, oficinas remotas, respuesta a emergencias. Un modelo local funciona cuando internet no.

**Trabajo repetitivo de gran volumen.** Miles de tickets, facturas o documentos. Un precio por solicitud duele en volumen; una máquina fija no crece.

**Experimentación barata.** Probar ideas sin un contador corriendo. Útil antes de comprometer presupuesto.

**Dónde encaja mal:** razonamiento de nivel frontera, documentos muy largos, generación avanzada de imágenes, y cualquier equipo sin ningún soporte técnico. Si nadie puede mantenerlo, no lo empieces.

## Ética y responsabilidad

El alojamiento propio resuelve un problema ético y crea otros. Ten claro cuál es cuál.

**Lo que resuelve.** Tus datos de clientes dejan de viajar a empresas que tú no elegiste, y no pueden usarse para entrenar el producto de otro sin tu permiso. Eso es una ganancia real de respeto hacia las personas cuyos datos guardas.

**Lo que no resuelve.** El modelo puede seguir estando equivocado, tener sesgos o inducir a error con total seguridad. Ejecutar un modelo sesgado en tu propio hardware no lo vuelve justo. Los deberes del [Capítulo 4](ch04-ethical-ai-doing-the-right-thing.md) siguen aplicándose, y también las reglas de divulgación del [Capítulo 5](ch05-rules-and-legal-responsibility.md).

**Lo que añade.** Ahora tú eres el operador. Aplicar parches, controlar el acceso, registrar y hacer copias de seguridad es tu trabajo. Si un servidor local sin parchear filtra datos, la responsabilidad es tuya de una forma nueva y muy directa.

**Supervisión de empleados.** Si registras las preguntas en un sistema local, ahora guardas un registro detallado de lo que pregunta tu personal. Ten una política escrita sobre qué se guarda, por qué, quién lo lee y durante cuánto tiempo. Mantén algo proporcional, y avísales.

**No vendas de más la soberanía.** "Soberano" es tanto una palabra de márketing como técnica. Si afirmas tener control pero no puedes parchear, hacer copias de seguridad ni auditar, la afirmación está vacía. Di lo que realmente tienes, y di con claridad lo que no.

**Energía.** Una máquina que ejecuta modelos todo el día consume electricidad. Lo local no es automáticamente más ecológico que un centro de datos grande y eficiente. Si afirmas un beneficio ambiental, compruébalo primero.

## Errores a evitar

1. **Comprar hardware antes de probar una tarea.** Prueba primero con un equipo alquilado o prestado. El hardware comprado con ilusiones se queda sin usar.
2. **Exponer el servicio local de IA a internet.** Es el error de alojamiento propio más común y más grave. Mantenlo local, ponle cortafuegos, no abras el puerto.
3. **Suponer que local equivale a seguro.** Ahora la seguridad de esa máquina es tuya, incluidas las partes en las que nunca pensaste.
4. **Sin copias de seguridad.** La máquina, los modelos, la configuración y el índice de documentos necesitan copia de seguridad.
5. **Elegir el modelo más grande.** Más grande es más lento, más voraz y a menudo no es mejor para tu tarea real.
6. **Ignorar las licencias de los modelos.** Los modelos de pesos abiertos vienen con condiciones distintas, incluidas reglas sobre el uso comercial y sobre cómo puedes describir tu uso. Lee la licencia antes de construir sobre ella.
7. **Depender de una sola persona.** Si una persona sabe cómo funciona y se va, el sistema se detiene. Escribe los pasos de instalación, reinicio y restauración.
8. **Alojar en local la carga equivocada.** Si la tarea necesita calidad de frontera, lo local decepcionará, y concluirás en falso que la tecnología no sirve.
9. **Nunca actualizar, o actualizar sin probar.** Una nueva versión del modelo cambia las respuestas. Vuelve a ejecutar tus tareas de muestra después de cada cambio.
10. **Tratarlo como todo o nada.** Una configuración híbrida suele ser la respuesta correcta, no una mudanza total en cualquier dirección.

## Ejercicio práctico

### 8.8 Evalúa si el alojamiento propio conviene a tu empresa

Puntúa cada fila con 0, 1 o 2. Sé honesto.

| Pregunta | 0 | 1 | 2 |
|---|---|---|---|
| ¿Qué tan sensibles son los datos? | Públicos | Internos | Confidenciales de clientes o regulados |
| Soporte técnico disponible | Ninguno | Ayuda de TI a tiempo parcial | Alguien que pueda mantener un servidor |
| Presupuesto de hardware | Ninguno | Una buena estación de trabajo | Estación de trabajo más un pequeño servidor |
| Complejidad de la tarea | Resúmenes y redacción | Preguntas sobre documentos | Razonamiento complejo, documentos muy largos |
| Conectividad | Poca fiable | Bien | Bien |
| Volumen | Ocasional | Diario | Alto y creciente |

Lee la puntuación fila por fila, porque las filas no todas empujan en la misma dirección.

- **Sensibilidad 2** y **Volumen 2** empujan hacia el alojamiento propio.
- **Soporte técnico 0** empuja fuertemente en contra, sea cual sea el resto de puntuaciones.
- **Complejidad de la tarea 2** empuja en contra, porque los modelos locales se quedan atrás en el razonamiento difícil.

Ahora haz una prueba de un día antes de gastar nada. Toma veinte tareas reales de tu lista. Haz diez con un modelo local de tamaño medio y diez con un servicio en la nube. Compara tres cosas: si la respuesta era suficientemente buena para usarse tal cual, cuánto tardó, y cuánto habría costado del otro modo. Escribe los resultados.

Si la respuesta local era utilizable para la mayoría de las tareas, el alojamiento propio vale la inversión. Si solo era utilizable para unas pocas, quédate esas en local y deja el resto en la nube con un contrato. De cualquier modo, ahora tienes evidencia en vez de una opinión.

## Lista de verificación

### 8.9 Lo que necesitas para empezar

- [ ] **Una tarea concreta** que involucre datos sensibles y se repita a menudo.
- [ ] **Una persona concreta** que pueda instalar, reiniciar, respaldar y actualizar el sistema, o un plan para contratar a alguien.
- [ ] **Una máquina con memoria suficiente**, elegida después de una prueba, no antes.
- [ ] **Un modelo elegido por tamaño y cuantización**, acorde a la tarea y no al más grande disponible.
- [ ] **Una interfaz local** que un compañero sin formación técnica pueda usar sin ayuda.
- [ ] **El servicio vinculado solo a la máquina local**, con cortafuegos y sin ningún puerto abierto a internet.
- [ ] **Una revisión escrita de la licencia** del modelo que elijas, incluidas las condiciones de uso comercial.
- [ ] **Un plan de copias de seguridad** para la máquina, los modelos, la configuración y el índice de documentos.
- [ ] **Una rutina de parches** con fecha fija, y una nueva prueba de las tareas de muestra después de cada cambio.
- [ ] **Una regla escrita de división** que diga qué datos se quedan en local y cuáles pueden usar un servicio en la nube, y quién decide.

## Puntos clave

- El alojamiento propio significa que la IA se ejecuta en máquinas que tú controlas, así que tus datos no salen de ellas.
- Se volvió práctico para los pequeños negocios cuando llegaron los modelos de pesos abiertos y la buena compresión en 2023, y herramientas como Ollama eliminaron la fricción de la configuración.
- Cambias capacidad y comodidad por control: el triángulo es control, capacidad y coste, y no puedes tener los tres.
- Lo local no es automáticamente seguro ni barato; un servidor local mal configurado es un riesgo real, y el mantenimiento ahora es tu trabajo.
- Empieza con una tarea, una persona y una prueba de un día antes de comprar cualquier hardware.
