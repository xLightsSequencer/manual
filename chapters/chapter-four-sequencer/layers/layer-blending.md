# Layer Blending

## Layer Blending

![](<../../../.gitbook/assets/image (318).png>)

The Layer Blending window can be opened by clicking on the Layer Blending icon from the toolbar or via the View , Windows menus.

![](<../../../.gitbook/assets/image (666).png>)

#### Reset panel when changing effects

![](<../../../.gitbook/assets/image (269).png>)

This will reset the Layer Setting back to default every time you select or create a new effect. Checked is the recommended setting for most users.

## Layer Blending

![Layer Blending Dropdown](<../../../.gitbook/assets/image (57) (1).png>)

The Layer blending settings allows the user to dictate how effects on multiple layers will be merged together for a model/group/submodel.

When setting the layer blending modes, the current layer is considered layer 1 and the layer below is considered layer 2.

Click the Question Mark(?) Button for more Information.

![](<../../../.gitbook/assets/image (220).png>)

{% hint style="success" %}
Put two effects on a model and step through each of the layering modes to see what they will look like. Experience is much better than reading about it.
{% endhint %}

| ![](<../../../.gitbook/assets/pasted image 0 (7).png>) | ![](<../../../.gitbook/assets/pasted image 0 (8).png>) |
| ------------------------------------------------------ | ------------------------------------------------------ |

| ![](<../../../.gitbook/assets/pasted image 0 (9).png>) | ![](<../../../.gitbook/assets/pasted image 0 (10).png>) |
| ------------------------------------------------------ | ------------------------------------------------------- |

