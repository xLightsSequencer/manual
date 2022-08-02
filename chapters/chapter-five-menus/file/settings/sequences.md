# Sequences

## Sequences

![](<../../../../.gitbook/assets/image (6).png>)

### Render On Save

The default setting is to render all the effects of all the models and groups when saving the XML. If this setting is unchecked (i.e. to turn off), then it will only save the sequence XML file when you click Save/Save As, resulting in a very fast save operation. If unchecked, then Render All must be used to populate the render buffer. You must Render All and then File Save to create a up to date FSEQ file.

### Low Definition Render

When Enabled model like matrixes and trees can be set to render at a smaller resolution to help lower render times during sequencing.

### Default Model Blending for New Sequences

When enabled, the Model Blending option in the sequence settings dialog will be enabled when creating a new sequence.

### Default View For New Sequences

![](<../../../../.gitbook/assets/image (36).png>)

Select a View to default as the Master View when creating a new sequence.

### Render Cache

![](<../../../../.gitbook/assets/image (126) (1).png>)

Render Cache allows xLights to render an effect or group of effects once and then save the individual frames in memory (and on disk) so it doesn't need to render the frames again. This can speed up render times, as xLights does not need to re-render unchanged effects.

### Render Cache Directory

This defines where the render cache files are saved on disk. If "Use Show Folder" is 'checked' xLights will use the current show folder. If 'unchecked' and a folder path is specified all the Render Cache data will be saved to that location. If this folder doesn't exist (move computers or remove a harddrive) the Render Cache directory will default back to the show directory.

![](<../../../../.gitbook/assets/image (827).png>)

{% hint style="info" %}
There is a purge render cache option under Tools->Purge Render Cache.
{% endhint %}

### Auto Save Interval

The Auto Save functionality creates a copy of your working sequence xml, in your show directory. By default, the open sequence will be saved every 3 minutes and will create or override a file ‘XXX.xbkp’ where ‘XXX’ is the name of your sequence. You can use this menu to change the timeframe this occurs at or to disable it. The ‘\*xml.xbkp’ files will also be included when you press F10 to back up your xml files from the show directory. It won’t be included if F11 is used to back files up to an alternate location.

![](<../../../../.gitbook/assets/image (66) (1).png>)

![](https://lh3.googleusercontent.com/zuDkOJbt4\_ToDqX5VR0iU6Z7zbpFQRbdVJCbhyApI7tAle2Biufsdxdz9Dd7Ncnm\_9Bhc0pbXmDe\_gR8cGKDKVifrBtVu3Y-2jq6IlfVcyfZXiDTb7X5mfo1ZpMiS462pw5ALk4p)

In order to recover your sequence file from an unexpected error or corruption to the point when the last autosave executed: e nsure that xlights is not active. Then rename your existing sequence file (’xxx.xml’) to another name and rename the ‘xxx.xbkp. file to ‘xxx.xml’. Restart xLights, open the sequence and Click on Render All.

### Media/Resource Directories

![](<../../../../.gitbook/assets/image (75).png>)

This defines where xLights will search for audio/picture/video files, This should only be set if  the audio/picture/video files are **not** stored in the current show folder or a sub-directory of the current show folder. On Mac OS, adding folders in this section will give xLights the correct permissions to search them.

### Save FSEQ On Save

This will save the current rendered data to the FSEQ file on save. If this setting is disabled, the user will have to preform a Render All after opening a sequence. It is recommended that thus setting always remain checked (enabled).

### FSEQ Version

![](<../../../../.gitbook/assets/image (83) (2).png>)

Version 1 is the "original" FSEQ file format. V1 files contain all the channel data and can be very large file. xLights, FPP, and most controllers support V1. Version 2 of the FSEQ file format added compression and "skips" off channels to reduce file sizes. FPP 2.5 and lower do not support the V2 file format. ZSTD, ZLIB, Uncompressed are additional options to select which compression format to use. ZSTD is the default and is the preferred setting. These options can be changed in xLights to generate FSEQ files in the different file format for devices that require them. xLights 2019.64 and FPP 2.6+ support all the available file formats.

### FSEQ Directory

![](<../../../../.gitbook/assets/image (43).png>)

This defines where xLights will save FSEQ files. The FSEQ files are the raw sequence data for each sequence. If "Use Show Folder" is 'checked' xLights will use the current show folder. If 'unchecked' xLights will use the set folder path. If this folder doesn't exist (move computers or remove a harddrive) the FSEQ directory will default back to the show directory.
