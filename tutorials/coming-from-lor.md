# Coming from LOR

## Running LOR Controller in DMX Mode

### LOR to DMX Channel conversion

The following table describes the conversion of a LOR Unit id to a DMX address. As an example, if you have a controller with a Unit id of 03, then when converted to run under DMX, the channel ranges will be 33 to 48.

| LOR Unit ID | DMX Address | LOR Unit ID | DMX Address |
| ----------- | ----------- | ----------- | ----------- |
| 01          | 1           | 11          | 257         |
| 02          | 17          | 12          | 273         |
| 03          | 33          | 13          | 289         |
| 04          | 49          | 14          | 305         |
| 05          | 65          | 15          | 321         |
| 06          | 81          | 16          | 337         |
| 07          | 97          | 17          | 353         |
| 08          | 113         | 18          | 369         |
| 09          | 129         | 29          | 385         |
| 0A          | 145         | 1A          | 401         |
| 0B          | 161         | 1B          | 417         |
| 0C          | 177         | 1C          | 433         |
| 0D          | 193         | 1D          | 449         |
| 0E          | 209         | 1E          | 465         |
| 0F          | 225         | 1F          | 481         |
| 10          | 241         | 20          | 497         |

## Running LOR in DMX mode

The following diagram shows an example of how LOR controllers can be connected in DMX mode. Refer to the table above of Unit IDs to DMX channel conversions.

