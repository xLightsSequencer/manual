# Preferences

## Backup Tab

![](<../../../../.gitbook/assets/image (696).png>)

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

![](<../../../../.gitbook/assets/image (9).png>)

This defines the location where the backup folder(Backup on Save/Launch or F10) will be saved. If the 'Use Show Folder' Checkbox is selected (the default) the backup files will be saved in the current show folder. If this is unchecked and a folder path is specified all the backup files will be saved to that location. If this folder doesn't exist (move computers or remove a harddrive) the backup directory will default back to the show directory.

![](<../../../../.gitbook/assets/image (669).png>)

### Alternative Backup Directory

![](<../../../../.gitbook/assets/image (290).png>)

This is the location where the Alternative backups will be saved. This is manually triggered with F11 or the File Menu option. This Backup function is intended as a secondary backup location, like a external hardrive or NAS device. By default the location is not set and will prompt you if you attempt to do a Alternative Backup and no folder is set. To enable, set the desired folder or drive location.

## View Tab

![](<../../../../.gitbook/assets/image (637).png>)

### Tool Icon Size

This function enables you to change the size of the tool icons that are used to represent the effects on the effects ribbon.

Four options are available:

![](<../../../../.gitbook/assets/image (218) (1).png>)

#### OpenGL Version

![](<../../../../.gitbook/assets/image (253).png>)

The OpenGL setting is used to define what version of the OpenGL API is being used for certain components of xLight rendering of 2D and 3D graphics.

This option does not have to be used unless you see issues with the waveform or icons not being displayed or the sequencer is jerky. In which case, starting with 3.x and working downwards , select an option and restart xLights and check the results. Advise the xLights team, as it could be that your video card drivers on your computer need updating.

#### OpenGL Render Order

In 3D mode, Model and Objects sometimes do not look correct in the house preview on all videocards. The Render Order 1-6 options use different render methods to generate the model layout. If you are having unwanted visual artifacts, try a different options and see if the models look better on your specific computer.

![](<../../../../.gitbook/assets/image (688).png>)

### Model Handle Size

This option will adjust the size of the model handles in the Layout Tab.

![](<../../../../.gitbook/assets/image (291).png>)

There are three sizes available:

![Normal](<../../../../.gitbook/assets/image (158) (1).png>)

![Large](<../../../../.gitbook/assets/image (40).png>)

![Extra Large](<../../../../.gitbook/assets/image (473) (1).png>)

### Effect Assist Window

![](<../../../../.gitbook/assets/image (645).png>)

"Always On" will display the window in all cases, "Always Off" won’t display the window and "Auto Toggle" will display the window if the effect supports it, else won't display the window if the effect does not have this capability. Click on an effect in the sequencer grid and expand the Effect Assist window. If "Always on" is selected and the effect is not supported by this window, then you will see a red X in the window.

