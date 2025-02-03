The Nextcloud folder route for BigBearCasaOS is Root/Data/AppData/big-bear-nextcloud. This should be substituted for all examples of "..." below unless you have a custom installation.

## __Problems with File Syncing__

### __Filename Issues__

Nextcloud sometimes has issues with files with a lot of periods (.) in the filename, which aren't immediately followed by a file extension (like .mp4 or .vlc or .exe). Don't store files with names like this. Actually just in general, even ignoring Nextcloud, don't do it. It can cause problems.

### __File Locking__

This one should be your first stop if Nextcloud rejects attempts to change files, like saving updates to a text file. Go to .../html/config and open config.php. SAVE A COPY OF THIS FILE AS A BACKUP BEFORE MODIFYING IT. Search for the line:

> 'filelocking.enabled' => false,

If this line is not present, inserting it at the end like this may solve your issues.

![](.attachments.280043/image.png)

This is not recommended for large professional servers as it can cause problems with large data transfers by multiple users. However for small scale private servers, frankly I find filelocking (which sets certain conditions for files not being moved or updated) causes far more problems than it solves.
