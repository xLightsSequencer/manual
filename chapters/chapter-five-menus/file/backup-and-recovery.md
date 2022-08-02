# Backup and Recovery

## Backup

Backing up your critical files and sequences should be done regularly – as good practice.

What should be backed up ? Anything you require to run your show, but in particular your XML sequences, your media files and your user specific xLights configuration files.

![](<../../../.gitbook/assets/image (798).png>)

The xLights configuration files are located in your show directory and are: xlights\_keybindings.xml, xlights\_networks.xml and xlights\_rgbeffects.xml

{% hint style="success" %}
By default xlights backs up the key files at the start of a session when xLights is launched.
{% endhint %}

The files are saved in a subfolder with a timestamp and ‘\_onstart’ suffix.

![](https://lh6.googleusercontent.com/P0tdvXNAx-bdxZzzvFKB80xmizSiXI73iORJA7wYiY88Tu3l2a\_9XW02lq5NUwoPQbZDFUPhViat47g6HzENaDEIAaIuOeQQ4uokDoWMNmgwoThcl2ZZE1x-mZq4RqUgKDv2VT5n)

It will also create a backup when the show directory is changed. If you have enabled Backup on Save, it will also take a snapshot after every Save operation.

{% hint style="success" %}
Pressing F10 anytime, anywhere will backup your XML files for you and store them in a new folder with the date/time embedded in the name the backup was created. You can press F10 as many times as you like and should do this at least once per sequencing session. Keep in mind that you must have saved at least once in order for an updated XML file to be protected.
{% endhint %}

Alternatively, from the File menu, select Backup.

You will be presented will a message indicating where a backup will be created. Click Yes to proceed.\
Every time this step is executed, a copy will be created of all the ‘\*xml’ files from your show directory into the Backup subdirectory of your show directory. A new subfolder is created each time a backup is executed.

{% hint style="info" %}
The F11 function does not do an auto (in memory) backup of the current sequence if you have one open. It will backup the open sequence XML contents from when it was last saved.
{% endhint %}

{% hint style="success" %}
It is a good practice to also separately backup any files that you may have used as inputs to your sequences such as LSP, LOR, Papagayo files that you imported, media files that may have amended with audacity, GIF or JPEGs etc. You may also wish to backup any FSEQ files, though this can be recreated by saving the sequence again.
{% endhint %}

Backing up the show directory (and media directory if it is different) to an alternate location is the simplest way to ensure that you have the files required.

![](https://lh5.googleusercontent.com/01Vxfgt8wGxpwf6MizV8wsICSfvfhPBLbW-nWXoMTcuOBp1WJxalmSdYwTyz4FcObgWDLHWpXgse3FNf4Wb7WZA4-KGMaESj6RvyjfHkGfcXaURmORxrJh9nrghd0KEROcZEwPoA)

## Recovery

To summarise the backup functionality:

* When xlIghts starts up - a folder timestamp\_OnStart is created and the XML and XBKP files in the show directory are backed up there.
* When F10 / F11  is pressed , a folder (timestamp) is created  in the show/alt location and the above files are backed up there (referred to as an on demand save).
* Every x (3,10,15,30) minutes , the current open XML file (i.e xxx.xml) is backed up (overwrite) to xxx.xbkp or \_\_.xbkp (for a new unnamed sequence) in the show directory. This will occur if there have been any changes since the last auto save or on demand (F10/F11) save.
* Every x minutes (same value as set above), the xlights\_rgbeffects.xml is backed up to xlights\_rgbeffects.xbkp in the show directory. This includes the layout as well.  This will occur if there have been any changes since the last auto save or on demand (F10/F11) save.

### Restore Backup

If you need to recover, File -> Restore Backup

![](<../../../.gitbook/assets/image (32).png>)



![](../../../.gitbook/assets/2022-08-02\_00h53\_10.png)

Select the backup folder from the left list and "check" which files to restore. The right list display basic data about the files found in the selected backup folder.

* **xlights\_networks.xml** file contains the controller tab data.
* **xlights\_rgbeffects.xml** file contains the layout, model, preview and preset data .
* **xlights\_keybindings.xml** files contains the keyboard shortcut settings.

The Sequence Tab can be used to backup sequence files.

![](<../../../.gitbook/assets/image (19).png>)

Click the "Restore Files" button to start the restore process.

![](<../../../.gitbook/assets/image (33).png>)