![](https://lh6.googleusercontent.com/ZnAkRO230t1gqoo\_oKnf70rwFxwfDi66PQRTNIqSFZwPKM-QejOmY4uKxCuHnxdRMZa8KacviV7vF68Kw3oEX\_IDgj\_0ns0WHrzGnW-WPillGrK4ZFDGeYSx9iL278KRv2gHiAL2)

![](https://lh5.googleusercontent.com/YneUk4XYocaquvQJ45Lz95Mn-t1cQsWSX4-f1Sf0PRVZrQ8nsh7YbZ3POWv1pro3QaPHINc94556KPVyrRJ2DZII9VwVuZLCIPOnRxvbbgRxyAv4VDdHjh0GtngpwDvzl4QbO0nI)

You must use the LOR hardware utility to set the DMX start address on a LOR controller if the controller doesn’t have on board channel selection. The next diagram shows an example of how LOR controller addresses are set in a DMX universe. The controllers do not need to be physically connected in order of the controllers start address. The controllers can be put in any order.

![](https://lh5.googleusercontent.com/bwNbH862Xcn265vgIp9p5u2jNRvmQGWUFP6a7\_\_1QU8-5YH60MmcrVzXf64VzbQxDRVa0bOyH-kis5lxri-L6s-uzDj7RRE5BF2BJ9SRNj9Cl8DGEVNQlX049zEfjGIPSeIUeIi-)

## Convert a LOR LMS file to play using non LOR hardware

_This section is based on a video created by Steve Giron_

The item to be converted is a purchased 12 leg CCR tree sequence. The input file should be in LMS format. Within xLights, go to the Convert tab and from there Select Convert, navigate to where the LMS file is and select it. Select the ‘Show Verbose Channel Map’ attribute. ‘Click on Start Conversion.

If you get an error “Unable to determine the length of this LOR sequence (looked for length of track 1)", it usually means that the LMS sequence has been saved using the demo software. The lms file from demo LOR is mostly binary and does not contain the xml tags.

Error messages are expected for the first run in the status window on the right side. Scroll to top of error messages and look at messages that says “LOR Network”.

![](https://lh6.googleusercontent.com/Z7iMVto0yQ4ovhbQ6Y8mFiNHij8xgh4ICZBK6G3wzC4PBLbSqINlqD\_ke8KcEFFY4cgbTOeCNq6TJo\_PRRVIfRQ57j6athzg7O-UN1chIFWBCvujrdXpunOu3deRAUJ\_tYDZvzYj)

The messages tell us that two networks are required: One with zero channels – (this was a star where channels were deleted from), one with 1800 channels.

Go to the Setup tab and define these.

Setup tab (Existing layout)

![LORSetupSteveVideo12CCR.png](https://lh5.googleusercontent.com/OfRngi4xLauRTtGkSRhbP240dQqsWGuRklpccVuXbuJk6bII-aqXegb56H45DUnste3KKvqQMX8MyCq53zJ5Oa\_bI6459KapZNEd5QaSHkVkSEr2JK8T5VL8CyvxGzuErQfnXbcP)

Add two entries: Network type of LOR, any baud rate, however the last channel must map correctly. Then move them to the top using the green UP arrows.

![LORSetupSteveVideo12CCR\_3.png](https://lh6.googleusercontent.com/NWdwSFkClg\_1KGeDwMJSw0qiqtyeq7iAPh9V5zP1nO29BvSPF775GyYVHmto1kYndSS0F8YSDLMYFXoylVczfKp-D3MhU6QFWHRF\_7EKVnu3aAiIjHPuY3rJS\_89UNMYOUCh7xlS)

Ensure that ‘Map Empty LMS Channels’ is not selected (else you may get errors as the CCR macros do not have effects in them). Reconvert and it should convert with no errors.

Open the xseq file that was created and play it to view the effects on the layout window. You may need to click on the ‘Render All’ button.

If you are not playing the sequence though LOR hardware, go back to the setup and delete the two LOR entries that you added for the conversion, leaving your previous configuration as it was. If you are using LOR hardware, then these entries will need to be correctly defined.

## Converting a LOR sequence and importing into xLights

_This section is based on a video created by Clyde Lindsey._

First ensure that within LOR, all the channels for the controller have been defined and are in sequence. Tools, Channel configuration will display an image similar to the following.

![LOR\_CL1.png](https://lh6.googleusercontent.com/ueA25UCiy5Kg3nYFYwDUT4lAwo-okjG5NVRj8HIhSEqUCwDlQ7nCQFPBnH\_nw9sRRRbK8HSMN-NbNGhCKycEmQCQWTga0LpHJQku0L6m-sSzUAXINUGy-znWKjVlHEko9t9dx\_ED)

If there are any channels missing use the ‘Add Channels’ function to add the missing (unused) channel.

Note that in the image, the Unit id is 03 and the Channels (Circuit) values run from 1 to 16. However, referring to the LOR Unit Id to DMX channel mapping table Unit id 03 corresponds to Channel number 33. If Units prior to Unit 3 have not been defined, then you need to define them so as to ‘utilise’ the missing channels. Use the ‘Insert Device’ function to ‘Insert Device Above’ the current device (Unit 03) as a LOR 16 channel device – Unit id 01. Repeat this step and add another device - Unit id 02.

![LOR\_CL3.png](https://lh6.googleusercontent.com/TMsj0Wj7j\_OYfu91NxH1jrX2Cqp71n9fRkOlYdDnfLYolOvE6s87Gzxn7g9VSxzIolpSEHp2qfvBp6tQsyCsSQqQxCOatDg9uX-c8bkPGEpHBk\_SS14OTDWyRLkvQWz8puzxbtPa)

Therefore Channels 1-32 (Unit 1 and 2) have been defined – even if not required in LOR, and channels 33 – 48 belonging to Unit 03 are the ones that we are interested in.

![LOR\_CL4.png](https://lh3.googleusercontent.com/nylhTMxJt0jpgb4f4vJmQZ5Ej-PqowQGcC6JVeM6LRf166NhBzEn8vfkzCVWAM4YF0Wn-0T0eLm6Wt1PEZBrArelabYrKf6sNLh5wuV8FiF6k11tGIFcfCW4g0kbNJlopYhu04zY)

On the xLights setup screen, the corresponding channels must be defined.

![LOR\_CL5.png](https://lh3.googleusercontent.com/0hXyxhjSE80UEjNUtk-9cQ3jlgq1euPnMr-tal1aQko8Pemqk6QALsVk5T33FgZIPFNvniyzaqoWBtePhDd2zGqQ0UONzjtI\_xocO90CCbqq70CfvytrENeQ\_NIDkZAjsqhizeGM)

You can define it as a USB, with a network type of LOR, and set up the COM port (obtained from the LOR device manager) and you will need to try different baud rates.

However, there is sometimes a lag associated with the sequence when you use this option.

It is preferable to use a DMX (to E131) bridge if possible and then define the channels as E131.

![LOR\_CL6.png](https://lh4.googleusercontent.com/jzlnAK\_PJ4PEiabryFk3r8YcZbZAnz\_gjGW0adfQsZIPzaJ6ijipuTU-fSSf4sbxteZ\_LIM-scsz4S2JgJdR9MzCRxenJoNUlo7RloCiebOIyophcYBKVVA0h6W9tmqpAJFqPtPo)

For the three devices were defined in LOR, only 48 channels need to be defined, but to preserve a buffer for future use, an extra 16 channels corresponding to an additional LOR device, (i.e. a total of 64 channels) will be defined in Universe 1 as E1.31.

### Model definition

Next create a new Model definition that matches the LOR Channels of Unit 03.

![LOR\_CL7.png](https://lh4.googleusercontent.com/kXBZix47UelIC-eQuCywyajeQ78xlkDuiR\_okYsJF3Yjf8azVXX0F7zEd\_A3dhpzOx3hJvtAj2wvF\_0PTR\_Y-HacEKGpbzsHFHc132Mg6atkjmAu2iZhMpvME1Vnd9IqN1tV4yHf)

Let’s say that this was 16 single channels Trees. In that case create a model ‘Small Tree 1’, with 1 channel. The start channel must be set to 33 (not 1) as this corresponds to the 1st channel of Unit 3.

Then you can copy the model, update the name (Small Tree 2) and change the starting channel to 34 and repeat this for all 16 channels, increasing the start channel by 1 each time until the last one is 48.

{% hint style="success" %}
If within the LOR Unit 03 definition, there are unused channels, you do not have to create a model for that channel or channel range. For example, let’s say within Unit 03, channels 10-14 are not used. In which case, you would create 9 Trees (1 -9), and then another 2 trees (for 15-16). This is different to the setup tab where you must cover the entire range of channels from 1 onwards.
{% endhint %}

The next step is to use the Layout tab to align the models (the Trees) as required. Save the model definition.

### Import sequence data

Create a new music sequence, add timing tracks and add the models you have defined to the sequencer tab.

Using the Import, Import Effects menu, change the ‘Import file’ file to LOR Music Sequence - LMS, navigate to where the LOR LMS file is and select the file to Import.

![](<../.gitbook/assets/image (850).png>)

On the Map Channels dialog, all the xLights models will appear on the left hand side and all the LOR Channels on the right side.

![](<../.gitbook/assets/image (708).png>)

Do not select the Map by Strand/CCR option in this case.

Highlight the 'Map To' Cell – in line with the model name. Double Click the LOR model name (as identified by the labels in LOR) in the right 'Available' list. You can also drag and drop channels from the 'Available' list to the 'Map To' column. Repeat this for all the channels.

When Done, Save the mapping first, so that you can re-use it later.

![](<../.gitbook/assets/image (331).png>)

Click OK to start the process.

![](<../.gitbook/assets/image (427).png>)

Double Click the model name and then double click the stand name to see the effects on the nodes.

![](<../.gitbook/assets/image (261).png>)

Click on the Render All icon and play the sequence.

![](<../.gitbook/assets/image (731).png>)

{% hint style="success" %}
**If you were importing data from a Singing face where your model has multiple channels, then you need to double click in the Channel column, but against the node row instead.**
{% endhint %}

{% hint style="success" %}
**The Convert tab has an option to ‘convert a LOR sequence file with a ‘Show verbose Channel map’ setting that will provide details of the LOR to xLights channel mappings . You can simulate a conversion and review the mapping details first.**
{% endhint %}

Instead of using the Import tab to import the data as an editable effect, you can also import the data as a Data Layer. The process is much more efficient, however you cannot directly edit the data after your have imported it. That option has also been described in this chapter.

## Common Scenarios

### Scenario 1

A user is still using LOR for 8 controllers this year. How should he set them up ? Should he run it in DMX if the controller support DMX?

The general rule is that you can do 96 channels of LOR with xLights if the LOR controllers are in LOR mode. In this case, put the LOR controllers in DMX mode and then xLights can do it all. The user can can import all the LOR sequences, schedule them play them, edit them, etc.

### Scenario 2

A user has an E682 and an E6804 running pixels and 2 CMB16 and 1 CMB24 controllers. How should they be configured and connected ? Is a cross over cable required?

Plug in the USB, same com port that would be used, if running it from LOR. No crossover cable is required if running from a LOR network. On the setup screen, add LOR channels via USB device. Put in at least 48 channels. Set the com port as required. After the LOR USB row, add in universes of 510 for the E68x controllers.

### Scenario 3

A user is using comm4 and the USB to ethernet dongle. How should they be configured?

Network Type – LOR, Port – COM4, Baud rate – 57600, Num channels (160 as example).

Note: Baud Rate of 250000 is for DMX only.

### Scenario 4

A user is setup is a mixture of LOR and DMX Channels i.e. intermixed LOR -DMX-LOR-DMX.

LOR Controller 1, LOR Controller 2, LOR Controller 3, DMX Universe 1 ch. 1-126,

LOR Controller 4, LOR Controller 5, DMX Universe 1 ch. 127-183.

How should this be configured?

#### Option 1

Use Universe 1 for all the LOR and DMX channels.

Since the DMX is already set (channels 1-183), add an LOR entry with Universe 1 starting at 184 until the last channel for controller #5 (16 x 5 = 90), for a total of 274 total channels. You can 'reserve' additional channels should you need them later upto 510/512.

#### Option 2

Keep it simple with DMX - Universe 1, LOR - Universe 2 and then start with Universe 3 with the RGB controllers.

{% hint style="success" %}
All the channels in LOR must be mapped exactly including blank ones in between. Setup your AC LOR channels first in XL4 and then start with your first prop in the same order as your LOR sequences. Otherwise the convert process will indicate that channels are unmapped.
{% endhint %}

{% hint style="success" %}
LMS to xLights XML via Import Effects is done via model mapping so channel numbers don't matter. However, if using the LMS to xLights via Data Layer import option, channel numbers need to match models between LMS and xLights configurations.
{% endhint %}

{% hint style="success" %}
When importing timing grids, xLights searches the LMS file for a section called \<timingGrids> which needs to contain a subsection called \<timingGrid> which must contain an attribute called "type=freeform". So, in case you can't import a LOR timing grid, you can open your LMS file in any editor that can view XML in a nice format like, Notepad++, and search for some of those terms to see why your timing grids aren't found inside the file.
{% endhint %}
