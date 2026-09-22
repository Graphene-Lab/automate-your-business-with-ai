# Apéndice D — Inventario de datos

No puedes proteger datos que no puedes encontrar. Este inventario enumera cada elemento de datos importante que tu negocio posee, dónde vive y quién puede alcanzarlo. Rellénalo antes de conectar cualquier herramienta de IA. Si un dato no está en esta lista, no se lo des a la IA.

## Cómo usarlo

1. Recorre tus herramientas: correo, unidades, contabilidad, CRM, sistemas de RR. HH., hojas de cálculo.
2. Añade una fila por elemento de datos (una lista de clientes, un archivo de nóminas, una carpeta de contratos).
3. Marca cada elemento **Personal** (relacionado con una persona) o **Sensible** (categorías especiales — ver abajo).
4. Revisa el acceso: quién puede abrirlo hoy, y quién *debería* poder hacerlo.
5. Revísalo antes de cualquier proyecto de IA. Esta lista te dice qué es seguro usar y qué no.

## Plantilla en blanco

| Elemento de datos | Dónde se almacena | Responsable | ¿Personal / Sensible? | Quién puede acceder | Estado de respaldo | Retención |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Ejemplo relleno

| Elemento de datos | Dónde se almacena | Responsable | ¿Personal / Sensible? | Quién puede acceder | Estado de respaldo | Retención |
|---|---|---|---|---|---|---|
| Lista de contactos de clientes | CRM (nube) | Gerente de ventas | Personal (nombres, correos, teléfonos) | Equipo de ventas (editar), Finanzas (leer) | Diario, fuera del sitio | Mantener mientras esté activo + 3 años |
| Archivo de nóminas | Unidad compartida, carpeta "RR. HH." | Responsable de RR. HH. | Sensible (salario, identificación, banco) | Solo RR. HH. | Semanal, fuera del sitio | 10 años (legal) |
| Contratos de proveedores | Archivador de papel + carpeta escaneada | Dueño | Ninguno (confidencial de negocio) | Dueño, Finanzas | Parcial (solo escaneos) | Vida del contrato + 6 años |

## Dónde buscar datos

Recorre cada uno de estos. Los datos se esconden a plena vista:

- [ ] Bandejas de correo compartidas y buzones personales.
- [ ] Unidades compartidas y carpetas de red.
- [ ] Herramientas en la nube: CRM, contabilidad, RR. HH., herramientas de proyecto.
- [ ] Hojas de cálculo y adjuntos (a menudo lo más desordenado).
- [ ] Archivos en papel, archivadores y copias escaneadas.
- [ ] Copias de seguridad y exportaciones viejas.
- [ ] Herramientas de chat e historial de mensajería.
- [ ] Teléfonos y portátiles del personal.
- [ ] Herramientas de terceros en las que el personal se registró por su cuenta (copias en la sombra).

## Qué cuenta como "Sensible"

Bajo el RGPD, estas categorías especiales necesitan un cuidado extra. Márcalas claramente:

- Datos de salud
- Origen racial o étnico
- Opiniones políticas
- Creencias religiosas o filosóficas
- Afiliación sindical
- Datos genéticos y biométricos (para identificación)
- Vida sexual u orientación sexual

Trata también como sensible, aunque no sea "categoría especial": datos bancarios, números de identificación, contraseñas, datos de niños, y cualquier cosa que pueda dañar a una persona si se filtra.

## Guía de columnas

- **Elemento de datos** — Un nombre claro para la cosa (no el nombre del archivo).
- **Dónde se almacena** — Sistema y ubicación: herramienta en la nube, ruta de la unidad, archivador de papel.
- **Responsable** — Una persona responsable de ello.
- **¿Personal / Sensible?** — Personal, Sensible o Ninguno.
- **Quién puede acceder** — Roles o personas, y si pueden leer o editar.
- **Estado de respaldo** — Con qué frecuencia se respalda, y dónde. Anota si **no** hay respaldo.
- **Retención** — Cuánto tiempo lo guardas, y por qué (regla legal o necesidad del negocio).

## Señales de alarma a arreglar ahora

- [ ] Datos sensibles sin responsable.
- [ ] Datos sensibles que cualquiera en la empresa puede abrir.
- [ ] Datos importantes sin respaldo.
- [ ] Datos guardados "para siempre" sin razón.
- [ ] Datos personales en una herramienta que no controlas (IA en la sombra, correo personal).
- [ ] Los mismos datos en muchos lugares sin una copia maestra.

## Reglas prácticas de retención

- Guarda los datos solo el tiempo que los necesites. Más tiempo no es más seguro — es más riesgo.
- Revisa los mínimos legales: los registros fiscales y de nómina suelen tener años fijos. Pregunta a tu contable.
- Para datos de clientes, guárdalos mientras la relación esté activa, y luego un período corto y declarado.
- Borra o anonimiza los datos que ya no necesites. No dejes que se acumulen.
- Escribe la razón de cada período de retención, para que nadie tenga que adivinar más tarde.

## Mantener el inventario actualizado

- Revísalo cada 6 meses, y antes de cualquier nuevo proyecto de IA.
- Añade una fila el día que aparezca una nueva herramienta o fuente de datos.
- Nombra un responsable por elemento; los responsables lo mantienen honesto.
- Trátalo como un documento vivo, no una tarea de una sola vez.

## Regla para proyectos de IA

Antes de que cualquier dato entre en una herramienta de IA, revisa este inventario. Si un elemento es **Sensible**, necesitas una razón clara, una herramienta segura, y a menudo una DPIA. Cuando dudes, déjalo fuera.
