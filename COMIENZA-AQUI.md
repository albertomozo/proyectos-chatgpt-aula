# Comienza aquí

**Objetivo:** tener tu proyecto de ChatGPT preparado para ejecutar el primer prompt. No necesitas instalar programas ni tener una cuenta de GitHub si el docente te facilita el ZIP.

1. Descarga y descomprime el [kit de ejemplo compacto](descargas/kit-ejemplo-compacto.zip). Mantén una copia intacta.
2. En ChatGPT crea un **proyecto nuevo** llamado `INCIDENCIAS AULA · tu nombre`.
3. Abre [las instrucciones compactas](sistema/INSTRUCCIONES-COMPACTO.md), copia solo el bloque y pégalo en **Ajustes del proyecto > Instrucciones**.
4. Añade como fuentes solo estos tres archivos de `fuentes/`: `00-INDICE-DOCUMENTAL.md`, `CTX-00-contexto.md` y `99-EXPEDIENTE.md`. No subas el ZIP ni todos los archivos del repositorio.
5. Abre un chat dentro de tu proyecto llamado `00 · Contexto`. Copia el bloque del [Prompt 00](prompts/00-configurar-contexto.md) y envíalo.
6. Revisa lo que propone. Guarda la versión completa revisada del contexto, índice y expediente que cambie. Actualiza las fuentes de tu proyecto; conserva el histórico en tu carpeta local.
7. Abre otro chat dentro del mismo proyecto, llamado `01 · Acta`. Copia el [Prompt 01](prompts/01-crear-acta.md).
8. Repite el ciclo: copiar prompt, revisar, guardar y actualizar fuentes, abrir siguiente chat.

**Compartir un proyecto no crea automáticamente una copia independiente para cada alumno.** La copia de este sistema se obtiene creando un proyecto propio con los mismos archivos e instrucciones. La copia de un repositorio de GitHub tampoco crea el proyecto de ChatGPT.

Si ChatGPT no encuentra DOC-01 en modo compacto, indícale que consulte la sección DOC-01 de `99-EXPEDIENTE.md`. Si aún dice «No generado», primero ejecuta el prompt que lo produce.

Para un proyecto diferente usa el [kit vacío compacto](descargas/kit-plantilla-compacto.zip), cumplimenta CTX-00 y crea otro proyecto nuevo. No reutilices documentos o aprobaciones del ejemplo como si fueran de tu nuevo caso.

[Guía paso a paso](docs/GUIA-INSTALACION-ALUMNADO.md) · [Lista de prompts](prompts/README.md) · [Guía docente](docs/GUIA-DOCENTE.md).
