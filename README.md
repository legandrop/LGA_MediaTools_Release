# LGA Media Tools — Releases

Este repositorio no tiene codigo: existe solo para publicar los artefactos de
**LGA Media Tools** y para que se puedan bajar sin credenciales.

El codigo vive en `legandrop/LGA_MediaTools_v2`, que es privado. Hasta que ese repo paso a
privado los releases se publicaban ahi mismo, y por eso dejaron de ser alcanzables: de ahi que
exista este.

## Descargas

Ir a **[Releases](../../releases/latest)** y bajar el instalador:

| Archivo | Para que sirve |
|---|---|
| `LGA_MediaTools_Setup_v<version>.exe` | Instalacion en Windows |

**Media Tools es solo Windows.** No hay build de macOS.

## Actualizaciones

El card de **LGA Updates** del tab Tools de PipeSync avisa cuando hay una version nueva. La
version que lee sale del manifiesto de `legandrop/LGA_Updates`, que se regenera solo cuando se
publica un release aca.

Para que PipeSync sepa que version esta instalada, Media Tools escribe su version al arrancar en
el registro compartido de LGA. Una instalacion que nunca se abrio figura como "instalada, falta
abrirla" y no como una version concreta.
