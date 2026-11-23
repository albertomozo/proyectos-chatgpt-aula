# Prompt 07 Crear un tablero Kanban (plantilla 13)

**Entradas:** DOC-03, DOC-02, CTX-00 y decisiones; DOC-07 si ya existe.  
**Salida:** DOC-07 como diseño de tablero. **Revisión humana:** asignaciones y reglas de flujo.

Abre un chat nuevo dentro de tu proyecto y copia el bloque completo. Las instrucciones del proyecto y el índice deben estar configurados. Los datos nuevos pueden añadirse después del bloque. En modo compacto, los documentos DOC se consultan dentro de `99-EXPEDIENTE.md`.

```text
Consulta el índice, CTX-00, DOC-02, DOC-03 y DOC-05; revisa DOC-07 si existe. Transforma las tareas del cronograma aprobado en una propuesta de tablero Kanban. Si el plan es provisional, identifica el tablero como propuesta de preparación, sin afirmar que la ejecución está autorizada.

Usa herramienta, columnas y límite WIP definidos en CTX-00. Si faltan, propón Pendiente, En curso, Revisión y Hecho; plantea un WIP provisional justificado por la capacidad conocida o deja su valor pendiente.

Crea tarjetas: TAR | título | ENT | responsable | prioridad | dependencia | criterio de terminado | fecha objetivo | estado y evidencia del estado. Para tareas nuevas sin prueba de ejecución, usa Pendiente. Si ya hay tablero, conserva los estados comprobados y señala la fecha de corte.

Define reglas de movimiento, bloqueos, prioridades, revisión y WIP. Entrega tabla Markdown adaptable a la herramienta. No afirmes haber creado o actualizado un tablero externo.

Entrega DOC-07 con versión o corte y traspaso con filas propuestas del índice. No cambies fechas o compromisos aprobados.
```

Antes del siguiente chat: revisa el resultado, conserva su versión y actualiza las fuentes y el índice.

[Volver al listado de prompts](README.md).
