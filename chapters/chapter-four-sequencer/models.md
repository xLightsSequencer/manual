# Models

## Models

![](<../../.gitbook/assets/image (867).png>)

### Play

If the Model Preview window is open, you can play the model effects in the window by right clicking to the left of the sequencer grid and selecting Play Model. The sequencer will start playing and the effects in this window will focus on the selected window.

You can also achieve the same result by clicking on an effect against the model in the grid and then selecting Play.

### Export Model / Render and Export

This function is used if you wish to export effects from your model to another sequencer, such as LOR, LSP, Vixen, HLS. It can also be used to export an eseq (effect sequence) to the Raspberry Pi Falcon Player (FPP). Effect files are .fseq format files with an .eseq extension. These special sequence files contain only the channels for a specific effect and always start at channel 1 in the sequence file. The actual starting channel offset for the Effect is specified when you run it or configure the Effect in an Event on the FPP.

{% hint style="success" %}
Eseq (effect sequences) can be played on the FPP any time while a main fseq sequence is running and you can have as many effect sequences running as you want on different elements of your display. If you create an fseq called ‘background.eseq’ and upload to the FPP, it will execute as soon as the FPP has started i.e no definition is required on the FPP.
{% endhint %}

Right click to the left of the sequencer grid and select Export Model or Render and Export Model.

‘Render and Export’ renders the model to a clean buffer and thus would ONLY contain the data from the effects on that model.

‘Export Model’ could include data from other sources that may affect the model such as data layers, model groups, overlapping models.

You will then be presented with a window where you can select the target sequencer type and the filename to be created. Press OK when done.

![](https://lh3.googleusercontent.com/miuvCLx-mnpzpYNynWbSiNFXre3pepR7dSInWLWVssKNmqYXrnydCtF\_Pav8XFnYN8qi2ldVxTqDBmEoOY3J-9qfmD2\_3Z\_2bZBXCMxCmpC8sYZ9\_YeTnmXau7qnxdgHwiVLPcL5)

Status messages will be displayed on the last line of your sequencer as the model is exported. The file will be created in your show directory.

{% hint style="success" %}
You can use this functionality to export a models effects to the Falcon Player and then use the effect to run a continuous background sequence such as a “Tune to” sign, independently of sequences running in via the fseq file.
{% endhint %}

### Model Export as Video

You can export your effects as a video avi file. It is limited to matrices, trees and custom models. It generates a low res video which can be used in the video effect or in other sequencers. Right click against the Model name on the sequencer grid, select Export Sequence and then select either Compressed video or Uncompressed video. Enter the filename and press Ok. The avi file will be created in your show directory.

![](https://lh3.googleusercontent.com/CiTQL-Yl48h9ka0GcE45wx3gr038d2Hd0F265SQL3sEKNogeH4XwICO\_gKV50KkDe4BpuVb3\_MBKwswUWV0L2c8P98N\_QEQcZm5VdxfdiMVR0M-i668JPOrMRgctQjwDAeUL03gf)

### Toggle Strands and Nodes

From the sequencer grid view, right click on a model name, and click on the Toggle Strands option, to display all strands for the model.

![](https://lh6.googleusercontent.com/VAwXGBAL1Z0m1ub95jLAvJNwWN7j3pXOkosX5VszdOnC0FeCmqulryRIPSIs\_CRaCNbq30leT5Gh0pkN7NBo-MRcuv-wHLbvQ8UP92EXicag-M-Tv30jVZ0wNYFhtSdG3dpvur7s)

With the strands view open (i.e. displayed), right click on a strand to either toggle the strands closed or to Toggle Nodes and display the nodes for a strand.

This is often useful to see how a particular effect has been rendered down to the node level.

{% hint style="success" %}
Dropping an effect on a Model group will give different results than dropping the same model on all elements of the group (because in the former case the canvas is treated as a whole matrix and then the effect is applied to the models within it). Some effects work at the Group level better than others.
{% endhint %}

{% hint style="success" %}
If a model has sub-models they will be listed above the strand names. You then can use these to define an effect applied only to the sub-model.
{% endhint %}

On the left column of the sequencer tab, Model Groups have a symbol after the name that distinguishes them from Models.

![](https://lh4.googleusercontent.com/DayFHnCuM8LjP1GA5bJ6mLhWc557P7NrTrPp1NRXsdznnRo\_Lwzslv-SuaYlQnBtN0twvhnGh4VgNnO4SKEuDVgIjfY55ZOo8K2kHMcCzQxScfXOzq6O9ULGyG2ezl37nyhwwomR)

![](https://lh4.googleusercontent.com/I7prOUGhYLcNktyNWIY-TlAMx371gZR2Vnx1nJR774fkkIpR6PldNs0qKqQeGan2nZweuBHnSdtRJdJMj8NvBH0Oxjd3V7ztX1ZcKaWziwWa4j8oX6lKdhKoHzEooa6cYJYqKlcO)

{% hint style="success" %}
When on the sequencer tab, If you right click on a Model group, the window will display a ‘Toggle Models’ option which will display all the models under the Model group (or hide them if you select the option again). You can also double click on the Model Group to obtain the same results.
{% endhint %}
