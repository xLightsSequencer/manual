# Glossary

## Bulk Edit

**Bulk editing** is a way to change the settings on multiple effects at the same time, rather than having to do each individually. Select multiple effects by highlighting them, and right click on the setting you would like to change.&#x20;

## Buffer

**Buffer** or Render Buffer is the 2D grid representation of a model or model group used to render the effects on. Each Model has a "Default" Render Buffer that can be viewed using the Node Layout Dialog. The Buffer settings are found on a tab of the Layer Settings Window.

## Channel

A **channel** is the smallest controllable element that xLights can control. The channel value may be set to on or off, or in many cases, a value that is between these two. Each channel has a level which is 256 "steps" divided over a range of 0 (off) to 255 (fully on). Below are some common examples of light types and channels.

* AC Lights (both incandescent and LED) will use one channel per outlet on the controller.  The entire string of lights reacts the same way when a command is sent to it, therefore all the lights are considered to be a single channel. &#x20;
* Dumb RGB lights will use one channel per color (Red, Green, and Blue) for each string of lights, or a total of three channels. The entire string of lights will react the same, and you can't control individual LEDs.
* Smart RGB lights will use one channel per color (Red, Green, and Blue) per node. Therefore, the total number of channels will be 3 times the number of nodes/pixels. Note that some strings of smart pixels will have multiple LEDs that will all react the same.  The number of channels is 3 times the number of chips that control the LEDs, not the number of LEDs itself.

## DDP

**DDP** (Distributed Display Protocol) is a high efficiency data protocol. It is more efficiency than ArtNET or E1.31. Currently, this protocol is only supported on a handful of controllers, NOT by all Ethernet based controllers. (only on FPP/Kulp, Falcon FW 2.58+, HinksPix, ESPixelStick, WLED FW 0.12+, Genius , and Minleon as of July 2021).&#x20;

## DMX

**DMX** or **DMX512** is standard protocol for digital communication that is commonly used to control stage lighting and theatrical effects. (ex: moving lights, color changing lights, fog machines, etc.). It has also been adapted to be used with many Christmas light controllers.

* DMX uses a RS-485 serial hardware interface.
* Each DMX signal/output is a set of 512 separate channels.
* Each DMX output of 512 channels is defined as a Universe.
* Each DMX device is addressed to specific DMX channel or range of channels.
* DMX devices can be daisy-chained together.  The last device may need to the terminated for the chain to function properly.

## E1.31

**ANSI** **E1.31** also known as Streaming ACN or sACN is a standard to transport DMX512 data over a IP networks. Protocol is supported by xLights and most Ethernet based hardware controller available today.

## Effect

An **Effect** is what xLights uses to determine which lights are on at which intensity and color on a model, submodel, or group.  See below for the Built-in Effects in xLights. Note that thru the use of layers, buffering render styles, and other options, additional effects can be generated from these.

{% content-ref url="../effects/off/" %}
[off](../effects/off/)
{% endcontent-ref %}

## Face (aka Singing Face)

**Faces** is a setting for each model which allows for the definition of certain parameters which allow the model to look as if the mouth is singing to the song. This requires a lyric track to function well.&#x20;

{% content-ref url="../chapters/chapter-four-sequencer/singing-faces/" %}
[singing-faces](../chapters/chapter-four-sequencer/singing-faces/)
{% endcontent-ref %}

## FPP (Falcon Player)

The **Falcon Player** (FPP) is a lightweight, optimized, feature-rich sequence player designed to run on low-cost SBC's (Single Board Computers). It was originally created to run on the Raspberry Pi, hence the middle 'P' in the short name. The FPP software runs on more than just the Raspberry Pi, such as the BeagleBone Controllers, but the name has remained. &#x20;

FPP is a software solution that you download and install on hardware which can be purchased from numerous sources around the internet. FPP aims to be controller agnostic, it can talk E1.31, DMX, Pixelnet, and Renard to hardware from multiple hardware vendors.

## FSEQ

This is the format that xLights sequences are stored in for playback on various platforms, most commonly xSchedule and FPP. &#x20;

{% hint style="warning" %}
The FSEQ file will become very large with high channel counts, long sequence lengths, or when certain effects such as video are added.  This can be of concern with small storage drives or slow connection speeds. &#x20;
{% endhint %}

{% hint style="danger" %}
xLights will not open FSEQ files to allow for editing of the sequence.  The XSQ files are used for the purpose.  A FSEQ file can always be generated from the XSQ files if the FSEQ files were deleted, but the XSQ files **cannot** be generated from the FSEQ files.
{% endhint %}

## Group (aka Model Group)

A **Group** is simply a combination of models and/or submodels. Effects can be placed on groups so that they will be displayed on multiple props or even the entire display. Note that the order of the models/submodels impacts how effects are displayed for certain render styles.

{% content-ref url="../chapters/chapter-four-tabs/model-groups.md" %}
[model-groups.md](../chapters/chapter-four-tabs/model-groups.md)
{% endcontent-ref %}

## IP

**IP** or IP address is the numerical label assigned to each device connected to a computer network.

## Matrix

A **matrix** is simply combination of rows and columns. Most commonly, a matrix is a model that is made up of panels (P5 and P10 being the most common) or pixels laid out in a grid fashion.

## LOR (Light-O-Rama)

**Light-O-Rama** is a company/lighting system designed for animated lighting displays. All in one system with proprietary software and hardware. Some of the LOR protocols/standards has been reverse engineered and ported to xLights. Currently Supported LOR devices and formats

* Importing of S2, S4, S5, SuperStar and Pixel Editor Sequences
* Controlling LOR controllers in DMX mode.&#x20;
  * Must be configures with the LOR Hardware Utils