![](https://lh3.googleusercontent.com/oJ1qR05VyFXZpxawaogvApOLAJwbaadAR0Yi\_yajBrGLb1cgce7-\_SPr6xSbM9BBSXHPJic3NKmq1vPjU0U8oBAc2K4AtP2qM4ffb0Xp9BzqvIzuk76XjMxYBhIjFzO5mDNtFy5d)

### Play Controls On Preview

This Options will display Play, Pause, Stop, Scrub Bar to the House Preview to allow control of the sequence playback. They will only appear if the house preview window is larger than 400 wide by 300 high.

![](<../../../../.gitbook/assets/image (286) (1).png>)

### Auto Show House Preview

Automatically Show the House Preview Window when the sequence is playing and hide the House Preview when the sequence is stopped.

## Effects Grid Tab

![](<../../../../.gitbook/assets/image (2).png>)

### Spacing

This function enables you to change the size (i.e. width of each band) of the sequencer grid.

Five options are available: Extra Small, Small, Medium, Large, Extra Large.

![](<../../../../.gitbook/assets/image (163) (1).png>)

![Grid Spacing Small ](<../../../../.gitbook/assets/image (788).png>)

![Grid Spacing Extra Large](<../../../../.gitbook/assets/image (620).png>)

### Icon Backgrounds

![](<../../../../.gitbook/assets/image (557).png>)

When an effect such as the Morph effect is placed between timing marks (as an example over several seconds long), a representation of the color changes over time for that effect.

If unchecked, then the effect on the sequencer grid will only show the generic effect icon and not the colors. Not all effects have this difference.

![Grid Icon Backgrounds On](<../../../../.gitbook/assets/image (41) (2).png>)

![Grid Icon Backgrounds Off](<../../../../.gitbook/assets/image (94).png>)

### Node Values

![](<../../../../.gitbook/assets/image (571).png>)

This function provides the ability to turn off the effect displaying colors at the node level.

Turning it off improves rendering performance and is recommended where effects are only being dropped at the model level. The value can be turned back on as required.

![Grid Node Values On](<../../../../.gitbook/assets/image (380).png>)

![Grid Node Values Off](<../../../../.gitbook/assets/image (268).png>)

### Snap to Timing Marks

![](<../../../../.gitbook/assets/image (125).png>)

If checked, When moving or resizing an effect this will snap the effect beginning and/or endpoint to the closest timing make if you drag it close enough (approx 10 pixels on your monitor).

### Double Click Mode

![](<../../../../.gitbook/assets/image (16).png>)

When "Play Timing" is selected, if you Double Click a timing mark, xLights will play the sequence for that timing mark interval. If "Edit Text" is selected, the Edit Label Dialog will appear. This Dialog allows you to input lyrics for singing faces or states for the state effect. The opposite option's functionality will works if you hold down shirt key then double click.

![Edit Label Dialog](<../../../../.gitbook/assets/image (266).png>)

### Small Waveform

![](<../../../../.gitbook/assets/image (653).png>)

When Enabled, the audio waveform will appear smaller on the screen. This is designed for screens with lower resolutions.

![Small Waveform](<../../../../.gitbook/assets/image (11) (2).png>)

![Normal Waveform](<../../../../.gitbook/assets/image (117).png>)

### Display Transition Marks

![](<../../../../.gitbook/assets/image (603).png>)

If checked, color bars are display to represent transitions, like fade in or fade out.

![](<../../../../.gitbook/assets/image (276) (1).png>)

## Sequence Tab

![](<../../../../.gitbook/assets/image (441).png>)

### Render On Save

The default setting is to render all the effects of all the models and groups when saving the XML. If this setting is unchecked (i.e. to turn off), then it will only save the sequence XML file when you click Save/Save As, resulting in a very fast save operation. If unchecked, then Render All must be used to populate the render buffer. You must Render All and then File Save to create a up to date FSEQ file.

### Model Blend Default Off

When checked, the Model Blending option in the sequence settings dialog will be disables by default when creating a new sequence.

### Render Cache

![](<../../../../.gitbook/assets/image (126).png>)

Render Cache allows xLights to render an effect or group of effects once and then save the individual frames in memory (and on disk) so it doesn't need to render the frames again. This can speed up render times, as xLights does not need to re-render unchanged effects.

### Render Cache Directory

This defines where the render cache files are saved on disk. If "Use Show Folder" is 'checked' xLights will use the current show folder. If 'unchecked' and a folder path is specified all the Render Cache data will be saved to that location. If this folder doesn't exist (move computers or remove a harddrive) the Render Cache directory will default back to the show directory.

![](<../../../../.gitbook/assets/image (294).png>)

{% hint style="info" %}
There is a purge render cache option under Tools->Purge Render Cache.
{% endhint %}

### Auto Save Interval

The Auto Save functionality creates a copy of your working sequence xml, in your show directory. By default, the open sequence will be saved every 3 minutes and will create or override a file ‘XXX.xbkp’ where ‘XXX’ is the name of your sequence. You can use this menu to change the timeframe this occurs at or to disable it. The ‘\*xml.xbkp’ files will also be included when you press F10 to back up your xml files from the show directory. It won’t be included if F11 is used to back files up to an alternate location.

![](<../../../../.gitbook/assets/image (66).png>)

![](https://lh3.googleusercontent.com/zuDkOJbt4\_ToDqX5VR0iU6Z7zbpFQRbdVJCbhyApI7tAle2Biufsdxdz9Dd7Ncnm\_9Bhc0pbXmDe\_gR8cGKDKVifrBtVu3Y-2jq6IlfVcyfZXiDTb7X5mfo1ZpMiS462pw5ALk4p)

In order to recover your sequence file from an unexpected error or corruption to the point when the last autosave executed: e nsure that xlights is not active. Then rename your existing sequence file (’xxx.xml’) to another name and rename the ‘xxx.xbkp. file to ‘xxx.xml’. Restart xLights, open the sequence and Click on Render All.

### Media/Resource Directories

![](<../../../../.gitbook/assets/image (560).png>)

This defines where xLights will search for audio/picture/video files, This should only be set if  the audio/picture/video files are **not** stored in the current show folder or a sub-directory of the current show folder. On Mac OS, adding folders in this section will give xLights the correct permissions to search them.

### Save FSEQ On Save

This will save the current rendered data to the FSEQ file on save. If this setting is disabled, the user will have to preform a Render All after opening a sequence. It is recommended that thus setting always remain checked (enabled).

### FSEQ Version

![](<../../../../.gitbook/assets/image (83) (2).png>)

Version 1 is the "original" FSEQ file format. V1 files contain all the channel data and can be very large file. xLights, FPP, and most controllers support V1. Version 2 of the FSEQ file format added compression and "skips" off channels to reduce file sizes. FPP 2.5 and lower do not support the V2 file format. ZSTD, ZLIB, Uncompressed are additional options to select which compression format to use. ZSTD is the default and is the preferred setting. These options can be changed in xLights to generate FSEQ files in the different file format for devices that require them. xLights 2019.64 and FPP 2.6+ support all the available file formats.

### FSEQ Directory

![](<../../../../.gitbook/assets/image (705).png>)

This defines where xLights will save FSEQ files. The FSEQ files are the raw sequence data for each sequence. If "Use Show Folder" is 'checked' xLights will use the current show folder. If 'unchecked' xLights will use the set folder path. If this folder doesn't exist (move computers or remove a harddrive) the FSEQ directory will default back to the show directory.

## Output Tab

![](<../../../../.gitbook/assets/image (111) (1).png>)

### Use Frame Sync

To use ArtNET or E1.31 frame synchronization then you need to enable it using this option. When enabled xLights will emit at the end of the frame a sync packet which supported controllers will use to trigger light output. This can make your show look a lot sharper but very few controllers support these packets.

For ArtNET you just need to select this option.

For E1.31 you also need to set a universe number on the controller tab … this universe number needs to be a universe you are not otherwise using.

![](<../../../../.gitbook/assets/image (312).png>)

### Force Local IP

By default xLights automatically selects which network interface to send out network data on and sometimes it selects the wrong one. To force xLights to send to a particular adapter select this option and select the IP Address of the adapter you want to use. Select the top blank line to disable forced IP mode and return to the default option of auto.

![](<../../../../.gitbook/assets/image (2) (1).png>)

### Duplicate Frames To Suppress

![](<../../../../.gitbook/assets/image (685).png>)

This selection allows xLights to "skip" frames that contain the same data as the previous frame. This can help with lagging, as it will reduce network traffic. xSchedule will also use this setting when outputting data.

### xFade/xSchedule

![](<../../../../.gitbook/assets/image (381).png>)

When using the Jukebox Panel with xFade or xSchedule, this determines which instance of xLight to select the effect from.

## Random Effects Tab

The Random Effects tab allows the user to set which effects are used by the Generate Random Effects Right click menu option in the sequencer.

![](<../../../../.gitbook/assets/image (151) (1).png>)

![](<../../../../.gitbook/assets/image (204).png>)

## Colors Tab

The Color Tab allows the user to change the colors options of xLights.

{% content-ref url="color-manager.md" %}
[color-manager.md](color-manager.md)
{% endcontent-ref %}

![](<../../../../.gitbook/assets/image (138).png>)

## Other Tab

![](<../../../../.gitbook/assets/image (621).png>)

### eMail Address

This settings allows the user to provide a contact email for when xLights submits a crash report. This is completely optional.

### Hardware Video Decoder

This setting allows xLights to use the computer's GPU to render video files. If you are having issues with video files's not displaying, it is recommended to disable this setting.

### Exclude Presets From Packaged Sequences

If selected, when a sequence is packaged with the Package Sequence option, all effects presets are stripped from the xlights\_rgbeffects.xml file.

### Exclude Audio From Packaged Sequences

If selected, when a sequence is packaged the audio file is skipped as it is generally not legal to share audio files with other people. When the recipient opens the sequence they will need to point to where the audio file is on their computer.

{% hint style="warning" %}
If excluding the audio from a packaged sequence, it is necessary to provide the source of the audio file to those the package sequence is being sent to. This is best done by filling on the metadata on the sequence settings for the song, artist, album, and music URL (link for download).
{% endhint %}

### Link Save

This option will cause xLights to save both the Controller Settings and Layout Settings when either save button is clicked.

### Link Controller Upload

When Uploading Controller Inputs and Outputs, this will cause xLights to do both upload actions when Upload Output is clicked.

![](<../../../../.gitbook/assets/image (331).png>)

### Prompt issues during batch render

If enabled this will prompt the user of error during batch render. These errors could be related to missing models and missing effect files. If disables these errors will be ignored and render will be skipped for the models involved.
