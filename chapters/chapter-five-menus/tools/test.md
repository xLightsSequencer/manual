# Test

## Test

The test tab enables you to test anything from a single channel; all channels for a model, group, or universe; or all channels by sending test patterns to the physical lights.

{% hint style="warning" %}
The controllers and lights must be connected to the computer running xLights in order for the test feature to work. The connection may be wireless or wired, but a means of communication is required.
{% endhint %}

{% hint style="warning" %}
Testing from xLights, especially when using multicast may flood your network with data, and result in slower network connections. This is especially noticeable when using the Zoom Room for live assistance.
{% endhint %}

![](https://lh5.googleusercontent.com/0Dm4AzgxkGb-lfbRgygMuSwoOJ0K0UiRCaOJljoXv5qhFzxBO-nTPhZVS4Rm3QdmNTy8taq2gHSnbWRL8vGZbdlNBctKmISkDPfe5o3zRjA89QL0J4qOTBqUqaWi2MwiXY66R0Rh)

Ensure that output is enabled by selecting the "Output To Lights" button (it should be selected by default).

![Test Dialog](<../../../.gitbook/assets/image (763).png>)

## Selecting What to Test

When you first access the Test Dialog, you will be presented with three tabs. The first tab is a view of all the channels configured against each ‘Controllers’, with output (Universe/Channel range) defined in the Controller Definition shown under the controller name. You can click against the Controller or Output to select or deselect all channels beneath.

![](<../../../.gitbook/assets/image (759).png>)

Once you have selected a set of channels, you can save this individual set up as a test configuration for future repeat testing by clicking on the Save button and specifying a name for that group of channels. You can load a previously saved test configuration by clicking on the Load button.

![](<../../../.gitbook/assets/image (75).png>)

If you click on the second tab labeled 'Model Groups', the view with display all the Model Groups. You can then select one or more Model group to test.

You can also click against a Model Group which will then display all the models under the group. This is quite useful to test a model or group of models at a time.

![](<../../../.gitbook/assets/image (733).png>)

The third Tab, will display a list of all 'Models'. You can test individual models or expand the model, by clicking the down arrow, and test the individual nodes.

![](<../../../.gitbook/assets/image (277) (1).png>)

## Selecting How to Test

Different test functions are available for RGB, non RGB lights. You can also select the options to execute different test cycles. You can also select and change background as well as highlight colors and control the speed of the function using the controls provided.

The 'Standard' Tab will test the individual channels. This is intended for AC lights. The 'Highlight Intensity' is the "High" channel value, while the 'Background Intensity' is the "Low" intensity. At value off 255 is 100% ON while 0 is OFF. By default, the Highlight Intensity is 255 and the Background Intensity is 0. 'Case' will set one channel at a time to the 'Highlight Intensity' and proceed thought all the enabled channels. 'Alternate' will set every-other channel to the 'Highlight' and 'Background' Intensity. 'Background Only' with set all the channels to the 'Background Intensity'.

![](<../../../.gitbook/assets/image (656).png>)

The 'RGB' Tab will test the individual Pixel or Dumb RGB strands. Similarly to above, the 'Highlight Intensity' is the "High" channel value, while the 'Background Intensity' is the "Low" intensity. At value off 255 is 100% ON while 0 is OFF. By default, the Highlight Intensity is 255 and the Background Intensity is 0. The three sliders will set the Output Color. For Model with RGB color order, the first sliders would be Red, 2nd is Green and the third is Blue. For all color orders the the first sliders controls the first color, the second sliders the second color, and third sliders the third color. 'Case' will set one Pixel or group of three channels, at a time to the 'Highlight Intensity' and proceed thought all the enabled channels. 'Alternate' will set every-other Pixel or group of three channels to the 'Highlight' and 'Background' Intensity. 'Background Only' with set all the Pixel to the 'Background Intensity'.

![](<../../../.gitbook/assets/image (107).png>)

The 'RGB Cycle' Tab will test the individual colors in a Smart(Pixel) or Dumb RGB strands. The 'A-B-C' option will turn on each individual colors of the selected output. For Model with RGB color order, this would be Red, then Green and then Blue. For all color orders 'A' the first color, 'B's the second color, and 'C' is the third color. The 'A-B-C-All' will cycle the color and add an all colors on state. 'A-B-C-All-None' additionally adds an all colors off state. 'R-G-B-W' with cycle four channel RGBW lights.

![](<../../../.gitbook/assets/image (531).png>)

{% hint style="info" %}
Output from the test tab is, in most cases, always in RGB sequence. It actually turns on every 3rd channel, i.e. 1,4,7,10 etc for red and 2,5,6,11, etc for green, etc and then all channels for white. A quick way to test your lights to ensure the correct RGB, BRG, GRB etc. is set properly, is to turn on channel 1. That should turn on RED. Next would be to turn on channel 2, that should be Green and finally Channel 3 should turn on Blue. Go to the first light of the string . Select the first 3 channels in the setup i.e 97,98, 99. Check that Model is defined as RGB. Use background color and move the first (Red) bar only up. Green turned on for first light. Move first bar down and move the second (Green) bar only up. Blue turned on for first light. Move second bar down and move the third (Blue) bar only up. Red turned on for first light. So the controller should be set to GBR.
{% endhint %}

If you wish that the ‘RGB definition’ of your model be used instead, then select the R-G-B-W option instead.

![](<../../../.gitbook/assets/image (502).png>)

This will use the model definition and turn on the color that corresponds to the channel as defined in the model. So if the model definition is GBR, then the colors turned on will be Green, Blue, and Red respectively.
