# Backup

## Backup

![](<../../../../.gitbook/assets/image (257).png>)

### Backup On Save

With this setting activated, xLights will perform an backup (similar to a user pressing F10 to manually backup) each time the sequence is saved - when the user clicks on Save or Save As.

The existing files, including the saved sequence XSQ, will be backed up to the Backup folder in your show directory prior to the render executing and FSEQ file being created.

### Backup On Launch

With this setting activated, xLights will perform an backup (similar to a user pressing F10 to manually backup) each time xLights is launched. The existing files will be backed up to the Backup folder in your show directory, prior to the application launching and updating any xLights files when it is launched. The Backup sub directory created will have a suffix of ‘\_OnStart’ added to the folder name.

![](https://lh3.googleusercontent.com/Gj\_dlECG5u3kLvTUz4EFSCHZVEDsuFZbfalKz\_8PubdgJfGTp22pFAQDjMCQQSpQcgzTDcDgqPYiJggSLa7kEshIIKuCsR8FkEhGA7JIFkrlpczkm93YWUMqlJoVuOZhw3BqdIiA)

### Backup Subfolders

When selected, backups are made of all relevant files both in the show directory as well as any sub-directories (excluding the backup folder itself).

### Purge Backups Older Than

This drop-down sets how long xLights will keep backup. With "Never" selected xLights will not delete any backups. 365, 90, 31, and 7 days will delete backup folder older than the selected length. This helps to clear out older files and free up space.

![](<../../../../.gitbook/assets/image (681).png>)

### Backup Directory

![](<../../../../.gitbook/assets/image (60).png>)

This defines the location where the backup folder(Backup on Save/Launch or F10) will be saved. If the 'Use Show Folder' Checkbox is selected (the default) the backup files will be saved in the current show folder. If this is unchecked and a folder path is specified all the backup files will be saved to that location. If this folder doesn't exist (move computers or remove a harddrive) the backup directory will default back to the show directory.

![](<../../../../.gitbook/assets/image (270).png>)

### Alternative Backup Directory

![](<../../../../.gitbook/assets/image (219).png>)

This is the location where the Alternative backups will be saved. This is manually triggered with F11 or the File Menu option. This Backup function is intended as a secondary backup location, like a external hardrive or NAS device. By default the location is not set and will prompt you if you attempt to do a Alternative Backup and no folder is set. To enable, set the desired folder or drive location.

