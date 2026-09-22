# Apéndice M — Recursos, lecturas y herramientas recomendadas

Una lista corta y honesta de herramientas y lecturas. **No** son anuncios. Son proyectos reales y con nombre que puedes investigar por tu cuenta. La mayoría es de código abierto, lo que significa que puedes ver cómo funcionan y no quedas atado a una sola empresa.

**Una nota sobre el nivel de habilidad:** Algunas herramientas de aquí necesitan a una persona técnica (un socio de informática, un desarrollador o una contratación con conocimientos técnicos). Tú no necesitas ejecutarlas tú mismo. Léelas para saber qué es posible y para hablar con criterio con quien las configure.

**Verificado:** Cada herramienta y libro de abajo se comprobó contra su propio sitio web o repositorio de código en **septiembre de 2026**. Las herramientas cambian rápido — vuelve a comprobarlas antes de adoptarlas.

## Ejecuta la IA en local (en tus propias máquinas)

Ejecutar los modelos en local significa que la IA funciona en tu propio ordenador o servidor. Tus datos no salen de tu máquina. Esta es la opción más privada.

- **Ollama** — `ollama.com`. Una herramienta gratuita y de código abierto para ejecutar modelos de IA abiertos en tu propio ordenador. Los modelos locales no cuestan nada y mantienen los datos en tu máquina. Es el punto de partida más fácil para la IA local y a menudo se usa como motor detrás de otras herramientas.
- **Thunderbolt** — `thunderbolt.io` (código: `github.com/Thunderbird/thunderbolt`). Un **cliente de IA** de código abierto y autoalojable de MZLA Technologies, la filial de Mozilla que también crea Thunderbird. Anunciado en abril de 2026 y con licencia Mozilla Public License 2.0. Su promesa es "IA que tú controlas: elige tus modelos, sé dueño de tus datos, elimina la dependencia del proveedor". Funciona en web, Windows, macOS, Linux, iOS y Android, y funciona con modelos locales, en servidor propio o en la nube. Para uso local apunta a Ollama o llama.cpp. **Estado:** está en fase inicial y bajo una auditoría de seguridad — trátalo como prometedor, no terminado.
- **llama.cpp** — un motor de código abierto muy conocido que ejecuta modelos grandes en hardware de ordenador corriente, incluido tu propio portátil. Es el motor técnico sobre el que otros construyen. Se menciona aquí porque Thunderbolt lo recomienda para inferencia local gratuita.

**Cuándo elegir lo local:** manejas datos sensibles, quieres evitar comisiones por mensaje, o necesitas que la IA funcione sin enviar datos hacia fuera. La compensación: pagas el hardware y la configuración, y los modelos locales suelen ser más pequeños que los mayores modelos en la nube.

## Crea automatizaciones (conecta la IA a tu trabajo)

Estas herramientas te permiten integrar la IA en tareas reales — leer documentos, responder tickets, mover datos entre aplicaciones.

- **Haystack** — `haystack.deepset.ai` (código: `github.com/deepset-ai/haystack`). Un framework de código abierto de **deepset** (Alemania) para crear aplicaciones de IA, especialmente pipelines de **RAG**. RAG ("generación aumentada por recuperación") significa que la IA consulta tus propios documentos antes de responder, así que responde con tus hechos, no con suposiciones. Gratis para instalar (`pip install haystack-ai`); el soporte empresarial de pago es opcional. Lo mejor para un equipo con un desarrollador.
- **n8n** — `n8n.io`. Una plataforma de automatización **fair-code** (el código es público en GitHub) que te permite crear flujos de trabajo en un lienzo visual y conectarte a más de 500 aplicaciones. También crea agentes de IA y sistemas RAG, con aprobaciones con intervención humana. Puedes autoalojarla o usar su nube. "Fair-code" significa que el código es abierto para leerlo y autoalojarlo, pero no es una licencia de código abierto estándar — revisa los términos si planeas revenderla.

**Cuándo elegir estas:** quieres que la IA actúe sobre tus datos en varias aplicaciones, no solo chatear. Haystack es para construir pipelines de IA a medida; n8n es para conectar aplicaciones y automatizar pasos con IA dentro de ellas.

## Aprende más (lecturas)

- **Headcount Zero: How to Build an AI-Run Company with Paperclip** — de **Anthony David Adams**. Un libro de código abierto (en GitHub, licencia CC BY-NC-SA 4.0) sobre dirigir una empresa donde los agentes de IA hacen la mayor parte del trabajo y un pequeño número de humanos juzgan el resultado. Trata la idea de la "empresa de una sola persona", cómo funcionan los agentes de IA, la economía de tener pocos empleados y cómo gobernar la IA con interruptores de parada. Léelo por la visión audaz — y luego aplícalo con la cautela que este libro enseña: mantén a los humanos al mando de lo que importa.
- **Los propios capítulos de este libro** — la mejor "lectura adicional" suelen ser los capítulos que hojeaste. Relee el capítulo de riesgo antes de cualquier lanzamiento, y el capítulo de datos antes de conectar cualquier herramienta a datos reales de clientes.
- **Documentación de proveedores y proyectos** — para cualquier herramienta de arriba, lee la documentación y la licencia del propio proyecto antes de adoptarla. Te dice qué es gratis, qué es de pago y a qué te comprometes.

## Cómo elegir, en tres preguntas

1. **¿Dónde deben quedarse los datos?** Si no deben salir de tus máquinas, mira las herramientas locales (Ollama, Thunderbolt, llama.cpp).
2. **¿Cuentas con ayuda técnica?** Si sí, Haystack y n8n abren más puertas. Si no, empieza con una herramienta alojada sencilla y una pequeña prueba piloto.
3. **¿Puedes irte más tarde?** Prefiere herramientas que te permitan exportar tus datos y cambiar de modelo. Evita cualquier cosa que encarcele tus datos.

## Una advertencia sobre listas como esta

Las herramientas suben y bajan. Un nombre de aquí puede cambiar, fusionarse o desvanecerse en un año. Eso es normal en la IA. Los **principios** de este libro — mantener los datos privados, mantener a un humano en el ciclo, medir resultados y evitar la dependencia — duran más que cualquier herramienta individual. Usa esta lista como un mapa, no como una promesa.
