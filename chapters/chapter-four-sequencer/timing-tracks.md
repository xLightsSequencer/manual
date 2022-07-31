# Timing Tracks

## Timing Tracks

xLights can support multiple timing tracks on the sequencer, each with different frequencies of timing marks. By default, a timing track ‘New Timing’ is created for each sequence if you have not created one when creating a new sequence. Timing Tracks can be added via the File, Sequence Settings, Timing menu.

![](<../../.gitbook/assets/image (85).png>)

![](https://lh6.googleusercontent.com/c7Uqn9YaT6GdMJcEifMa67DI3OLSuI2BapJVAl8frx\_VBLZLjt-yafXWmv\_8hkQ\_qjiyiZuPqQ1DP4dgIFEV1akh\_HK2n6iP5jc0qatGLBUn5rEyg0cujBOWCi\_A2rUOxWaHmtMt)

Clicking on the down arrow will provide a drop down list of timing intervals to select from to create a timing track. Other than the first three, the remaining are from the VAMP plugins. If you have not installed the plugins then they will not appear in the list.

![](https://lh3.googleusercontent.com/Rpt6-NX4V1qZobg6X6dvCwK8GfWGfgEs2c9GihH9Z4gNvckhCMnruEmMKOdJdahF\_ncAQL95NVix5S7JIA8SU\_jvE34HC9iOdqRB\_StOESBuut1WuvMax\_VqKsyWs9l3E5d3PsO7)

You can also import a Timing track that has been created externally. Click on the Import button instead of the New button. A window Chose Timing files(s) window will open, enabling you to browse for and select the timing file to be imported. Navigate to the .txt file containing the timing track and click OK to import it. The new timing track can be a lyric track with phrases and words broke down into phenoms.

![](https://lh3.googleusercontent.com/12QtPYnhVDORqwqr\_-hFLwzabT2fs2axkkSSAH7O-oLAgxWzGG4LBiXtYQAYfU\_t4C\_By9q1BNhZI4tK6VWA1-Cu0-91CuvekVBgOerQx0fRqTNsB5bOG1S\_jKdp1buxPmIujTxb)

{% hint style="info" %}
If you are trying to import a LOR timing grid and it is not retrieved i.e. the window is empty, use any xml supported editor and check the LMS xml file for a section called \<timingGrids>. The section should contain a subsection called \<timingGrid> which must contain an attribute called "type=freeform".
{% endhint %}

When you create a timing track it gets added to all views that you have defined. Timing tracks are local to a sequence.

{% hint style="info" %}
The timing marks create a grid but once the effects are dropped they have no relation to the original timing marks that were used to drop them. You can switch to any other timing track and have a completely different grid.
{% endhint %}

If you have multiple timing tracks defined,

* Each timing track has a different color of timing marks.
* You can select the timing track radio button (to the left of the timing track name) to enable that track. You can also select more than one timing track to be displayed at the same time, however only one timing track will be active for effects to calculate the start and end position.
* You can rename a timing track , by right clicking on the timing track name and then providing a new name in the window that gets displayed.

![](https://lh3.googleusercontent.com/Lm0V6P5ht4qLyB3PiVSnkV69xQSZMIvD1bPUaLxDejAjl3cJYzEqFfFokk23F78jFJKx8rred7Dgd\_R5tbsTs5CH0knB9XXOyt9LViMCd7ri-n7UVRd82V7CvqBuGuEEhMppfY0C)

You can set up timing marks on any timing track manually, by placing your cursor on the waveform (above the grid) and while playing the sequence, press the ‘t’ key where you wish the timing mark to appear. This is equivalent to what is called a 'tapper' function.

You can also have xLights create fixed timing interval timing tracks by selecting the Metronome timing option and then choosing the timing interval.

### Fixed Timing Tracks

When xLights created a Metronome timing it is generated as a Fixed Timing Tracks. Fixed Timing Tracks are not editable and the timing marks cannot be changed. Fixed timing tracks are colored orange in the sequence tab by default.

![](<../../.gitbook/assets/image (246).png>)

To edit a Fixed timing track the user must right click and select Make Timing Track Variable.

![](<../../.gitbook/assets/image (302).png>)

### Adding/Removing Timing Track

While on the sequencer tab, you can add new timing tracks or delete an existing timing track at any time.

Right Click , with your cursor in the area of the timing track names and select Add Timing Track or Delete Timing Track.

![](<../../.gitbook/assets/image (461).png>)

### Importing Timing Track

You can also import timing marks created externally (the most common being those created via Audacity or another xLights sequence).

![](<../../.gitbook/assets/image (19).png>)

This capability includes importing a Singing Face (xLights Papagayo) timing track.

{% hint style="success" %}
If you wish to select and delete multiple timing marks all at once, uncheck the circle beside the timing track and then drag select with the yellow dashed rectangle and hit the delete key.
{% endhint %}

In order to import a timing track, right click the Timing names area, then select Import Timing Track, navigate to the .txt ,PGO, LMS, LOR, LSP, .xml, or .xtiming file containing the timing track and click OK to import it.

![](https://lh5.googleusercontent.com/J8qZGgZoqIRKz46RQp-d5N2l7THuYZy-8-VO7SJ-KykOUq5VS3qJqHuT6Bda0AAF5eA-De8MXzTNuttTKz9bxX8NM-OL3p7DIc5rOm40R1smp63EFYH3Xk3b9VZnClUfVn9mjj\_V)

The timing tracks from the specified file are imported as xLights timing tracks - the following is an example of one that has been imported from LSP.

![](https://lh6.googleusercontent.com/9IiCjGeeOHILUErIABDD6ozU4o2XWd2u9XEMizPcgW\_1Y1RU\_lLGOoZJSonMo9wvDksIP\_MLWQTYn4netGqbtDz6ZkV4EOFDh-OYDqrMsiu-0JftmmE676Duyf7uBxlk8bG31rGy)

Importing of a PGO timing track is covered elsewhere in the document.

### Exporting Timing Track

Similarly to export a timing track, right click on the timing track name in the Timing names area, and save as as .xtiming file.

![](https://lh6.googleusercontent.com/HtDtXuE-CenC5ngVjQ1n7nZMm4-2-Xgu-xe6ebX7zttXTg5Uqn3iBcxf7TOBMOHUw2kgnbpQ68tCvRl8AuL3NsyKTS07Bc6JblthK17uAgJVPduGQYeDGauvDzLa\_wL4sPZxQ1Dr)

This capability includes exporting a singing face (xLights Papagayo) timing track.

You can export the file as a PGO file , if you wish to provide the file for use in another type of sequencer (LOR ). If you wish to use this in for another xLights sequencer , then export as an XTIMING file.

![](https://lh3.googleusercontent.com/D8ra2mwK-xjBy6BKwMw9JRd94jx8VuSMUBTSxLSIFTsbTW0Q0uRVrMtrAlR7BXRe5yJR3x9ARkCtNlta1t\_XjJmi3chiwaQZM5w43zwWUv-\_8uG5bnrbZOK8tEZdK2pAeynjUf\_a)

Multiple timing tracks can be exported to a single XTIMING file by selected them from the following dialog.

![](<../../.gitbook/assets/image (368).png>)

{% hint style="success" %}
Timings are created just like effects which means they have a duration. Every timing effect has a starting edge and an ending edge. So you can have a timing effect that goes from 1 to 2 seconds and then another from 3 to 4 seconds with nothing in between 2 and 3 seconds. If you want one in there just select a range and hit "t" then drag the edges over to connect to the existing timing effects.
{% endhint %}

## Import Notes

The purpose of this function is to create a timing track by importing the notes from an external source such as a MIDI file, from an externally generated source such as Audacity or from a music XML file.

Right Click on the Timing Track name and select Import Notes.

![](<../../.gitbook/assets/image (259).png>)

Specify a name for the Timing Track to be created , the Notes Source, and then navigate to and select the file from which the notes are to be Import.

![](https://lh6.googleusercontent.com/7wqZ-7F9o5oYYuZi9ZVMg3uiLks1siB2K\_-UJhK7zvnjy\_9Ip9hiQrkD-ZhoZtbXe6E\_0bjDGqrkAVKS6GE36fxxuOjQeI0tVIjdcxkn\_p7Z9NYwhRNmxALmd1r4\_ZD4OL3LPonr)

Click OK and the Timing track will be created from the notes.

Once the timing track that has been created , it can be edited or adjusted if required.

Subsequently , when when using the Piano effect , specify the Timing Track that has been created as the Notes source.
