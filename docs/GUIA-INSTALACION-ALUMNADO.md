# Guía para instalar y utilizar el sistema de proyectos en ChatGPT

**Destinatarios:** alumnado de formación informática. **Edición:** 1.0. **Fecha:** 23/11/2026.

Esta guía te permite preparar un proyecto propio de ChatGPT y utilizar los prompts del curso en chats separados. Al terminar tendrás el contexto, el índice y el expediente inicial configurados. Después generarás y revisarás los documentos de gestión, uno cada vez.

El ejemplo INCIDENCIAS AULA consiste en preparar un formulario y un registro para comunicar problemas de un aula informática. Sus datos de partida son ficticios. Tus documentos, decisiones y pruebas se producirán durante la práctica.

## 1 Qué significa instalar este sistema

La instalación consiste en crear un proyecto de ChatGPT, copiar unas instrucciones y añadir tres fuentes. No necesitas instalar software, usar Git, programar ni conectar aplicaciones. Para comenzar necesitas una cuenta de ChatGPT, navegador, acceso a los materiales y una carpeta local donde guardar tus versiones.

El repositorio conserva el material de inicio. El proyecto de ChatGPT contiene tu trabajo. Cada alumno crea su proyecto independiente; si empieza otro caso, repite la preparación con la plantilla vacía.

| Elemento | Qué contiene | Qué haces con él |
|---|---|---|
| Repositorio o ZIP | Guías, instrucciones, archivos iniciales y prompts | Consultarlo o descargarlo |
| Instrucciones del proyecto | Reglas comunes del asistente | Copiarlas en los ajustes |
| Fuentes del proyecto | Contexto, índice y documentos | Añadirlas y mantenerlas actualizadas |
| Chats del proyecto | Una tarea o prompt por conversación | Abrir uno nuevo para cada trabajo |

## 2 Cómo obtener tu copia

El docente puede facilitarte un ZIP o acceso al repositorio. En GitHub, si tienes acceso, puedes descargarlo con Code y Download ZIP. Extrae el ZIP antes de utilizar sus archivos; subir el ZIP entero a ChatGPT no equivale a instalar el sistema.

Si el repositorio está marcado como plantilla y tienes cuenta de GitHub, puedes usar Use this template y Create a new repository. Esa operación copia los archivos del repositorio a otro repositorio; todavía debes crear el proyecto de ChatGPT.

Compartir el proyecto de ChatGPT del docente permite trabajar en un espacio compartido. La ayuda oficial describe una copia de tus chats al salir de un proyecto compartido, pero no establece una copia completa garantizada de instrucciones, archivos y conversaciones ajenas. Por eso la instalación del curso se realiza desde el paquete descargable. Fuentes oficiales y fecha de consulta al final de esta guía.

## 3 Elige el modo de trabajo

Para la primera práctica utiliza el modo compacto. El modo estándar es una alternativa si prefieres documentos separados y tu cuenta admite suficientes fuentes.

| Modo | Fuentes iniciales | Documentos posteriores |
|---|---|---|
| Compacto recomendado | Índice, contexto y expediente | Secciones dentro del expediente |
| Estándar | Índice y contexto | Un archivo por documento |

En el modo compacto, DOC-01 sigue siendo el acta aunque esté dentro de una sección de 99-EXPEDIENTE.md. Cada documento mantiene su versión y estado. El expediente común solo es el contenedor.

Según la ayuda consultada el 23/11/2026, el plan Gratis admite hasta cinco archivos por proyecto y un máximo de tres cargas diarias, sujeto a ajustes. Go y Plus admiten hasta 25 archivos y otros planes hasta 40. El modo compacto empieza con tres archivos, pero las actualizaciones pueden consumir cuota: no garantiza ejecutar toda la secuencia con nuevas cargas en el mismo día. Sigue el aviso de tu cuenta y acuerda el ritmo con el docente.

## 4 Prepara los materiales iniciales

Para trabajar con el ejemplo descarga descargas/kit-ejemplo-compacto.zip. Al extraerlo encontrarás INSTRUCCIONES-PARA-PEGAR.md y una carpeta fuentes con tres archivos.

| Archivo de fuentes | Función |
|---|---|
| 00-INDICE-DOCUMENTAL.md | Localiza documentos, versiones y pendientes |
| CTX-00-contexto.md | Describe el problema, recursos y objetivos iniciales |
| 99-EXPEDIENTE.md | Recibe los documentos generados en sus secciones |

