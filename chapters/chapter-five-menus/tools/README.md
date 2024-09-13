# Tools

## Tools

![](../../../.gitbook/assets/2022-08-02\_01h48\_51.png)

### Test

The Test Dialog enables you to test anything from a single channel, all channels for a model or all channels by sending different test patterns to your physical lights.

![](../../../.gitbook/assets/base647b688d87c5c65c44.png)

{% content-ref url="test.md" %}
[test.md](test.md)
{% endcontent-ref %}

### Check Sequence

The Check Sequence option runs a series of verification routines against the currently loaded setup, layout and sequence. This process will generate a text file containing information on the controller outputs, channel mappings and model information as well as identify any potential issues which could cause problems within xLights. Selecting the option will open up a text file using the default text file editor on your computer.

![](<../../../.gitbook/assets/image (834).png>)

{% hint style="warning" %}
ERRORS in a check sequence file indicate there is something wrong with your setup, layout, or sequence and the show will not run correctly. Errors should be fixed before trying to run the sequence from your controllers.

WARNINGS are indications that something is not typical, but the show will still run. Verifying that the warnings are intended, or correcting their cause is recommended before running the sequence from your controllers.
{% endhint %}

### Cleanup File Locations

Cleanup File Locations will move all the files currently used by xLights (audio, videos, pictures, etc) into the Show directory. This is useful when backing up or packaging your sequence for sharing, so that all of the needed files and paths are retained.

![](<../../../.gitbook/assets/image (998).png>)

### Package Sequence

This option will take the currently open sequence and packages it up neatly into a zip file with all the images, audio and other files necessary to open and re-render this sequence on another computer. If you plan on sharing a sequence with another person then this is the best way to ensure you grab everything the recipient will need to open and use your sequence.

### Download Sequences/Lyrics

The Download Sequences/Lyrics Dialog provides a list of free sequences available on the Google Drive. You can select a Sequence to download and xLights will open the download link in your default web browser.

This Dialog also contains links to the Singing Faces Project Lyric tracks. You must be a member of the singing faces project to access these files.

![](<../../../.gitbook/assets/image (1030).png>)

### Batch Render

<figure><img src="../../../.gitbook/assets/image (1197).png" alt=""><figcaption></figcaption></figure>

Batch Render allows the user to re-render multiple sequence files. This is useful if a Layout change was made and all the FSEQ files need to be updated. The "Filter" drop-down allows the user to select which folders to search for the sequence XSQ/XML files in.

* Recursive Search - No Backups
  * Search the show folders and sub-folder **not** including backup folders.
* Recursive Search
  * Search the show folder and sub-folder **including** backups folders.
* Only Show Directory
  * Search Only the root show folder.

If "Recursive Search" or "Recursive Search - No Backups" is selected the "Folder" drop-down allows the user to select a sub-folder to limit the search too.

Place a check-mark next to the sequence XSQ/XML file name you plan to batch render. There is a right click menu to Select All or Select None.

![](<../../../.gitbook/assets/image (982).png>)

Click OK to render all the Sequence XML file.

{% hint style="warning" %}
If a Error is found during batch rendering, xLights will display a popup and will stop rendering. Monitor batch rendering to verify all the FSEQ files are created correctly.
{% endhint %}

### FPP Connect

![](<../../../.gitbook/assets/image (653).png>)

FPP Connect is used to upload to a Falcon Pi Player that is playing the role as a show player the channel and model configurations and one or more sequences (including associated audio).

{% content-ref url="fpp-connect.md" %}
[fpp-connect.md](fpp-connect.md)
{% endcontent-ref %}

### Bulk Controller Upload

Bulk Controller Upload allows the user to upload the E1.31 Universe Inputs, and Controller String port Settings. Check the controllers you would like to upload and click upload.

![](<../../../.gitbook/assets/image (665).png>)

Right Click to enable options to Select Controllers based on Active, Auto Config or FPP Proxy

<figure><img src="../../../.gitbook/assets/image (1198).png" alt=""><figcaption></figcaption></figure>

### HinksPix Export

HinksPix Export dialog is used to generate the required SD card files to use the HinksPix controllers in standalone mode. The selected sequences files will be generated for the selected controllers.

![](<../../../.gitbook/assets/image (331).png>)

### Run Scripts

This dialog allows the user to run Lua scripts to automate xLights functions.

![](<../../../.gitbook/assets/image (36).png>)

### Export Models

The Export Models functionality creates a Spreadsheet (.xlsx) file with the details of all your models. Click on the Export Models menu item. You will be prompted for a filename and location to create the file in. Specify the filename and click OK.

![](<../../../.gitbook/assets/image (745).png>)