* Controlling LOR controllers in LOR protocol mode with a LOR dongle.
  * Not Recommended if DMX mode is available.
* Converting LOR Singing Faces Channel Data to Phonemes data.

## Model

A **model** in xLights defines the entire required characteristic about a single physical element(prop) in your display.

{% content-ref url="../chapters/chapter-four-tabs/models/" %}
[models](../chapters/chapter-four-tabs/models/)
{% endcontent-ref %}

## Multicast

**Multicast** is a one-to-many communication technique over an IP network. A data packet sent from a device and can be received by multiple endpoints. It can be more efficient as no acknowledgment from the receivers is required, but sends more information over the network.

## Node

A **node** is the the number of controllable elements on a string of lights. It is a combination of Red, Green, and Blue channels in any order. This can be, but is not necessarily, the same as the number of LEDs.  Some strings will use multiple LEDs in a single pixel. All LEDs that act together based on the wiring of the lights are considered a single node. Each node consists of 3 channels.

## Null Pixel

A **null pixels** is a pixel that is used to pass data to other pixels, but does not light up itself. The controller setting must be configured to skip these pixels.

## Pixel

**Smart Pixel,** or **Pixel**. Each individual LED is addressable. In xLights, taken to be the as the same as a Node.

## Port

The physical output number of a connections on a controller.

## Presets (aka Effect Presets)

**Presets** or Effect Presets are a way of saving an effect or effects, including their settings and/or layering, so that it can be easily available for use in the same or other sequences, or shared with others.

{% content-ref url="../chapters/chapter-four-sequencer/effect-presets.md" %}
[effect-presets.md](../chapters/chapter-four-sequencer/effect-presets.md)
{% endcontent-ref %}

## Render

**Rendering** in the process which xLights uses to take the effects on the sequencer tab and generate them on the models. Rendering will generally take place automatically when working with a single effect on an existing model. When working with groups, layers, or making large amounts of changes, Rendering all is often needed.

## Sequence

A **sequence** is the file which contains the information about which effect is placed on which model, in order to make the actual lights display. There will be two files for each sequence - the XSQ file, which is used by xLights to generate the data, and the FSEQ file which is used by the show player to control the lights.

## Show Directory

The **Show Directory** or Show Folder is the folder location on the computer's hard drive where xLights will store all the light show related files and data.

{% content-ref url="../chapters/chapter-four-set-up/directories.md" %}
[directories.md](../chapters/chapter-four-set-up/directories.md)
{% endcontent-ref %}

## Strand

A **strand** is the number of times a string of lights folds or zig-zags back and forth. For example, a string of lights that starts at the bottom of a model, goes up, down, up and finally back down would have 4 strands.   The total number of pixels per string is divided equally to each of the strands.

## String

A **string** in xLights is the number of physical connections to a controller. It is **NOT** the number of physical strings that are connected together.  For example, in xlights there is no difference between 1 physical string of 250 pixels and 5 physical strings of 50 pixels each connected or spliced together - both of these would be seen as 1 string of 250 pixels in xLights.

## Submodel

A **Submodel** is a selection of the full model. This allows you split models into smaller parts for sequencing.

{% content-ref url="../chapters/chapter-four-tabs/sub-models.md" %}
[sub-models.md](../chapters/chapter-four-tabs/sub-models.md)
{% endcontent-ref %}

## Unicast

**Unicast** is a one-to-one transmission from one point in the IP network to another point. The sender and receiver, are each identified by a IP address.

## Universe

A **Universe** is a grouping of channels normally totalling 510 or 512 channels. In DMX a universe is one physical output on the light console. With E1.31 it is used to group channels into blocks for sending over Ethernet.

## Value Curve

A **Value Curve**, allows an effect or sequence setting change over the duration. For example, if the user wants to increase the line thickness of an effect, a "Ramp" value curve would be used on the line thickness setting. Value Curves can also be manually defined by the user.

{% content-ref url="../chapters/chapter-four-sequencer/value-curves.md" %}
[value-curves.md](../chapters/chapter-four-sequencer/value-curves.md)
{% endcontent-ref %}

## XML

**XML** is a file format used to encode program data. XML is human-readable and machine-readable making it easier to decipher if needed. Most data is xLights is saved in a XML format.

* "xlights\_networks.xml" - XML file containing Controller Tab data.
* "xlights\_rgbeffects.xml" - XML file containing Model Settings, Groups, Views, Perspective, Effect Presets, and Color Manager Data.
* "xlights\_keybindings.xml" - XML file containing Keyboard Shortcuts data.

## XSQ

**XSQ** is a file extension used by xLights for sequencing files. The XSQ file is encode in XML format.&#x20;

* "sequence\_name.xsq" - XSQ file containing Sequencing data.

## xSchedule

**xSchedule** is the 'builtin' Show Player installed with xLights. The user can create song playlists and schedule when to play the playlists. There is a build in web interface, for show control from you smartphone or tablet. See the xSchedule manual for more information.

## Zig Zag

**Zig-Zag** is the number of 'folds' in a string of of lights. This can normally be defined in the controller or xLights, but it is recommended to use xLights when possible.&#x20;

## Zoom Room

The **Zoom Room** is a online meeting room with audio and video, where users can meet for technical support. Participants can share their computers desktop for remote assistance. It is Recommended to have a microphone to help other participants talk you through the issue. It is also possible to use your phone and call in for audio only assistance. There is a "Official" US meeting at every Wednesday 8pm EST , and Australian meeting every Friday, 8pm AEST. The Zoom Room is open 24/7 and can be used anytime for tech support questions.