Guarda una copia del kit intacta y otra carpeta para tu trabajo. Ejemplo de nombre local: INCIDENCIAS-AULA-Ana. Las carpetas locales sirven para organizar tus archivos; no se crean automáticamente como carpetas dentro de ChatGPT.

No subas la guía, todos los prompts, ambas variantes de instrucciones ni los dos casos de inicio. Elige un caso y un modo. Los prompts se copian desde el repositorio cuando los necesitas.

## 5 Crea tu proyecto de ChatGPT

1. Entra en tu cuenta y selecciona Nuevo proyecto.
2. Escribe un nombre reconocible, por ejemplo INCIDENCIAS AULA Ana.
3. Si aparece la elección de memoria, puedes utilizar memoria exclusiva del proyecto para mantener el contexto de este caso. El método se apoya en fuentes identificadas, no en recuerdos de otros chats.
4. Abre el proyecto recién creado y comprueba que cualquier chat nuevo se abre dentro de él.

Los nombres de los controles pueden variar según la cuenta o la interfaz. Si trabajas en un espacio de una organización, también se aplican sus ajustes. El sistema no requiere compartir tu proyecto con otros alumnos.

## 6 Copia las instrucciones y añade las fuentes

Abre INSTRUCCIONES-PARA-PEGAR.md del kit, o sistema/INSTRUCCIONES-COMPACTO.md del repositorio. Copia únicamente el contenido del bloque de texto, sin las líneas de tres comillas invertidas.

Abre el menú del proyecto y entra en Ajustes del proyecto. Pega el bloque en Instrucciones y guarda. Adjuntar el archivo de instrucciones como fuente no sustituye este paso.

Después añade como fuentes los tres archivos de la carpeta fuentes. Comprueba sus nombres en la lista del proyecto. CTX-00 contiene el caso ficticio y el expediente solo contiene secciones iniciales sin resultados ni aprobaciones.

Antes de ejecutar el primer prompt puedes enviar este mensaje de comprobación en el chat de preparación:

```text
Comprueba si puedes consultar 00-INDICE-DOCUMENTAL.md,
CTX-00-contexto.md y 99-EXPEDIENTE.md.
Indica el nombre del proyecto, el modo de trabajo y si existe
algún documento aprobado. Si no puedes leer una fuente, dilo.
No generes todavía el acta.
```

La respuesta debe identificar INCIDENCIAS AULA, modo compacto y ausencia de aprobaciones acreditadas. No basta con que repita los nombres que has escrito: debe describir datos del contexto y reconocer las secciones sin generar del expediente.

## 7 Ejecuta el primer prompt

1. Abre un chat nuevo dentro del proyecto y llámalo 00 Contexto.
2. Abre prompts/00-configurar-contexto.md en el repositorio o en el kit.
3. Copia el bloque completo de texto y pégalo en el chat.
4. Responde a las preguntas imprescindibles con tus datos de la actividad. Si no conoces algo, escribe PENDIENTE.
5. Revisa CTX-00, el índice y el registro inicial de decisiones que proponga.

Si el asistente propone nombres diferentes, conserva las ubicaciones de trabajo del kit o registra el cambio exacto en el índice. No mantengas dos contextos distintos como vigentes.

Decide con el docente el calendario real, la dedicación disponible y quién revisará la actividad. Las tres sesiones de dos horas son una propuesta inicial del caso, no un plazo verificado ni una obligación de tu curso.

## 8 Guarda y actualiza antes de cambiar de chat

Revisa el documento antes de guardarlo. Corrige datos, conserva las decisiones existentes y comprueba que no se haya omitido contenido al reconstruir el expediente. En modo compacto solicita el expediente completo actualizado y el índice completo; una tabla de cambios por sí sola no actualiza las fuentes.

Guarda los archivos revisados en tu carpeta de trabajo. Usa un editor de texto con codificación UTF-8; en Windows comprueba que el nombre no termine en .md.txt. Conserva el nombre de trabajo y guarda el histórico en otra carpeta con la versión o fecha.

Para actualizar una fuente, conserva primero una copia local anterior. Si la interfaz permite reemplazarla, comprueba que la versión nueva esté disponible. Si no, retira de las fuentes del proyecto la copia antigua y añade la revisada. No elimines el único original ni dejes dos versiones contradictorias como vigentes. Volver a subir un archivo con igual nombre puede crear un duplicado y consumir cuota de carga.

También puedes guardar una respuesta mediante Añadir a las fuentes del proyecto cuando esté disponible. Registra su título exacto y actualiza la ubicación en el índice si sustituye un archivo; evita dos fuentes vigentes con contenido distinto. Esta alternativa también está sujeta a los límites aplicables. Para empezar, los archivos completos facilitan conservar tus versiones.

