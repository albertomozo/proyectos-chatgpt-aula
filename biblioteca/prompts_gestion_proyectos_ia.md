# Biblioteca de prompts: gestión de proyectos con inteligencia artificial

**Versión:** 2.0 · **Fecha:** 22/11/2026  
**Formato:** Markdown portable · **Ámbito:** proyectos de distintos sectores, tamaños y metodologías  
**Modo de trabajo:** un prompt por chat nuevo dentro del mismo proyecto de ChatGPT; contexto y documentos compartidos mediante las fuentes del proyecto.

## 1. Qué cambia respecto a la versión 1.0

Se mantienen los **16 prompts, numerados del 00 al 15**, sus fases y las referencias opcionales a las plantillas 02, 05, 07, 10, 13, 16, 22 y 24. Se sustituye la copia repetida de documentos por un índice documental y códigos estables. Los datos generales se introducen una vez en CTX-00; después solo se aportan novedades o evidencias que todavía no estén disponibles como fuentes.

Cada prompt especifica entradas, salida y revisión. Las reglas comunes se configuran una vez en las instrucciones del proyecto. Cada ejecución deja un traspaso para el siguiente chat: documento, versión, pendientes y filas propuestas para actualizar el índice.

Esta biblioteca es reutilizable. **No contiene una auditoría verificada de INCIDENCIAS AULA**: para realizarla hay que consultar sus documentos originales. Los nombres, fechas, estados y conclusiones comunicados en una conversación son datos declarados hasta contrastarlos con las fuentes.

## 2. Preparación: una sola vez por proyecto

1. Crea o utiliza un proyecto de ChatGPT dedicado al proyecto de gestión. Fija una denominación oficial; si aparecen variantes como «INCIDENCIAS AULA» y «Resolución de Incidencias AULA», registra la equivalencia y confirma cuál prevalece.
2. Copia el bloque de `01-INSTRUCCIONES-PROYECTO.md` en las instrucciones del proyecto. El texto completo figura también en el anexo A de esta biblioteca.
3. Añade esta biblioteca y `00-INDICE-DOCUMENTAL.md` a las fuentes del proyecto. Cumplimenta la ficha inicial del índice con lo conocido; deja el resto como PENDIENTE.
4. Añade los documentos existentes. Registra su nombre exacto, código, versión, estado y aprobación comprobable. No necesitas renombrarlos para empezar.
5. Abre un chat nuevo dentro del proyecto, ejecuta el Prompt 00 y revisa CTX-00 y el índice resultantes. Añade esas versiones revisadas a las fuentes antes del siguiente chat.

