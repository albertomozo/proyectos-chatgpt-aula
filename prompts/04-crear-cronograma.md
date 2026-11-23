# Prompt 04 Desglosar tareas y crear cronograma (plantilla 07)

**Entradas:** DOC-01, DOC-02, CTX-00 y DOC-05; línea base aprobada cuando exista.  
**Salida:** DOC-03. **Revisión humana:** duraciones, disponibilidad, dependencias y fechas.

Abre un chat nuevo dentro de tu proyecto y copia el bloque completo. Las instrucciones del proyecto y el índice deben estar configurados. Los datos nuevos pueden añadirse después del bloque. En modo compacto, los documentos DOC se consultan dentro de `99-EXPEDIENTE.md`.

```text
Consulta el índice, CTX-00, DOC-01, DOC-02 y las decisiones de DOC-05. Identifica las versiones aprobadas y los borradores utilizados.

Prepara DOC-03 desglosando cada entregable ENT en tareas TAR: descripción | ENT y REQ vinculados | responsable | esfuerzo estimado | duración | disponibilidad considerada | dependencia y tipo | inicio | fin | criterio de finalización. Añade hitos y calendario utilizado.

Distingue esfuerzo de duración. Fundamenta las dependencias; identifica tareas paralelizables, cuellos de botella y conflictos de disponibilidad. Comprueba que cada entregable tenga tareas y que las tareas de gestión tengan una justificación identificada.

Si faltan fecha de inicio, calendario o dedicación, presenta duraciones y secuencia relativa como propuesta; deja las fechas absolutas pendientes. No certifiques el plazo ni inventes capacidad. Si hay conflicto con fechas aprobadas, muestra alternativas sujetas a decisión, sin sustituirlas.

Entrega tabla Markdown, supuestos y comprobaciones. Si añades un diagrama, usa código Mermaid limpio en bloque mermaid, sin CSS, SVG ni estilos copiados del navegador.

Termina con traspaso y filas propuestas para el índice. DOC-03 queda en borrador hasta la decisión correspondiente.
```

Antes del siguiente chat: revisa el resultado, conserva su versión y actualiza las fuentes y el índice.

[Volver al listado de prompts](README.md).