| ![](https://lh6.googleusercontent.com/8VqltNyiMNdMWdJ9jyiA8KO0CpuKyR\_GEZoDMDUZjQWcU0Lt6YX3fcZdJeFsn3BMQt2S2iVW5pd5P2h4coQj4AfvCc8UkTJxMCq9ef8N2GfX9oA8AKCesTpBxdhoxUk22DU19qaS) | ![](https://lh3.googleusercontent.com/\_3XMHX4fBN9nrSRO1xUp1Pb\_07nP9I2pTyIWslOF\_yX1uI1MVuMsgkCYyQIiFfrGzzAomcTHa2eTOzidsQQjeeZgsNfFR6\_tekDyRAKkEaHuq15fLcbjTjJ2jYhvNuy0DFY\_P4HL) |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |

| ![](<../../../.gitbook/assets/pasted image 0 (13).png>) | ![](<../../../.gitbook/assets/pasted image 0 (14).png>) |
| ------------------------------------------------------- | ------------------------------------------------------- |

| ![](<../../../.gitbook/assets/pasted image 0 (17).png>) | ![](<../../../.gitbook/assets/pasted image 0 (18).png>) |
| ------------------------------------------------------- | ------------------------------------------------------- |

| ![](<../../../.gitbook/assets/pasted image 0 (16).png>) | ![](<../../../.gitbook/assets/pasted image 0 (15).png>) |
| ------------------------------------------------------- | ------------------------------------------------------- |

### Morph

This is not to be confused with the Morph Effect. This is a layering option that can be applied to any two effects.

![](<../../../.gitbook/assets/image (541).png>)

The morph option of layer blending will magically make effect 1 ‘morph’ into effect 2 during the length of the timing cell that the effects are in. You will not see effect 2 at the beginning of the timing cell, and you will not see effect 1 at the end of the timing cell. Somewhere near the middle you will see the effect 1 ‘morph’ into effect 2.

### Suppress Effect Until Frame

This will hide the effect for the specified amount of frame and display it when the number of frames is reached. This can be used to "warm up" an effect and hide the undesired beginning frames.

### Freeze Effect At Frame

This will pause or stop an effect at the specified frame and hold that frame and display it until the end of the effect.&#x20;

## Transitions

There are 19 layer blending transition choices. Using the transitions will help you bridge between effects providing a way to smooth out abrupt changes between different effects. A stylistic use would be between sections of a song such as the chorus to verse or verse to verse. Keep in mind that the blending is done within the boundary of the timing mark and does not transition between timing marks.

![](<../../../.gitbook/assets/image (227) (1).png>)

These transitions are common in the video editing world, and should be visually familiar to anyone who’s used video editing software or anyone who’s watched anything on TV in the past 20 years.

{% hint style="success" %}
When setting a layer transition, the setting will apply to all future effects placed, so be sure to reset the transition times back to 0 if you do not wish the transition to apply to all future effects.
{% endhint %}

| Transition     | Description                                                                                                                                                                                                                                                                                                               |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fade           | The Effect with gradually disappear or appear.                                                                                                                                                                                                                                                                            |
| Wipe           | A line travelling from one side of the frame to another will cause the effect to disappear. The adjustment slider sets the starting wipe direction. 0 is from the top, 25 from the left, 50 from the bottom, 75 from the right.                                                                                           |
| Clock          | This uses a circular motion as the hand of a clock from the center of the model to wipe the effect in or out. The adjustment slider sets the starting position and the reverse checkbox allows for a counter clockwise wipe.                                                                                              |
| From Middle    | This is a curtain type wipe either from the middle or towards the middle depending if the effect is placed on the in transition or the out transition. The reverse makes the effect operate in a “to the middle” mode instead of “from the middle”. The adjustment slider will change the angle of the curtain direction. |
| Square Explode | This transition will draw the effect starting from the middle of the model and expand outwards with square edges until the model is filled. The reverse button starts drawing the effect from the outer edges and filling in towards the middle.                                                                          |
| Circle Explode | Same as square explode, except the shape is circular instead of square.                                                                                                                                                                                                                                                   |
| Blinds         | This transition is analogous to twisting the wand to open vertical blinds. The adjustment slider determines how many blinds are used. The reverse checkbox determines the direction that the effect will fill in from.                                                                                                    |
| Blend          | This transition effect when used as an “in” transition rapidly fills the model with square chunks until the model is full. Likewise when used as the “out” transition, square chunks of the effect disappear until no pixels are left. The adjustment slider determines the size of the chunks.                           |
| Slide Checks   | This transition is a checkerboard type transition where the effect starts out with a checkerboard type of mask on the model and then the black portions are filled in either left to right depending on the reverse button selection. The size of the pattern is set via the Adjustment slider.                           |
| Slide Bars     | This transition is broken up into 1-24 horizontal slices of the model determined by the Adjustment slider value. The effect selected will be filled in from opposite sides of the model interlacing each section until the model is filled.                                                                               |
| Fold           | This transition bends the effect onto itself like a piece of paper.                                                                                                                                                                                                                                                       |
| Dissolve       | This transition will cause the effect to appear/disappear by adding/removing random pixels.                                                                                                                                                                                                                               |
| Circular Swirl | This transition will cause the effect to appear/disappear by emulating an object's rotation.                                                                                                                                                                                                                              |
| Bow Tie        | This is a wipe transition using a Bow Tie Shape. The adjustment slider sets the starting location, 50 is the middle. The reverse checkbox will flip the direction.                                                                                                                                                        |
| Zoom           | The effect will start out large and shrink into place.                                                                                                                                                                                                                                                                    |
| Doorway        | The Effect will start/end as a small box and increase/decrease size to fill the frame.                                                                                                                                                                                                                                    |
| Blobs          | This transition will cause the effect to appear/disappear by creating random rounded shapes on the frame.                                                                                                                                                                                                                 |
| Pinwheel       | This transition will cause the effect to appear/disappear using blades like a fan. The adjustment slider sets the number of blades on the pinwheel.                                                                                                                                                                       |
| Star           | This is a wipe transition using a Star Shape. The adjustment slider sets the number of side of the star. 40 for four sided star, 50 for for five sided star, etc.                                                                                                                                                         |

If an effect has a transitions applied a green bar will appear for an in transitions and a red bar for an out transitions. If the in and out transitions overlap, the overlap area will appear yellow.

![](<../../../.gitbook/assets/image (602) (1).png>)

## Mix Slider

This slider adjusts the level of each effect in the combined output of the effects. You can use this to just put a hint (or more) of one effect on another.

![](<../../../.gitbook/assets/image (159) (1).png>)

## Canvas

![](<../../../.gitbook/assets/image (524).png>)

Canvas Mode is a special render mode that only works with specific effects. The default render mode in xLights will draw the effects on a blank buffer for each layer. Canvas Mode allows an effect to draw on a previous layer without "blanking it" out. This is used by effects like the Warp and Kaleidoscope Effect that manipulate data from the underlying layers.

### Canvas Layer

This Dialog allows the user which layers to use when Canvas Mode is Enabled

![](<../../../.gitbook/assets/image (746).png>)

![](<../../../.gitbook/assets/image (245) (1).png>)
