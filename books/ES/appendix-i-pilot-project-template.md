# Apéndice I — Plantilla de proyecto piloto

Un piloto es una prueba pequeña y barata que responde a una sola pregunta: ¿esto funciona para nosotros? Manténgalo acotado, con fecha límite y honesto. Este plan de una página contiene todo lo que necesitas. Rellénalo antes de empezar y juzga el resultado contra él al final.

## Cómo usarlo

1. Elige **un** proceso (de tu mapa de procesos) con alto potencial y alto dolor.
2. Rellena cada campo de abajo. Si no puedes rellenarlo, el piloto no está listo.
3. Fija una fecha de fin y una regla de decisión clara.
4. Ejecútalo, mide y luego decide: escalar, cambiar o detener.

---

## Plan del piloto

**Nombre del piloto:** ______________________  **Fecha de inicio:** ______  **Fecha de fin:** ______

### 1. Objetivo (una frase)

¿Qué único problema resuelve este piloto?

> Ejemplo: "Reducir el tiempo de procesamiento de facturas entrantes de 12 minutos a menos de 4 minutos, sin más errores."

Tu objetivo: ______________________________________________________

### 2. Proceso elegido

- **Proceso:** ______________________ (enlace a la fila de tu mapa de procesos)
- **Por qué este:** ______________________
- **Responsable:** ______________________

### 3. Antes (línea base)

Mide el estado actual **antes** de empezar. Sin una línea base, no puedes demostrar una mejora.

| Medida | Valor actual |
|---|---|
| Tiempo por ejecución |  |
| Ejecuciones por semana |  |
| Tasa de error |  |
| Coste por ejecución |  |
| Satisfacción del personal (1–5) |  |

### 4. Después (objetivo)

| Medida | Valor objetivo |
|---|---|
| Tiempo por ejecución |  |
| Ejecuciones por semana |  |
| Tasa de error |  |
| Coste por ejecución |  |
| Satisfacción del personal (1–5) |  |

### 5. Criterios de éxito (cómo decidimos)

Escribe 2–4 condiciones claras y comprobables. Sé específico.

- [ ] Ejemplo: El tiempo por ejecución es inferior a 4 minutos.
- [ ] Ejemplo: La tasa de error no es peor que antes.
- [ ] Ejemplo: El personal dice que es más fácil (puntuación ≥ 4).
- [ ] Ejemplo: Ningún incidente de datos o seguridad.

### 6. Herramientas

- **Herramienta de IA:** ______________________
- **Sistemas conectados:** ______________________
- **Proveedor / plan:** ______________________
- **Coste durante el piloto:** ______________________

### 7. Cronograma

| Semana | Qué sucede |
|---|---|
| 1 | Configuración, conexión, línea base confirmada |
| 2–3 | Ejecución con trabajo real, revisión humana de cada resultado |
| 4 | Medir, recopilar comentarios |
| 5 | Decidir |

### 8. Equipo

| Rol | Persona | Responsabilidad |
|---|---|---|
| Responsable del piloto |  | Dirige el piloto, informa del resultado |
| Ejecutor |  | Usa la herramienta a diario, da comentarios |
| Revisor |  | Comprueba los errores en los resultados |
| TI / seguridad |  | Configura de forma segura, vigila el riesgo |

### 9. Riesgos (los 3 principales, de tu evaluación de riesgos)

| Riesgo | Mitigación | Responsable |
|---|---|---|
|  |  |  |
|  |  |  |
|  |  |  |

### 10. Regla de decisión

Acuerda esto **antes** de empezar, para que la elección no sea emocional más adelante.

- **Escalar** si: se cumplen todos los criterios de éxito y ningún riesgo Crítico/Alto está abierto.
- **Cambiar y reintentar** si: se cumplen algunos criterios y la corrección está clara. Plantea un nuevo piloto corto.
- **Detener** si: no se alcanza el objetivo, el coste supera el beneficio o aparece un riesgo grave.

**Decisión tomada el:** ______  **Decisión:** ☐ Escalar ☐ Reintentar ☐ Detener
**Motivo:** ______________________________________________________

---

## Ejemplo resumido (un piloto terminado)

- **Objetivo:** Reducir el procesamiento de facturas de 12 a menos de 4 minutos, sin errores extra.
- **Proceso:** Procesar facturas entrantes (del mapa de procesos).
- **Antes:** 12 min/ejecución, 40/semana, 6% de tasa de error.
- **Después (objetivo):** 3 min/ejecución, 40/semana, tasa de error ≤6%.
- **¿Éxito alcanzado?** Tiempo 3,1 min ✓, errores 5% ✓, puntuación del personal 4 ✓, sin incidentes ✓.
- **Coste durante el piloto:** 600 €.
- **Decisión:** Escalar — todos los criterios cumplidos, ningún riesgo Alto abierto.
- **Siguiente paso:** Desplegar para todas las facturas; mantener la revisión humana en importes superiores a 5.000 €.

## Qué hacer después del piloto

- **Si escalas:** planifica el despliegue más amplio, mantén la revisión donde el riesgo es alto, fija una fecha de revisión.
- **Si reintentas:** anota qué falló, cambia una cosa, ejecuta un nuevo piloto corto.
- **Si detienes:** registra el porqué, para que la lección se conserve y no se repita.
- Comparte el resultado con el equipo en cualquier caso. Un piloto fallido que enseñó algo es un buen uso de un presupuesto pequeño.

## Reglas del piloto

- Manténgalo pequeño: un proceso, un equipo, unas pocas semanas.
- Un humano revisa cada resultado durante el piloto.
- Mide primero la línea base — nunca te saltes esto.
- Un piloto que falla de forma barata es un éxito: aprendiste sin una gran pérdida.
- Escribe el resultado y compártelo, sea bueno o malo.
