# What's new in LGA Media Tools

## v1.001 (2026-11-02)

- **New:** El lápiz de la fila `----` del dropdown `Transcode Preset` abre una ventana con todos tus presets y qué hace cada uno, donde podés renombrarlos y cambiarles el orden.
- **New:** Si cerrás Media Tools con transcodes en curso, te pregunta si querés abortarlos; al confirmar, la app restaura los originales y borra la salida a medias antes de cerrarse.
- **New:** Transcode acepta clips Sony X-OCN de la VENICE (MXF) y los convierte a cualquier formato de salida.
- **Improved:** Cuando Transcode no puede arrancar su motor de conversión (por ejemplo, porque un antivirus o la seguridad de la empresa lo bloquea), la fila explica qué pasó y ya no quedan procesos colgados en segundo plano.
- **Improved:** Cuando un transcode falla porque el proceso se cortó, la fila muestra el motivo real en vez de "illegal value".
- **Improved:** Transcode de secuencias EXR a EXR (DWAA, ZIP y PIZ) va más rápido en la Mac, sobre todo en colas de varios jobs. (macOS only)
- **Improved:** Transcode a PNG, TIFF y DPX arranca más rápido en la Mac en colas de varios jobs. (macOS only)
- **Improved:** Exportar secuencias PNG en la Mac es varias veces mas rapido, con archivos del mismo tamano o mas chicos. (macOS only)
- **Improved:** Transcode de secuencias EXR a ProRes 422 va mucho más rápido en la Mac, sobre todo en colas de varios jobs. (macOS only)
- **Improved:** Transcode avisa cuando Delete Originals no puede borrar un original (por ejemplo, porque otro programa lo tiene abierto): la conversión queda hecha, el original sigue en la carpeta Originals y la fila lo marca con ⚠.
- **Improved:** Clicking the Original column header in Rename sorts by name with standalone folders on top and each sequence right below its folder; click again to reverse the order.
- **Fixed:** La cola de Transcode y el arranque de la app ya no se congelan cuando hay secuencias grandes, un disco externo desconectado o una carpeta de red caída.
- **Fixed:** La carpeta temporal por defecto que muestra Settings es la que de verdad usa el transcode. (macOS only)
- **Fixed:** Transcode a H.264 y H.265 con `Use GPU` ya funciona en la Mac con el encoder por hardware de Apple; si el hardware no acepta el tamaño del cuadro, convierte por CPU en vez de fallar. (macOS only)
- **Fixed:** Transcode ya convierte videos a DPX en la Mac: antes fallaba apenas arrancaba. (macOS only)
- **Fixed:** Transcode de EXR a EXR con conversión de color o cambio de tamaño ya funciona en la Mac: antes fallaba apenas arrancaba. (macOS only)
- **Fixed:** Transcode ya convierte videos a MP4 y MOV en la Mac: antes fallaban apenas arrancaban. (macOS only)
- **Fixed:** Cuando una conversión de video falla, Transcode Queue muestra el motivo en vez de decir que la abortaste.
- **Fixed:** Transcode en Same folder/Originals con Delete Originals ahora sí borra el video original al convertirlo a EXR o TIFF, en vez de dejarlo en la carpeta Originals. (Windows only)
- **Fixed:** Transcode en Same folder/Originals ya no borra el original que ya estaba en la carpeta Originals al volver a convertir un clip o una foto: el nuevo se guarda al lado como _2, _3...
- **Fixed:** Transcode ya no reemplaza un video o una carpeta de frames que ya existe en el destino: la conversión nueva sale con _2, _3..., y Transcode Queue muestra ese nombre.
- **Fixed:** Rename's Fix Files and Fix folder now show their progress right away, and the list stays where it was afterwards instead of jumping back to the top, so you can keep fixing the other mismatches below.

## v1.000

- **Improved:** Rename shows a yellow folder icon beside each folder name, making folders easy to distinguish from files and sequences.
- **Fixed:** The file lists in Rename, Transcode and Transcode Queue now show their scrollbar, and Transcode no longer shows a horizontal scrollbar when all columns fit.

## v0.630

- **New:** Rename lists the dropped folder and its subfolders, including empty folders, and lets you rename them; use Folders to toggle their selection.

## v0.629

- **Fixed:** Closing Media Tools now also stops its background transcode processes, which kept up to 2 GB of graphics card memory busy for 10 to 30 minutes after the app was closed. (Windows only)

## v0.627

- **Fixed:** Transcode no longer flashes a terminal window that stole the focus when a job started, which happened on the first transcode after installing. (Windows only)

## v0.625

- **Improved:** The installer is less than a third of the size (about 140 MB instead of 436 MB), so updates download faster, and Media Tools takes about 1.3 GB less disk space. (Windows only)

## v0.624

- **New:** Rename groups files by folder and numbering starts again in each folder (or continues, if you prefer), from the number you choose.
- **New:** Rename can order files by name, date taken or date modified, or by hand: drag rows or use Alt+Up/Down to set the numbering order.

## v0.623

- **Fixed:** Rename no longer hides files when a folder has two groups with the same name and different extensions, like an iPhone export with IMG_0737.JPEG and IMG_0737.MOV.

## v0.621

- **New:** Transcode now opens iPhone HEIC/HEIF photos and converts them to JPG with the new JPG photo output, keeping the date, camera, GPS location, color profile and orientation.

## v0.620

- **New:** Rename's Search & Replace understands wildcards: search `*` and replace with `name_###` to rename every checked file as name_001, name_002… in table order, or use `ref_*` to keep the original name with something added. The file extension is never touched, and you are warned before a counter would replace the frame numbers of an image sequence.
- **Improved:** Rename sorts files naturally (photo 2 before photo 10) and ignores the hidden `._` files that macOS leaves next to your media.
- **Fixed:** Renaming files whose new names were taken by other files in the same batch (for example swapping two names) no longer fails halfway.

## v0.613

- **New:** In Rename you can add more Search & Replace rows with the + button (up to 8) to rename everything in one go; presets are disabled while there are more than two rows.

## v0.612

- **Improved:** Media Tools now checks for updates every few hours while it stays open, not only at startup. Remind me later waits one day instead of a week, and closing the update window won't ask again until you restart the app.

## v0.611

- **New:** The Transcode Queue has a Skip Current button that stops the transcode in progress and moves on to the next one; if it doesn't respond, the button becomes Force Skip. Hover over a Skipped item to see why it stopped.
- **Fixed:** After aborting a ProRes transcode, the next one no longer fails right away as cancelled.

## v0.609

- **Improved:** Update now in the update window and OK in the What's new window are highlighted as the main action.

## v0.608

- **New:** The update window now shows what's new before you install, the app shows it once after an update you didn't see, and Help has a What's new link with the full history.
- **Improved:** In the update window, Update now moved to the right, after the other buttons.

## v0.601

- **Improved:** NTFX Pull now creates the comp folder in lowercase (comp), and reuses a Comp folder if the shot already has one.

## v0.591

- **Improved:** Uninstalling no longer leaves leftover files behind in the app folder. (Windows only)

## v0.583

- **Improved:** Settings > Transcode Temp Folder: the app now works in its own subfolder of the folder you choose, empties it of files older than 24 hours and leaves everything else in your folder alone, so keep nothing of yours inside it.

## v0.582

- **Improved:** Caches, logs, temporary transcode files and the downloaded update installer now live inside the app folder and clean themselves up, so uninstalling removes them too. (Windows only)
