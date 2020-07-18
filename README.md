# findDeletedReferencedPhotos

Find photos from your Photos Library when their referenced files are missing or deleted.

This script scans the albums you enter and finds any photos whose referenced files are missing. They are added to a new album in Photos, so you can review and delete them from your Photos Library later if you like.

This is an AppleScript script, and it can run using Script Editor.

1. Create a new script in Script Editor,
2. Copy the content of `findDeletedPhotos.script` and paste it into Script Editor,
2. Edit the three variables at the top:
	* `listOfAlbumNamesToScan` – this must be a list of strings, and contain the names of the albums to scan. It will find all referenced photos whose files are missing.
	* `nameOfDeletedImageFilesAlbum` – the name of the album that will be created in Photos if there are any missing files in your albums.
	* `referencedFilesFolderName` – the folder where all your files are physically stored. This script will search if the files exist in this folder and its subfolders.
3. To run the script, click the `Run` button or press `Command` + `R`,
4. When the script finished, go to Photos and select the album named after `referencedFilesFolderName`. This album will contain all the photos whose files are missing. You can either delete them from your Photos library, or link them back to their original files if you still have them somewhere.

Tested using macOS 10.15.5 and Photos 5.0.
