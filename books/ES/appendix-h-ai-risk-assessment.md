# Apéndice H — Evaluación de riesgos de la IA

Antes de lanzar un proyecto de IA, pregúntate qué podría salir mal y qué tan grave sería. Esta tabla hace visibles los riesgos para que puedas reducirlos, no ignorarlos. Rellénala con tu equipo. Hazlo pronto y revísala a menudo.

## Cómo puntuar

Valora cada riesgo en dos escalas:

- **Probabilidad** — ¿Qué tan probable es? **Baja / Media / Alta**
- **Impacto** — ¿Qué tan grave si ocurre? **Bajo / Medio / Alto**

Combínalos en un **Nivel de riesgo**:

| | Impacto Bajo | Impacto Medio | Impacto Alto |
|---|---|---|---|
| **Probabilidad Alta** | Medio | Alto | **Crítico** |
| **Probabilidad Media** | Bajo | Medio | Alto |
| **Probabilidad Baja** | Bajo | Bajo | Medio |

Trata **Crítico** y **Alto** como obligatorio de corregir antes del lanzamiento.

## Plantilla en blanco

| Riesgo | Qué podría salir mal | Probabilidad | Impacto | Nivel de riesgo | Mitigación | Responsable |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Ejemplos rellenados

| Riesgo | Qué podría salir mal | Probabilidad | Impacto | Nivel de riesgo | Mitigación | Responsable |
|---|---|---|---|---|---|---|
| Datos erróneos en la IA | El personal pega datos personales de clientes en una herramienta pública | Alta | Alto | **Crítico** | Lista de solo-herramientas-aprobadas; bloquear herramientas públicas en dispositivos de la empresa; formación | Responsable de TI |
| Resultado erróneo usado | La IA redacta una factura con un importe incorrecto, enviada al cliente | Media | Alto | Alto | Revisión humana antes de enviar; comprobación automática de totales | Administrativo de contabilidad |
| Sesgo en las decisiones | Una herramienta de contratación favorece a un grupo por datos de entrenamiento sesgados | Media | Alto | Alto | Decide un humano; revisar los resultados por equidad; evitar la contratación totalmente automatizada | Responsable de RR. HH. |
| Fuga del proveedor | Al proveedor lo vulneran y los datos de clientes quedan expuestos | Baja | Alto | Medio | Lista de comprobación del proveedor; cifrar datos; cláusula de aviso de brecha en el contrato | Responsable de TI |
| Dependencia excesiva | El personal deja de comprobar y confía ciegamente en la IA | Media | Medio | Medio | Mantener la firma humana; auditorías puntuales; formación sobre los límites | Manager del equipo |
| Inyección de prompt | Un documento esconde instrucciones que engañan a la IA | Media | Medio | Medio | Tratar el texto externo como no confiable; limitar lo que la IA puede hacer con él | Responsable de TI |
| Dependencia del proveedor | No se puede abandonar al proveedor ni exportar los datos | Baja | Medio | Medio | Cláusula de exportación de datos en el contrato; guardar una copia | Propietario |
| Exceso de coste | El uso crece y la factura se dispara | Media | Medio | Medio | Poner alertas de uso; revisar el plan cada mes; limitar el coste por tarea | Propietario |
| Deriva del modelo | El proveedor cambia el modelo y baja la calidad del resultado | Media | Medio | Medio | Comprobar el resultado puntualmente cada semana; guardar casos de prueba para comparar | Manager del equipo |

## Guía de las columnas

- **Riesgo** — Un nombre corto para el riesgo.
- **Qué podría salir mal** — El escenario concreto, no una preocupación vaga.
- **Probabilidad / Impacto** — Bajo / Medio / Alto.
- **Nivel de riesgo** — De la cuadrícula de arriba.
- **Mitigación** — Qué harás para bajar la probabilidad o el impacto.
- **Responsable** — La única persona que se asegura de que la mitigación se haga.

## Riesgos comunes de la IA a considerar

Usa esta lista para inspirar tus propias filas:

- [ ] Fuga de datos personales o sensibles a una herramienta externa.
- [ ] Resultado incorrecto en el que se confía sin revisión.
- [ ] Sesgo o injusticia en decisiones automatizadas.
- [ ] Brecha de seguridad del proveedor.
- [ ] Inyección de prompt desde documentos no confiables.
- [ ] IA en la sombra (personal usando herramientas no aprobadas).
- [ ] Dependencia excesiva y pérdida de habilidades.
- [ ] Exceso de coste a medida que crece el uso.
- [ ] Dependencia de un solo proveedor.
- [ ] Incumplimiento del GDPR o del Reglamento de IA de la UE.
- [ ] Pérdida de confianza del cliente tras un error visible.
- [ ] Cambios silenciosos del modelo y bajada de la calidad del resultado.

## Cuándo volver a ejecutar esta evaluación

Revisa la tabla cuando ocurra cualquiera de esto:

- Añades una nueva herramienta, fuente de datos o proceso.
- El uso crece mucho, o la herramienta toca a más personas.
- Ocurre un incidente o un casi-incidente.
- Cambia una ley o un requisito del cliente.
- Un proveedor cambia sus condiciones, su modelo o dónde almacena los datos.

## Dos formas de reducir un riesgo

Cada mitigación tira de uno de dos resortes:

- **Bajar la probabilidad** — hacer que el evento malo sea menos probable de ocurrir. Ejemplo: una lista de solo-herramientas-aprobadas hace menos probable una fuga de datos.
- **Bajar el impacto** — hacer que el daño sea menor si ocurre. Ejemplo: la revisión humana hace que una factura errónea se detecte antes de llegar al cliente.

Un buen plan suele tirar de ambos. Pregúntate por cada riesgo: "¿Qué hace esto menos probable, y qué limita el daño si aun así ocurre?"

Si un riesgo sigue **Crítico** incluso tras la mitigación, no lo lances. Elimina el paso arriesgado o rediseña el proceso.

## Reglas

- Cada riesgo Crítico o Alto necesita una mitigación **y** un responsable antes del lanzamiento.
- Una mitigación sin responsable no es una mitigación.
- Vuelve a ejecutar esta evaluación en cada hito: los riesgos cambian.
- Si un riesgo Crítico no se puede reducir, no lo lances. Dilo.