The Spreadsheet file will be created with a row for each model defined listing all the key attributes. Additional sheets are added with group attributes and global Channel/pixel counts. Spreadsheet programs such as Microsoft Excel or [LibreOffice ](https://www.libreoffice.org/)are used to view the .xlsx files.

![](../../../.gitbook/assets/2022-08-02\_20h26\_52.png)

### Export Effects

The Export Effects functionality creates a CSV file with the details of all the effects in the open sequence. Click on the Export Effects menu item. You will be prompted for a filename and location to create the file in. Specify the filename and click OK.

A CSV file will be created with a row for each effect defined listing all the key attributes. In addition summary rows are created showing the number of times each sequence is used as well as the total duration of each effect.

![](<../../../.gitbook/assets/image (98).png>)

### Export Controller Connections

The Export Controller Connections option creates a Spreadsheet with all the controller to model wiring information. This is meant to be used as a prop "hookup" list.

![](<../../../.gitbook/assets/image (66).png>)

### View Log

The View Log option, enables a user to view the information / debug log that xLights maintains, if required to troubleshoot any problems and provide information when posting questions. Selecting the option will open up a text file using the default text file editor on your computer. Scroll to the bottom to view the latest messages that have been written to the log.

![](<../../../.gitbook/assets/image (387).png>)

![](../../../.gitbook/assets/2022-08-02\_20h28\_46.png)

### Package Log Files

The Package Log Files option, provides functionality to package the required xLights XML/XSQ and log files into a ZIP file which can then be provided for analysis. It is similar in content to the ZIP file created when a system crash occurs.

![](<../../../.gitbook/assets/image (741).png>)

From the Tools menu, with the sequence that needs to be investigated open, select the Package Log Files option. The required files will be zipped into a file ‘xLightsProblem.zip’ and you will be prompted to save it in the show directory.

You can change either the ZIP file name and/or the location before saving the file.

![](../../../.gitbook/assets/2022-08-02\_20h29\_42.png)

The zip file will contain the xLights network, rgbeffects, the sequence XSQ (if open is open) and a log file. The zip file can then be provided to the xLights team for analysis.

### Purge Download Cache

To speed up loading, xLights caches(saves) the download items(Vender Model List, Free Sequence List) for up to 5 days. Purge Download Cache deletes the cached files and forces xLights to downloaded the newest version. This is needed when there are updated to the files available for download, but xLights is not seeing the newest list.

### Purge Render Cache

The Render Cache is used to save rendered effects data to speed up render times. This option deletes the cache and forces xLights to re-render all the effects.

### Generate 2D Path

This 2D Path Generate Tool allows you to create X and Y value curve "paths" that can then be used by effects like the shape effect.

![](<../../../.gitbook/assets/image (593).png>)

Click and Drag the endpoint Dots, to move them. Double Click to add a new Line Segment. The Browse button allows the user to load a image to trace if needed. The slider will adjust the image brightness. Load will allow you to edit previously generated files. The Generate Button will save the path to two value curves files (X & Y Direction) to be loaded by an effect.

![ Value curve Files](<../../../.gitbook/assets/image (1100).png>)

### Generate Custom Model

The Generate Custom Model function enables you to generate an xLights custom model using a picture or video of the physical item. You should have defined your controller and need to know which channel the model will start on and how many channels.

![](<../../../.gitbook/assets/image (842).png>)

{% embed url="https://youtu.be/PrvqctYHC7I?si=-B5vEklLsqp1y6Av" %}

{% content-ref url="generate-custom-model.md" %}
[generate-custom-model.md](generate-custom-model.md)
{% endcontent-ref %}

### Remap Custom Models

This tool is used to take a model with valid/useful face definitions, state definitions and submodels and remap them onto a model with a reordered wiring layout. The two models must be identically dimensioned custom model with pixels in all the same positions.

![](<../../../.gitbook/assets/image (45).png>)

### Generate Lyrics From Data

The Generate Lyrics From Data allows xLights to generate Lyric Timing Tracks with Phonemes from channel data. This data can be a LOR LMS or LAS file, that has been imported as a data layer first. Select the start channel of the channel data and the offset for each mouth movement channel. xLights will then generate the Phonemes Track from this data.

![](<../../../.gitbook/assets/image (1060).png>)

{% embed url="https://www.youtube.com/watch?v=iYFGEfJiCB4" %}

### Convert

The Convert function is commonly used to convert a sequence file from one sequencer format to the format of another sequencer or to the format (.fseq) required to run via Falcon Player on a Raspberry Pi or BeagleBone Black controller.

![](<../../../.gitbook/assets/image (313).png>)

{% content-ref url="convert.md" %}
[convert.md](convert.md)
{% endcontent-ref %}

{% hint style="warning" %}
This is not to be used to convert files into an xLights sequence – use the Data Layer or Import, Import Effects options to achieve that.
{% endhint %}

### Prepare Audio

Prepare Audio allows xLights to load an audio "Cut List" file and edit an audio file to remove sections of a song or combine multiple songs. Reaper project files(.rpp) and xAudio Files (.xAudio) Files are supported.

### User Lyric Dictionary

![](<../../../.gitbook/assets/image (598).png>)

The User Lyric Dictionary Dialog allows the user to manually add word phonemes breakdowns to the user dictionary file in the current show folder. This list will be used in addition to the standard and extended library, to breakdown works when creating lyric tracks. Enter your new work into the first text box. The second text box will auto search the current word list and find similar words and display their phonemes. The second box supports multiple words separated by a space. Once you are happy with the phonemes breakdown you can add it to the library.

![](<../../../.gitbook/assets/image (635).png>)

### xSchedule

**Windows and Linux** - This menu option will launch the xLights scheduler/player xSchedule.

### &#x20;xCapture

**Windows and Linux** - This menu option will launch the xCapture E131 Recording Tool.

### &#x20;xScanner

**Windows and Linux** - This menu option will launch the xScanner, which can be used to discover controllers located on the network.

### 2nd xLights

**MacOS** - This menu option will launch the second instance of xLights that can be used for mapping sequences.
