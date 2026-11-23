# Prompt 06 Auditoría cruzada de coherencia del plan

**Entradas:** DOC-01 a DOC-04; CTX-00 y DOC-05 para contexto y aprobaciones.  
**Salida:** DOC-06 / AUD-PLAN. **Revisión humana:** resolver hallazgos y decidir sobre el inicio de ejecución.

Abre un chat nuevo dentro de tu proyecto y copia el bloque completo. Las instrucciones del proyecto y el índice deben estar configurados. Los datos nuevos pueden añadirse después del bloque. En modo compacto, los documentos DOC se consultan dentro de `99-EXPEDIENTE.md`.

```text
Realiza una auditoría cruzada del proyecto identificado en CTX-00. Consulta el índice, DOC-01 acta, DOC-02 alcance, DOC-03 cronograma, DOC-04 riesgos y las decisiones y aprobaciones de DOC-05. Comprueba el contenido y la versión de cada fuente; diferencia línea base y borradores.

Contrasta objetivos OBJ, requisitos REQ, entregables ENT, tareas TAR, responsables, fechas, disponibilidad, presupuesto, riesgos y criterios de aceptación con sus pruebas PRU.

Detecta tareas sin vínculo o justificación; entregables sin tareas; requisitos sin cobertura; dependencias incompatibles; sobreasignación; riesgos sin propietario; hitos inviables según los datos; incoherencias de costes; criterios sin pruebas, muestra o aceptante; decisiones no aprobadas; y divergencias entre versiones o denominaciones.

No califiques como error probado lo que sea un dato ausente, una hipótesis o una mejora opcional. No declares una desviación real sin datos reales comparables.

Entrega DOC-06 con instancia AUD-PLAN y:
1. Fuentes consultadas, no accesibles y no aportadas, con versión y estado.
2. Tabla: documento y versión | inconsistencia o pendiente | gravedad | evidencia y apartado | corrección sugerida | quién debe validarla o aprobarla.
3. Trazabilidad: OBJ/REQ | ENT | TAR | responsable | PRU/criterio | situación y carencias.
4. Dependencias justificadas; separa lo comprobado de la secuencia propuesta.
5. Condiciones de paso a ejecución: condición | evidencia requerida | situación | persona competente. Usa «aprobación no acreditada», «pendiente de comprobación» o «con evidencia» según corresponda. No autorices ni deniegues tú la ejecución.
6. Comprobaciones que no pueden completarse y prioridades para resolverlas.

Si falta un documento, limita expresamente la auditoría; no inventes fechas, dependencias, responsables o resultados. No modifiques originales. Incluye traspaso y filas propuestas del índice.
```

Antes del siguiente chat: revisa el resultado, conserva su versión y actualiza las fuentes y el índice.

[Volver al listado de prompts](README.md).