Las fuentes pueden incluir archivos o respuestas guardadas. Según la ayuda oficial de OpenAI, puedes guardar una respuesta desde su menú con **Añadir a las fuentes del proyecto**. También puedes guardar el Markdown como archivo y añadirlo. Las instrucciones se introducen en **Ajustes del proyecto**. La denominación de los controles puede variar. Consulta: [Proyectos en ChatGPT — OpenAI](https://help.openai.com/es-es/articles/10169521-projects-in-chatgpt), comprobado el 22/11/2026.

**Límite del método:** los códigos no son enlaces automáticos y el índice no garantiza acceso. Cada chat debe comprobar las fuentes necesarias. Guardar una respuesta como fuente tampoco equivale a aprobarla, actualizar el índice o sustituir una versión anterior.

## 3. Ciclo de trabajo: un prompt por chat

1. Abre un chat nuevo dentro del mismo proyecto. Nombre sugerido: `04 · Cronograma · revisión 01`.
2. Copia el bloque del prompt elegido. No hace falta volver a pegar acta, alcance o cronograma. Si hay datos nuevos, añádelos al mensaje o aporta una fuente identificada.
3. Comprueba la tabla de fuentes consultadas: ¿se ha utilizado la versión correcta? Si falta un archivo, añádelo y continúa ese trabajo.
4. Revisa y corrige el resultado. Cuando corresponda una aprobación, la persona competente debe aprobar una versión exacta y dejar evidencia accesible en DOC-05.
5. Guarda el documento revisado como fuente del proyecto, con código, título, versión y estado. Guarda también el índice actualizado. Las propuestas de actualización no se aplican por sí solas.
6. Abre el siguiente chat cuando las fuentes necesarias estén disponibles. Puedes seguir preparando borradores aunque queden decisiones pendientes, siempre que se identifiquen como provisionales.

**No es necesario aprobar todos los documentos ni detener toda la preparación.** Separa el trabajo de elaboración de las decisiones que requieren autorización. No presentes un plan provisional como línea base ni una revisión de la IA como autorización de ejecución.

Si una decisión solo existe en un chat, guarda la declaración humana relevante como fuente accesible, con fecha, persona o rol y versión afectada. No te apoyes únicamente en un resumen generado por la IA.

## 4. Correspondencia única de códigos

| Código | Documento | Prompts que lo producen o revisan |
|---|---|---|
| CTX-00 | Contexto y ficha del proyecto | 00 |
| DOC-01 | Acta de constitución | 01–02 |
| DOC-02 | Alcance y entregables | 03 |
| DOC-03 | Cronograma | 04 |
| DOC-04 | Matriz de riesgos | 05 |
| DOC-05 | Registro de decisiones y aprobaciones | Inicialización en 00; mantenimiento cuando haya decisiones |
| DOC-06 | Revisiones y auditorías | 02, 06 y 11; una instancia por revisión |
| DOC-07 | Tablero Kanban o exportación fechada | 07; propuestas de actualización en 08 y 11 |
| DOC-08 | Incidencias y evidencias | 08 |
| DOC-09 | Informes de seguimiento | 09; una instancia por fecha de corte |
| DOC-10 | Solicitudes de cambio y análisis | 10; una instancia por CAM |
| DOC-11 | Checklist y acta de aceptación y cierre | 12; cumplimentación posterior con pruebas y decisión humana |
| DOC-12 | Lecciones aprendidas | 14 |
| DOC-13 | Expediente final | 15 |
| SIM-01 | Cierre de simulación didáctica | 13, opcional |

El código identifica el documento; la versión identifica una revisión. Los informes repetidos añaden una instancia: `DOC-06 / AUD-PLAN-001 / v0.1`. Una auditoría inicial y una revisión tras un cambio son informes distintos, no versiones del mismo informe.

**Si ya utilizas otros códigos**, conserva la identificación existente y crea una tabla de equivalencias antes de aplicar esta biblioteca. No reasignes DOC-05 o DOC-06 a documentos distintos según la fase.

## 5. Contexto y novedades: qué introducir

La ficha CTX-00 reúne los datos que en la versión 1.0 se pegaban como variables: nombre, organización, descripción, problema, destinatarios, objetivo, fechas, presupuesto, recursos, responsables, entregables, restricciones, exclusiones, criterios de éxito, metodología y herramientas. El idioma por defecto es español y la salida es Markdown. El índice complementario incluye una ficha lista para cumplimentar.

No necesitas rellenar nuevas variables para cada prompt. Para los trabajos recurrentes, basta con aportar lo que aún no figure en las fuentes:

| Prompt | Novedad mínima, si no está registrada |
|---|---|
| 08 | Incidencia concreta, fecha, hechos observados y evidencias |
| 09 | Fecha de corte y datos reales de tareas, hitos y costes |
| 10 | Solicitud de cambio concreta y motivo |
| 11 | Decisión humana y versiones afectadas |
| 12 | Evidencias de pruebas y aceptación disponibles |
| 13 | Resultados expresamente simulados por el docente |
| 14 | Resultados comprobados y aportaciones reales del equipo |

Un campo desconocido es PENDIENTE, no un supuesto aceptado. Las estimaciones se presentan como propuestas a validar. Una fuente operativa debe tener fecha de corte para no confundir un estado antiguo del tablero con el actual.

---

# Fase 0 · Preparación

## Prompt 00 — Configurar el contexto y el registro documental

**Entradas:** ficha inicial del índice, datos de este mensaje y fuentes existentes. No exige documentos previos aprobados.  
**Salidas:** CTX-00, propuesta de índice actualizado y registro inicial DOC-05 si todavía no existe.  
**Revisión humana:** identidad del proyecto, datos iniciales, correspondencia de archivos y autoridad de aprobación.

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

# Fase 1 · Inicio

## Prompt 01 — Elaborar el acta de constitución (plantilla 02)

**Entradas:** CTX-00, índice y decisiones aplicables de DOC-05. Si existe DOC-01, se prepara una revisión identificada.  
**Salida:** DOC-01 en borrador. **Revisión humana:** viabilidad preliminar y decisiones de constitución.

```text
Consulta 00-INDICE-DOCUMENTAL.md, CTX-00 y las decisiones aplicables de DOC-05. Identifica las fuentes utilizadas. Redacta DOC-01, acta de constitución del proyecto identificado en CTX-00, o una revisión propuesta si ya existe.

Incluye problema y justificación, objetivo SMART propuesto, beneficios, alcance preliminar, exclusiones, entregables, hitos, presupuesto, recursos y dedicación, roles, riesgos iniciales y tres criterios de éxito medibles.

Respeta los datos y decisiones comprobados. Si una fecha está vencida, un coste no está confirmado o falta una persona responsable, señálalo; plantea alternativas como propuestas, sin sustituir lo aprobado. Distingue rol funcional y persona asignada. No conviertas un objetivo de coste cero en presupuesto aprobado.

Entrega acta Markdown con cabecera documental y estado BORRADOR, datos y autorizaciones pendientes, comprobaciones para la persona o rol aprobador y apartado de aprobación sin cumplimentar.

Añade el traspaso al siguiente chat y las filas propuestas para el índice. No generes firmas ni autorices el proyecto.
```

## Prompt 02 — Revisar el inicio y preparar la decisión

**Entradas:** DOC-01 de trabajo, CTX-00 y DOC-05 si existe.  
**Salida:** DOC-06 / REV-INICIO, informe de revisión. **Revisión humana:** correcciones y eventual aprobación de DOC-01 exacto.

```text
Consulta el índice y revisa la versión de trabajo identificada de DOC-01. Contrástala con CTX-00 y las decisiones accesibles de DOC-05. Si hay varias versiones sin selección clara, pide identificar cuál revisar.

Comprueba el objetivo SMART, la coherencia entre alcance, entregables, fechas, presupuesto, disponibilidad y responsables, y la posibilidad de verificar los criterios de éxito. No afirmes que el objetivo es alcanzable si faltan recursos o dedicaciones.

Genera DOC-06 con una instancia REV-INICIO identificada y tabla: hallazgo | tipo (inconsistencia, dato pendiente o propuesta) | gravedad alta/media/baja | evidencia con documento, versión y apartado | corrección propuesta | responsable de validación conocido o pendiente.

Separa inconsistencias comprobadas, supuestos y preguntas esenciales. Explica qué debe resolver la persona competente antes de aprobar el acta. Si no consta aprobación, indica «aprobación no acreditada»; no declares por tu cuenta una prohibición o autorización.

No modifiques DOC-01. Entrega traspaso, filas propuestas del índice y, cuando proceda, propuesta de entrada en DOC-05 sin inventar la decisión.
```

# Fase 2 · Planificación

## Prompt 03 — Definir alcance y entregables (plantilla 05)

**Entradas:** DOC-01 aprobado como referencia preferente; CTX-00 y DOC-05. Si el acta sigue en borrador, salida provisional.  
**Salida:** DOC-02. **Revisión humana:** requisitos, exclusiones y aceptación.

```text
Consulta el índice, CTX-00, DOC-01 y DOC-05. Elabora DOC-02, alcance y entregables, utilizando la versión aprobada aplicable de DOC-01. Si solo hay borrador, puedes preparar una propuesta provisional e indicar qué decisiones impiden consolidarla.

Define alcance del producto y trabajo del proyecto, inclusiones, exclusiones, requisitos REQ, supuestos y restricciones. Conserva los IDs existentes y asigna IDs ENT a los nuevos entregables.

Tabla: entregable | requisitos vinculados | descripción | responsable funcional y persona confirmada o pendiente | dependencias justificadas | criterio de aceptación verificable | prueba o evidencia requerida | quién acepta.

Concreta, cuando corresponda, procedimiento de prueba, muestra propuesta y condiciones de éxito. Identifica lo que aún necesita validación. No impongas una cadena lineal por el orden de los entregables ni añadas funcionalidades como compromisos aprobados.

Entrega DOC-02 en borrador con cabecera y puntos de conformidad, seguido del traspaso y las filas propuestas para el índice. No alteres el acta ni la línea base.
```

## Prompt 04 — Desglosar tareas y crear cronograma (plantilla 07)

**Entradas:** DOC-01, DOC-02, CTX-00 y DOC-05; línea base aprobada cuando exista.  
**Salida:** DOC-03. **Revisión humana:** duraciones, disponibilidad, dependencias y fechas.

```text
Consulta el índice, CTX-00, DOC-01, DOC-02 y las decisiones de DOC-05. Identifica las versiones aprobadas y los borradores utilizados.

Prepara DOC-03 desglosando cada entregable ENT en tareas TAR: descripción | ENT y REQ vinculados | responsable | esfuerzo estimado | duración | disponibilidad considerada | dependencia y tipo | inicio | fin | criterio de finalización. Añade hitos y calendario utilizado.

Distingue esfuerzo de duración. Fundamenta las dependencias; identifica tareas paralelizables, cuellos de botella y conflictos de disponibilidad. Comprueba que cada entregable tenga tareas y que las tareas de gestión tengan una justificación identificada.

Si faltan fecha de inicio, calendario o dedicación, presenta duraciones y secuencia relativa como propuesta; deja las fechas absolutas pendientes. No certifiques el plazo ni inventes capacidad. Si hay conflicto con fechas aprobadas, muestra alternativas sujetas a decisión, sin sustituirlas.

Entrega tabla Markdown, supuestos y comprobaciones. Si añades un diagrama, usa código Mermaid limpio en bloque mermaid, sin CSS, SVG ni estilos copiados del navegador.

Termina con traspaso y filas propuestas para el índice. DOC-03 queda en borrador hasta la decisión correspondiente.
```

## Prompt 05 — Elaborar la matriz de riesgos (plantilla 10)

**Entradas:** DOC-01 a DOC-03, CTX-00 y DOC-05; DOC-08 si hay incidencias.  
**Salida:** DOC-04. **Revisión humana:** valoraciones, medidas y propietarios.

```text
Consulta el índice, CTX-00, DOC-01, DOC-02, DOC-03 y DOC-05; consulta DOC-08 si existe. Prepara o revisa DOC-04 con los riesgos pertinentes al proyecto: técnicos, organizativos, costes, plazos, calidad, seguridad y aceptación, entre otros cuando apliquen.

Usa la escala definida en CTX-00. Si no hay otra, propón probabilidad e impacto de 1 a 5, nivel P×I y bandas alta 15–25, media 6–14, baja 1–5. Explica brevemente la escala; las puntuaciones son valoraciones iniciales a validar, no probabilidades observadas.

Tabla: RIE | riesgo y causa | ENT o TAR afectados | probabilidad | impacto | nivel | prevención | contingencia | indicador de alerta | propietario funcional | persona asignada o pendiente.

Distingue riesgos futuros de incidencias ocurridas. No inventes propietarios nominales. Si falta el cronograma, deja pendiente el contraste sobre plazos y tareas afectadas; continúa con los riesgos que sí puedan analizarse.

Entrega borrador de DOC-04, prioridades, validaciones y traspaso con filas propuestas del índice.
```

## Prompt 06 — Auditoría cruzada de coherencia del plan

**Entradas:** DOC-01 a DOC-04; CTX-00 y DOC-05 para contexto y aprobaciones.  
**Salida:** DOC-06 / AUD-PLAN. **Revisión humana:** resolver hallazgos y decidir sobre el inicio de ejecución.

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

# Fase 3 · Ejecución y organización ágil

## Prompt 07 — Crear un tablero Kanban (plantilla 13)

**Entradas:** DOC-03, DOC-02, CTX-00 y decisiones; DOC-07 si ya existe.  
**Salida:** DOC-07 como diseño de tablero. **Revisión humana:** asignaciones y reglas de flujo.

```text
Consulta el índice, CTX-00, DOC-02, DOC-03 y DOC-05; revisa DOC-07 si existe. Transforma las tareas del cronograma aprobado en una propuesta de tablero Kanban. Si el plan es provisional, identifica el tablero como propuesta de preparación, sin afirmar que la ejecución está autorizada.

Usa herramienta, columnas y límite WIP definidos en CTX-00. Si faltan, propón Pendiente, En curso, Revisión y Hecho; plantea un WIP provisional justificado por la capacidad conocida o deja su valor pendiente.

Crea tarjetas: TAR | título | ENT | responsable | prioridad | dependencia | criterio de terminado | fecha objetivo | estado y evidencia del estado. Para tareas nuevas sin prueba de ejecución, usa Pendiente. Si ya hay tablero, conserva los estados comprobados y señala la fecha de corte.

Define reglas de movimiento, bloqueos, prioridades, revisión y WIP. Entrega tabla Markdown adaptable a la herramienta. No afirmes haber creado o actualizado un tablero externo.

Entrega DOC-07 con versión o corte y traspaso con filas propuestas del índice. No cambies fechas o compromisos aprobados.
```

## Prompt 08 — Analizar una incidencia y proponer acciones

**Entradas:** DOC-08, DOC-07, DOC-04 y plan aplicable. Aportar solo la incidencia nueva si aún no figura en las fuentes.  
**Salida:** borrador actualizado de DOC-08 y propuesta de acciones sobre DOC-07. **Revisión humana:** hechos, responsables y resolución.

```text
Consulta el índice, DOC-08, DOC-07, DOC-04 y las versiones aplicables de DOC-01 a DOC-03 y DOC-05. Analiza la incidencia indicada en este mensaje o la única entrada pendiente de análisis identificable en DOC-08. Si hay varias sin selección clara, pide su ID; si falta la descripción, solicita el dato mínimo antes de diagnosticarla.

Identifica INC, fecha, situación real o simulada, hechos observados, fuentes y efectos comprobados. Si falta estado actualizado del tablero, indica el corte disponible y limita las conclusiones.

Analiza causas posibles e impacto en alcance, calidad, plazos, costes y usuarios. Separa hechos de hipótesis. Propón contención, investigación, corrección y comprobación: acción | TAR/ENT afectados | responsable confirmado o propuesto | prioridad | fecha propuesta | evidencia necesaria | criterio de resolución.

Propón tarjetas que añadir, bloquear o mover sin inventar su estado real. Indica decisiones que requieren autorización y si procede evaluar un cambio con el Prompt 10. Relaciona riesgos RIE e incidencia INC sin confundirlos.

Entrega la actualización propuesta de DOC-08, los cambios propuestos a DOC-07 y el traspaso con filas del índice. No afirmes que las acciones se ejecutaron ni que la incidencia está resuelta sin evidencia.
```

# Fase 4 · Seguimiento

## Prompt 09 — Generar el informe de estado (plantilla 16)

**Entradas:** plan aprobado, DOC-07, DOC-08, DOC-04, DOC-05 y datos reales con fecha de corte.  
**Salida:** DOC-09, instancia por corte. **Revisión humana:** exactitud de avances, desviaciones y decisiones pendientes.

```text
Consulta el índice y prepara el informe DOC-09 para la fecha de corte indicada en este mensaje o en la fuente operativa seleccionada. Si no hay fecha de corte inequívoca, pídela antes de fechar resultados. No uses automáticamente la fecha del chat como corte de los datos.

Contrasta las versiones aprobadas aplicables de DOC-01 a DOC-03 con DOC-07, DOC-08, DOC-04, DOC-05 y las evidencias disponibles de pruebas, hitos y gastos. Identifica la fecha de cada dato y cualquier desfase respecto al corte. Sin datos reales, entrega una estructura parcial identificada como tal.

Incluye resumen ejecutivo, entregables verificados, desviaciones, riesgos, bloqueos, próximos pasos y decisiones pendientes. Usa semáforo verde/ámbar/rojo con criterio y evidencia; añade «sin datos suficientes» cuando no sea posible valorarlo.

Tabla Previsto | Real | Desviación | Fuente y corte solo cuando los datos sean comparables. Distingue coste cero verificado de ausencia de información. No inventes porcentajes ni declares Hecho por una estimación o por el mero movimiento de una tarjeta sin el criterio de terminado exigido.

Entrega DOC-09 como borrador con instancia y corte exactos, fuentes y limitaciones, seguido del traspaso y las filas propuestas para el índice.
```

# Fase 5 · Control y adaptación

## Prompt 10 — Evaluar alternativas y solicitudes de cambio

**Entradas:** solicitud concreta, DOC-09, línea base, DOC-04, DOC-05 y DOC-10 si existe.  
**Salida:** DOC-10 / CAM, análisis sin decisión automática. **Revisión humana:** opción y autorización.

```text
Consulta el índice, CTX-00, la línea base aplicable de DOC-01 a DOC-03, DOC-04, DOC-05 y el informe DOC-09 pertinente. Analiza la solicitud de cambio indicada en este mensaje o una solicitud identificada de DOC-10. Si no puede determinarse cuál, pide ID y motivo.

Registra CAM, solicitante conocido o pendiente, motivo, situación actual y versiones afectadas. Distingue una solicitud, una desviación observada y una decisión ya aprobada.

Compara al menos tres opciones cuando existan: mantener el plan; ajustar tareas o recursos; modificar alcance o fecha sujeto a aprobación. No fuerces alternativas inviables. Para cada opción, presenta impacto en alcance, plazo, presupuesto, calidad, riesgos y carga de trabajo, ventajas, límites, datos necesarios y quién debe decidir.

Recomienda una opción condicionada a la evidencia. Explica qué documentos requerirían revisión y qué aceptación adicional sería necesaria.

Entrega DOC-10 como análisis en borrador, con decisión pendiente salvo evidencia humana expresa. No cambies la línea base. Termina con traspaso y filas propuestas del índice.
```

## Prompt 11 — Verificar la coherencia tras un cambio

**Entradas:** DOC-05 con decisión verificable, DOC-10 pertinente, versiones anteriores y propuestas actualizadas.  
**Salida:** DOC-06 / REV-CAMBIO y matriz de actualizaciones. **Revisión humana:** aplicación exacta de lo autorizado.

```text
Consulta el índice y localiza en DOC-05 la decisión humana de cambio que se solicita comprobar, junto con DOC-10, la línea base anterior y los documentos actualizados disponibles. Identifica CAM, DEC, alcance de la aprobación, persona o rol, fecha y versiones afectadas. Si hay varias decisiones, solicita el ID.

Si no consta decisión expresa o no pueden consultarse las versiones necesarias, limita el trabajo a una propuesta o revisión parcial; no presentes la actualización como aprobada.

Contrasta objetivos, requisitos, entregables, DOC-03 cronograma, DOC-07 Kanban, DOC-04 riesgos, presupuesto, criterios de aceptación y DOC-09 seguimiento. Comprueba también dependencias y coherencia de fechas.

Entrega DOC-06 con instancia REV-CAMBIO y tabla: documento/versión anterior | decisión que lo afecta | cambio exacto autorizado | actualización propuesta o comprobada | versión nueva conocida o sugerida | responsable | comprobación pendiente.

Separa «aprobado», «aplicado con evidencia» y «pendiente de aplicar». Un cambio aprobado no significa que sus archivos o herramientas externas ya se hayan actualizado. No amplíes el cambio aprobado ni sobrescribas fuentes en esta revisión.

Incluye traspaso y filas propuestas del índice que conserven el histórico y solo reflejen aprobaciones acreditadas.
```

# Fase 6 · Cierre y aprendizaje

## Prompt 12 — Preparar checklist de aceptación y cierre (plantilla 22)

**Entradas:** DOC-02 aprobado, DOC-05, DOC-08, DOC-09 y evidencias de pruebas; DOC-11 si existe.  
**Salida:** DOC-11. **Revisión humana:** conformidad por entregable y decisión de aceptación y cierre.

```text
Consulta el índice, DOC-02 y sus criterios aprobados, DOC-05, DOC-08, DOC-09, DOC-11 si existe y las evidencias de prueba identificadas. Prepara o actualiza DOC-11, checklist y propuesta de acta de aceptación y cierre.

Tabla: ENT | REQ/criterio | PRU y procedimiento | muestra prevista y ejecutada | evidencia accesible | resultado (cumple/no cumple/pendiente) | quién ejecuta | quién acepta | observaciones.

No marques cumple sin evidencia suficiente. Diferencia prueba funcional satisfactoria, aceptación humana y cierre administrativo; ninguna implica automáticamente las otras. Registra los defectos abiertos y sus efectos sobre la aceptación.

Añade documentación, permisos, seguridad, transferencia a operación y acciones posteriores cuando correspondan al alcance. Identifica qué puede aceptarse y qué requiere decisión, sin emitirla tú.

Si existe decisión humana verificable de aceptación, referencia exactamente su alcance y versión; si no, deja la aceptación y la firma pendientes. No declares cerrado el proyecto por completar la tabla.

Entrega DOC-11 con cabecera, fuentes y traspaso con filas propuestas del índice.
```

## Prompt 13 — Elaborar cierre con resultados simulados, opcional

**Entradas:** alcance y criterios; resultados expresamente simulados aportados por la persona docente.  
**Salida:** SIM-01, separado del expediente real. **Omitir en el cierre de un proyecto real.**

```text
Realiza exclusivamente una SIMULACIÓN DIDÁCTICA. Consulta el índice, DOC-02 y la estructura de DOC-11 si existe. Usa los resultados simulados expresamente aportados por la persona docente en este mensaje o en una fuente identificada. Si no se han aportado, pide el conjunto mínimo antes de cumplimentar resultados.

Genera SIM-01: ejemplo de checklist e informe de aceptación, con cabecera y marcas visibles SIMULADO en cada resultado, evidencia y decisión ficticia. No generes firmas aparentemente auténticas.

Distingue requisitos técnicos, resultados de negocio, incidencias pendientes y acciones posteriores. No actualices DOC-11 real, DOC-05 ni la línea base con estos resultados. No uses simulaciones para acreditar pruebas o aceptación reales.

Añade traspaso indicando que SIM-01 solo debe guardarse como material didáctico y propone su fila del índice con estado SIMULADO, fuera de la línea base real.
```

## Prompt 14 — Redactar lecciones aprendidas (plantilla 24)

**Entradas:** objetivos aprobados, DOC-08, DOC-09, DOC-05, DOC-11 y aportaciones del equipo.  
**Salida:** DOC-12. **Revisión humana:** contraste de aprendizajes con el equipo.

```text
Consulta el índice, los objetivos y versiones aplicables de DOC-01 y DOC-02, DOC-08, DOC-09, DOC-05, DOC-11 y las aportaciones reales del equipo registradas como fuentes o facilitadas en este mensaje.

Prepara DOC-12, retrospectiva en borrador. Identifica qué funcionó, qué no funcionó, causas posibles, decisiones útiles, herramientas y metodología empleadas y mejoras para proyectos futuros.

Tabla: situación | evidencia y fuente | aprendizaje o hipótesis | acción de mejora | responsable propuesto | comprobación futura.

No atribuyas opiniones no expresadas ni conviertas recomendaciones en hechos observados. Si el cierre no está aceptado o faltan resultados, identifica el documento como retrospectiva parcial y deja los resultados pendientes. Excluye SIM-01 de las evidencias reales; si todo el ejercicio es didáctico, etiqueta el conjunto como simulado.

Finaliza con cinco preguntas para contrastar el borrador con el equipo y con traspaso y filas propuestas para el índice.
```

# Fase 7 · Documentación y archivo

## Prompt 15 — Preparar el expediente final del proyecto

**Entradas:** índice, CTX-00 y versiones verificables de DOC-01 a DOC-12 que existan.  
**Salida:** DOC-13. **Revisión humana:** integridad del expediente y estado real del cierre.

```text
Consulta 00-INDICE-DOCUMENTAL.md, CTX-00 y las versiones identificadas de DOC-01 a DOC-12 que estén accesibles. Prioriza versiones aprobadas para compromisos y decisiones, y registros revisados con corte identificado para los hechos operativos. No ignores un pendiente vigente por existir un informe anterior más favorable.

Prepara DOC-13 con:
1. Índice del expediente: código | instancia | documento o archivo exacto | versión | fecha/corte | responsable | estado | aprobación y evidencia | ubicación comprobada.
2. Resumen ejecutivo de máximo 300 palabras, salvo otra extensión indicada.
3. Trazabilidad: OBJ | REQ | ENT | TAR o hito | PRU y evidencia de aceptación | resultado verificado.
4. Documentos ausentes o inaccesibles, discrepancias, cambios no aplicados, incidencias abiertas y autorizaciones pendientes.
5. Registro de uso de IA: tareas asistidas, revisión humana comprobada o pendiente y limitaciones.
6. Estado documental de cierre sustentado en DOC-11 y DOC-05, sin anunciar un cierre autorizado si no consta.

Identifica borradores e histórico; separa SIM-01 y todo material didáctico de la evidencia real. No inventes archivos, enlaces, rutas, resultados o firmas. Una referencia en el índice sin contenido accesible se marca no comprobada.

Entrega DOC-13 en borrador y traspaso final con filas propuestas para actualizar el índice y pendientes para completar el expediente. No afirmes que has archivado archivos o cerrado el proyecto por generar este documento.
```

---

## 6. Índice rápido y peticiones breves

Estos atajos sirven cuando ya están configuradas las instrucciones, el índice y esta biblioteca como fuentes. Si el asistente no puede consultar el prompt, pega su bloque completo. «Ejecuta» significa realizar la tarea documental, no actuar automáticamente en herramientas externas.

| Prompt | Chat sugerido | Petición breve | Resultado |
|---|---|---|---|
| 00 | Contexto e índice | Ejecuta el Prompt 00 de la biblioteca para este proyecto. | CTX-00 e índice |
| 01 | Acta | Ejecuta el Prompt 01 con CTX-00. | DOC-01 |
| 02 | Revisión del inicio | Ejecuta el Prompt 02 sobre DOC-01 de trabajo. | DOC-06 / REV-INICIO |
| 03 | Alcance | Ejecuta el Prompt 03 usando el acta aplicable. | DOC-02 |
| 04 | Cronograma | Ejecuta el Prompt 04 con DOC-01 y DOC-02. | DOC-03 |
| 05 | Riesgos | Ejecuta el Prompt 05 con el plan disponible. | DOC-04 |
| 06 | Auditoría del plan | Ejecuta el Prompt 06 de DOC-01 a DOC-04 y contrasta DOC-05. | DOC-06 / AUD-PLAN |
| 07 | Kanban | Ejecuta el Prompt 07 con DOC-03. | DOC-07 |
| 08 | Incidencia | Ejecuta el Prompt 08 sobre la incidencia que indico a continuación. | DOC-08 y acciones propuestas |
| 09 | Seguimiento | Ejecuta el Prompt 09 para la fecha de corte que indico. | DOC-09 / corte |
| 10 | Cambio | Ejecuta el Prompt 10 sobre la solicitud que indico. | DOC-10 / CAM |
| 11 | Revisión tras cambio | Ejecuta el Prompt 11 sobre la decisión DEC que indico. | DOC-06 / REV-CAMBIO |
| 12 | Aceptación y cierre | Ejecuta el Prompt 12 con las evidencias disponibles. | DOC-11 |
| 13 | Simulación | Ejecuta el Prompt 13 con estos resultados expresamente simulados. | SIM-01 |
| 14 | Lecciones | Ejecuta el Prompt 14 con los resultados y aportaciones disponibles. | DOC-12 |
| 15 | Expediente | Ejecuta el Prompt 15 con las versiones registradas y accesibles. | DOC-13 |

Los prompts 08 a 11 pueden repetirse cuando haya incidencias, cortes o cambios nuevos; no son pasos obligatorios una sola vez. El 13 es opcional. El 12 puede repetirse para incorporar pruebas y aceptación humana posteriores.

## 7. Cabecera documental y traspaso comunes

Incluye esta cabecera en cada documento producido, con los datos conocidos. El nombre sugerido debe incluir código y versión; en documentos recurrentes, también instancia o corte. Por ejemplo: `DOC-06-AUD-PLAN-001-v0.1.md`.

```text
Código / instancia:
Proyecto y denominación oficial:
Título:
Versión / fecha / fecha de corte si procede:
Estado: BORRADOR, salvo evidencia aplicable de otro estado
Responsable conocido o PENDIENTE:
Fuentes consultadas: código, instancia, archivo exacto, versión, estado y apartado
Fuentes no accesibles o no aportadas:
Relación con la versión anterior y cambios:
Aprobación: persona/rol, fecha, alcance, versión y evidencia, o NO CONSTA
```

Termina la respuesta con un bloque separado del documento, para facilitar guardarlo como fuente sin mezclarlo con indicaciones operativas:

```text
TRASPASO AL SIGUIENTE CHAT
Documento producido: código, instancia, versión, estado y nombre sugerido.
Fuentes que debes guardar: documento revisado, evidencias y decisiones nuevas.
Actualización propuesta del índice: filas completas que añadir o modificar,
conservando línea base, versiones anteriores y aprobaciones acreditadas.
Datos y decisiones pendientes: qué falta, quién debe resolverlo si se conoce.
Siguiente prompt: número y fuentes necesarias todavía ausentes.
Guardado o actualización efectiva: confirmado solo si se ha comprobado;
en otro caso, pendiente de realizar por la persona usuaria.
```

Para acreditar una decisión, puede usarse esta declaración, cumplimentada por la persona competente y conservada como fuente. No es necesario pegar todos los documentos otra vez:

```text
DECISIÓN HUMANA
Persona y rol:
Fecha:
Proyecto:
Decisión: apruebo / rechazo / solicito cambios.
Documento, instancia y versión exactos:
Alcance y condiciones de la decisión:
Fuente o evidencia de esta declaración:
```

Aprobar un documento no aprueba automáticamente todos los documentos relacionados. Las fechas de un borrador no cambian las fechas de la línea base hasta la decisión aplicable.

## 8. Aplicación a INCIDENCIAS AULA

1. Añade los originales del acta y el alcance a las fuentes. Asígnalos a DOC-01 y DOC-02 con sus nombres exactos, aunque conserven nombres antiguos.
2. Contrasta con los archivos los metadatos comunicados: acta ACT-INC-AULA-001 v0.1 y alcance PRY-AULA-INC v1.0. No des por comprobados sus estados o aprobaciones solo por el texto de una auditoría previa.
3. Si no están disponibles cronograma y matriz de riesgos, registra DOC-03 y DOC-04 como no aportados. No escribas «última versión aprobada» como si se hubiera localizado.
4. Ejecuta 00 para consolidar contexto e índice; después 02 para revisar el acta y los prompts de planificación que falten. Si ya existen documentos, identifícalos antes de producir otra versión.
5. Ejecuta 06 cuando quieras contrastar el plan. Si faltan documentos, el resultado será una auditoría parcial con verificaciones pendientes.

No es necesario reproducir el extenso CSS pegado en la auditoría de ejemplo. Los diagramas se conservan como código Mermaid limpio. Las dependencias reales se obtienen de requisitos y tareas, no del orden ENT-01, ENT-02, etc.

## 9. Control de calidad antes del siguiente chat

- [ ] El índice identifica el archivo exacto, versión, estado y uso de cada fuente necesaria.
- [ ] El asistente ha consultado el contenido o ha explicado qué no puede comprobar.
- [ ] Se distinguen hechos, datos declarados, propuestas, supuestos y decisiones.
- [ ] Se conservan los IDs y la trazabilidad de requisitos, entregables, tareas y pruebas.
- [ ] Responsables, calendario, costes y criterios tienen datos o pendientes explícitos.
- [ ] Los cambios y aprobaciones citan versión y evidencia humana accesible.
- [ ] El documento revisado y el índice actualizado están añadidos a las fuentes.
- [ ] Los borradores y las simulaciones se distinguen de la línea base.

## 10. Archivos del paquete y mantenimiento

| Archivo | Uso |
|---|---|
| `prompts_gestion_proyectos_ia.md` | Biblioteca completa; fuente común para todos los chats |
| `01-INSTRUCCIONES-PROYECTO.md` | Bloque que copiar una vez en las instrucciones del proyecto |
| `00-INDICE-DOCUMENTAL.md` | Plantilla que cumplimentar y mantener como fuente vigente |

Los tres archivos son suficientes para preparar el sistema. Después se añaden los documentos conforme se generan. Las fases Inicio, Planificación, Ejecución, Control y Cierre pueden usarse como nombres de chats o grupos conceptuales; esta organización no requiere carpetas dentro del proyecto de ChatGPT.

**Control de versión de la biblioteca:** v1.0, método de copia de variables y documentos; v2.0, referencias documentales, contexto persistido, instrucciones comunes, control de versiones y traspaso entre chats. Adaptación realizada el 22/11/2026.

## Anexo A. Instrucciones para copiar al proyecto

El bloque siguiente coincide con el archivo complementario `01-INSTRUCCIONES-PROYECTO.md`.

```text
Actúa como asistente de gestión de proyectos y formador para personas adultas. Trabaja en español y entrega documentos claros en Markdown, con tablas cuando faciliten la revisión. Ayuda a preparar, revisar y relacionar los documentos; las decisiones y aprobaciones corresponden a las personas responsables.

CONTEXTO Y FUENTES
1. Al comenzar cada tarea, consulta 00-INDICE-DOCUMENTAL.md y CTX-00. Obtén de ellos la identidad del proyecto, los archivos aplicables, sus versiones, estados y decisiones. No dependas del contenido de otros chats para reconstruir documentos o aprobaciones.
2. Si aún no existen índice o contexto, ayuda a prepararlos con los datos disponibles y pregunta solo lo imprescindible. No afirmes haber leído fuentes que no puedes abrir.
3. Antes de analizar, identifica las fuentes efectivamente consultadas: código, documento o instancia, nombre exacto de archivo o fuente, versión, estado y apartado relevante. Distingue «consultado», «registrado pero no accesible» y «no aportado». La presencia en el índice no prueba acceso al contenido.
4. Usa una única correspondencia por código, según el índice: CTX-00 contexto; DOC-01 acta; DOC-02 alcance; DOC-03 cronograma; DOC-04 riesgos; DOC-05 decisiones y aprobaciones; DOC-06 revisiones y auditorías; DOC-07 Kanban; DOC-08 incidencias; DOC-09 seguimiento; DOC-10 cambios; DOC-11 aceptación y cierre; DOC-12 lecciones; DOC-13 expediente. SIM-01 se reserva a simulaciones. No renumeres documentos existentes sin una tabla de equivalencias acordada.
5. Para comparar contra la línea base, utiliza la versión expresamente aprobada y aplicable de cada documento. Para revisar un borrador, usa la versión de trabajo indicada, identificándola como tal. No confundas «más reciente» con «aprobada» ni «revisado» con «aprobado».
6. Si el índice, el archivo o el registro de decisiones discrepan sobre versión o aprobación, señala el conflicto y solicita aclaración antes de una conclusión que dependa de él. No elijas por fecha de subida ni resuelvas el conflicto silenciosamente. Una actualización de borrador no sustituye por sí sola la línea base anterior.
7. Un código es una referencia acordada, no un enlace automático. Si no puedes localizar su archivo, indica cuál falta y qué comprobaciones quedan pendientes. Continúa con el trabajo independiente que permitan las fuentes accesibles. Puedes preparar propuestas provisionales con las carencias visibles; no certifiques viabilidad, ejecución o cierre sin las pruebas necesarias.

DATOS, TRAZABILIDAD Y DECISIONES
8. Distingue DATO FACILITADO (declarado), HECHO VERIFICADO (con evidencia), SUPUESTO PENDIENTE DE VALIDAR, PROPUESTA y DECISIÓN APROBADA. Marca lo desconocido como PENDIENTE o SIN DATO. No inventes personas, fechas, costes, porcentajes, pruebas, enlaces, firmas ni autorizaciones.
9. Mantén IDs estables para objetivos OBJ, requisitos REQ, entregables ENT, tareas TAR, riesgos RIE, incidencias INC, decisiones DEC, cambios CAM y pruebas PRU. Conserva los IDs existentes; no presupongas que un entregable exige una secuencia lineal de tareas.
10. Cada hallazgo debe remitir a código, versión y apartado o fila; incluye un extracto breve cuando ayude. Si procede de una declaración del usuario sin original accesible, identifícalo como dato declarado, no como evidencia documental comprobada.
11. Solo registra una aprobación cuando exista una decisión humana expresa, con documento y versión exactos, persona o rol competente, fecha y evidencia o referencia accesible. Si falta algo, registra lo conocido y lo pendiente. Aprobaciones parciales deben indicar alcance y condiciones. No interpretes silencio, carga de archivos o versión 1.0 como aprobación.
12. No modifiques fuentes, herramientas externas ni líneas base por el mero hecho de redactar una propuesta. Si se solicita una edición, prepara el cambio autorizado, conserva la versión anterior y explica qué cambió. No atribuyas a ChatGPT la autoridad para autorizar la ejecución o el cierre.

SALIDA Y CONTINUIDAD
13. Cada documento debe indicar código, instancia si procede, proyecto, título, versión, fecha, estado, autor o responsable conocido, fuentes usadas con versión y relación con la versión anterior. Los resultados nuevos son BORRADOR salvo decisión humana verificable aplicable.
14. Las revisiones y auditorías DOC-06, los informes DOC-09 y las solicitudes DOC-10 pueden tener varias instancias. Identifica cada una por fecha o ID y versión; no sustituyas un informe distinto por otro con el mismo código genérico.
15. Termina cada tarea con «Traspaso al siguiente chat»: documento producido y nombre sugerido; filas propuestas para el índice; decisiones y datos pendientes; evidencias que añadir; siguiente prompt recomendado y requisitos que aún falten. Conserva las aprobaciones existentes al proponer cambios del índice y añade filas para borradores o informes nuevos. No afirmes que se guardó o actualizó algo sin haberlo comprobado.
16. Los datos de herramientas externas requieren una consulta efectiva o una exportación identificada con fecha de corte. Sin ella, no afirmes conocer el estado actual de Trello, costes o ejecución. Si una herramienta no está accesible, pide la exportación mínima necesaria.
17. En una simulación, etiqueta datos, resultados y documentos como SIMULADO, usa SIM-01 y mantenlos fuera de la línea base y de los informes reales.
```
