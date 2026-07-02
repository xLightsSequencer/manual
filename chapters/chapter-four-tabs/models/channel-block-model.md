# Channel Block Model

## Channel Block Model

The Channel Block can be used to define an arbitrary amount of channels. It can be used to 'model' generic channel to be used or AC Lights, relays, smoke machines, etc.

![](<../../../.gitbook/assets/image (293).png>)

### # Channels

Number(#) of Channels defines the size of the channel block. These Individual channels can then be used to control specific channels on a device or controller.&#x20;

### Channel Color

Channel Color determines what color in the sequencer will "activate" this channel block channel. If set to 'White' all three RGB channel values will be use to set the output channel value. If set to 'Red' only the Red channel values will be use to set the output channel value.

#### ![](<../../../.gitbook/assets/image (86).png>)&#x20;

## Model Settings

<!-- TODO: screenshot -->

| **Options/Setting** | **Description** |
| --- | --- |
| **# Channels** | Number of channels in the channel block, defining its size. Range 1-128. Each channel can then be used to control a specific channel on a device or controller. |
| **Indiv Colors** | Group header for the per-channel color settings below (read-only). |
| **Channel Color (1, 2, 3, ...)** | Sets the color that "activates" each individual channel in the block. One color entry is shown per channel. If set to White, all three RGB channel values set the output; if set to Red, only the Red channel value is used. |
