# Prompt 11 Verificar la coherencia tras un cambio

**Entradas:** DOC-05 con decisión verificable, DOC-10 pertinente, versiones anteriores y propuestas actualizadas.  
**Salida:** DOC-06 / REV-CAMBIO y matriz de actualizaciones. **Revisión humana:** aplicación exacta de lo autorizado.

Abre un chat nuevo dentro de tu proyecto y copia el bloque completo. Las instrucciones del proyecto y el índice deben estar configurados. Los datos nuevos pueden añadirse después del bloque. En modo compacto, los documentos DOC se consultan dentro de `99-EXPEDIENTE.md`.

```text
Consulta el índice y localiza en DOC-05 la decisión humana de cambio que se solicita comprobar, junto con DOC-10, la línea base anterior y los documentos actualizados disponibles. Identifica CAM, DEC, alcance de la aprobación, persona o rol, fecha y versiones afectadas. Si hay varias decisiones, solicita el ID.

Si no consta decisión expresa o no pueden consultarse las versiones necesarias, limita el trabajo a una propuesta o revisión parcial; no presentes la actualización como aprobada.

Contrasta objetivos, requisitos, entregables, DOC-03 cronograma, DOC-07 Kanban, DOC-04 riesgos, presupuesto, criterios de aceptación y DOC-09 seguimiento. Comprueba también dependencias y coherencia de fechas.

Entrega DOC-06 con instancia REV-CAMBIO y tabla: documento/versión anterior | decisión que lo afecta | cambio exacto autorizado | actualización propuesta o comprobada | versión nueva conocida o sugerida | responsable | comprobación pendiente.

Separa «aprobado», «aplicado con evidencia» y «pendiente de aplicar». Un cambio aprobado no significa que sus archivos o herramientas externas ya se hayan actualizado. No amplíes el cambio aprobado ni sobrescribas fuentes en esta revisión.

Incluye traspaso y filas propuestas del índice que conserven el histórico y solo reflejen aprobaciones acreditadas.
```

Antes del siguiente chat: revisa el resultado, conserva su versión y actualiza las fuentes y el índice.

[Volver al listado de prompts](README.md).