Si hay una aprobación docente, conserva la declaración humana en DOC-05 con documento y versión, persona o rol, fecha y condiciones. Una revisión de ChatGPT no sustituye esa decisión. Aprobar el acta tampoco aprueba automáticamente el alcance o el cronograma.

## 9 Continúa con un chat por tarea

Tras guardar los resultados del Prompt 00, abre otro chat dentro del mismo proyecto para el Prompt 01. Después repite el ciclo. No hace falta copiar el acta completa en cada chat: el prompt remite a sus fuentes.

| Orden inicial | Tarea | Resultado principal |
|---|---|---|
| 00 | Revisar contexto y registro | CTX-00 e índice |
| 01 | Preparar el acta | DOC-01 |
| 02 | Revisar el acta | DOC-06 instancia REV-INICIO |
| 03 | Definir alcance | DOC-02 |
| 04 | Preparar cronograma | DOC-03 |
| 05 a 07 | Riesgos, auditoría y Kanban | DOC-04, DOC-06 y DOC-07 |

Los prompts 08 a 11 se utilizan cuando hay incidencias, seguimiento o cambios y pueden repetirse. El 12 prepara aceptación y cierre; el 13 es una simulación opcional; el 14 recoge lecciones y el 15 prepara el expediente final.

Si falta una aprobación puedes seguir preparando borradores provisionales. No presentes un borrador como compromiso aprobado. Si falta una prueba, déjala pendiente; no pidas inventar resultados para completar el documento.

## 10 Crea otro proyecto desde la plantilla vacía

Descarga descargas/kit-plantilla-compacto.zip y conserva el ejemplo como referencia. Crea otro proyecto de ChatGPT, copia las instrucciones y añade las tres fuentes de la plantilla vacía.

Cumplimenta CTX-00-contexto.md con tu nueva idea: nombre, problema, destinatarios, objetivo, recursos, fechas conocidas, entregables y exclusiones. Deja lo desconocido como PENDIENTE. Ejecuta el Prompt 00 y continúa con el mismo ciclo.

No arrastres el acta, aprobaciones, tablero ni resultados de otro caso. Cada proyecto tiene decisiones y evidencias propias. Si trabajas en equipo, acordad una única versión de las fuentes y quién registra los cambios.

## 11 Cómo pasar al modo estándar

Crea una copia local de tus fuentes y conserva el historial. Sustituye en Ajustes del proyecto las instrucciones compactas por sistema/INSTRUCCIONES-ESTANDAR.md. Extrae del expediente los documentos que quieras mantener separados, con código, versión, estado y fuentes en su cabecera.

Actualiza el índice con los nombres exactos y añade esos archivos a las fuentes. Retira o identifica como histórico el contenedor anterior para que no compita con las versiones nuevas. Haz una comprobación de acceso antes del siguiente prompt. Si tu cuenta no tiene espacio suficiente, continúa en modo compacto o agrupa por fases; no es necesario cambiar para completar la primera práctica.

## 12 Problemas frecuentes y comprobación final

| Problema | Qué hacer |
|---|---|
| No encuentra DOC-01 | Revisar el índice y su sección del expediente; comprobar si ya se generó |
| Usa otra versión | Identificar la vigente, corregir el índice y retirar la fuente contradictoria |
| Solo entrega cambios parciales | Pedir expediente e índice completos y comparar con la copia anterior |
| Expediente demasiado largo | Dividir por fases, actualizar ubicaciones y comprobar límites antes de continuar |
| Aparece límite de carga | Seguir el aviso y conservar el trabajo local; no subir biblioteca o prompts extra |
| Afirma una aprobación inexistente | Corregir el estado y registrar solo decisiones humanas con versión y evidencia |

Al finalizar comprueba: proyecto propio, instrucciones en ajustes, tres fuentes accesibles, contexto correcto, índice coherente y primer resultado revisado y guardado. Para entregar la primera práctica conserva acta, revisión, alcance y cronograma con sus versiones y pendientes.

## Fuentes oficiales consultadas

Consulta realizada el 23/11/2026. Las funciones y límites dependen de la cuenta y pueden cambiar.

- Proyectos en ChatGPT, OpenAI: https://help.openai.com/en/articles/10169521-projects-in-chatgpt
- Carga de archivos y límites, OpenAI: https://help.openai.com/en/articles/8555545-uploading-files-and-audio-to-chatgpt
- Crear un repositorio desde una plantilla, GitHub: https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template
