# Prompt 00 Configurar el contexto y el registro documental

**Entradas:** ficha inicial del índice, datos de este mensaje y fuentes existentes. No exige documentos previos aprobados.  
**Salidas:** CTX-00, propuesta de índice actualizado y registro inicial DOC-05 si todavía no existe.  
**Revisión humana:** identidad del proyecto, datos iniciales, correspondencia de archivos y autoridad de aprobación.

Abre un chat nuevo dentro de tu proyecto y copia el bloque completo. Las instrucciones del proyecto y el índice deben estar configurados. Los datos nuevos pueden añadirse después del bloque. En modo compacto, los documentos DOC se consultan dentro de `99-EXPEDIENTE.md`.

```text
Inicializa el trabajo de este proyecto utilizando las instrucciones del proyecto y 00-INDICE-DOCUMENTAL.md. Lee la ficha inicial y los documentos efectivamente accesibles. Si no hay índice, propone uno con el catálogo de esta biblioteca.

Prepara CTX-00: denominación oficial, organización, problema, descripción, destinatarios, objetivo preliminar, criterios de éxito, fechas y calendario, presupuesto y moneda, recursos y dedicación, personas y roles, entregables, restricciones, exclusiones, metodología, herramientas y modalidad real o didáctica.

Distingue datos declarados, hechos verificables, propuestas y pendientes. No resuelvas contradicciones entre fuentes sin señalarlas. Prioriza hasta cinco preguntas imprescindibles; deja los demás datos como PENDIENTE.

Relaciona cada archivo existente con su código, nombre exacto, versión y estado comprobados. No atribuyas aprobaciones a partir del nombre o de una versión 1.0. Si hay códigos anteriores, propone una tabla de equivalencias sin renumerar por tu cuenta.

Entrega por separado:
A) CTX-00-contexto-v0.1.md en borrador, o revisión propuesta si ya existe.
B) Propuesta completa de 00-INDICE-DOCUMENTAL.md, conservando las versiones y aprobaciones existentes.
C) Registro inicial DOC-05 solo si falta; sin decisiones ficticias.
D) Traspaso al siguiente chat con pendientes, fuentes que guardar y siguiente prompt recomendado.

Todavía no redactes el acta ni el resto del plan.
```

Antes del siguiente chat: revisa el resultado, conserva su versión y actualiza las fuentes y el índice.

[Volver al listado de prompts](README.md).
