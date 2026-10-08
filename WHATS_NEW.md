# What's new in LGA Media Tools

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
