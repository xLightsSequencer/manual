# State

![Icon](<../../.gitbook/assets/image (162) (1).png>)

![Sequencer Grid](<../../.gitbook/assets/image (387).png>)

![](<../../.gitbook/assets/image (296).png>)

The State effect is similar to the Faces effect, but enables you to have similar functionality for props that are not standard ‘Faces’ - such as Reindeer Coro faces, a seven segment FM ‘Tune to sign’ with a colon and a dot etc (image examples as below):

![](https://lh5.googleusercontent.com/U-Ie7jC51WfFpfXYA-NYtRucXmtFljR2tD1\_Zs9ymmCHFZYAPB8eRFQwdGOHaVnuII3MhF0anx-zHy-MqHIYQh9uiu1gLHWSi1uoj4YBZave4guki11xXun2mfJIt\_mWzJ\_guwpC)

![](https://lh3.googleusercontent.com/NHO431ihnNuDru\_U1Twlv710RaMCJy\_oKwH8cgNKacYud-nmTUJFr1ruWvI048RN2rI4UuYovNhYTlhiLdJTcyOxzleYpPxosEwahAg\_rmG4NIiLnUXZeFgLza7Bm9XRj7IwfR78)

![](https://lh4.googleusercontent.com/mbETnd-OtgIJO-Ku-1oPlaISeU52yjIp4XMNpx7-CRfjec6yuqrNRDedpCC2MqQOLhgHQ4-92b3cj-YHJ3qJumyGKP2K5EeddPg1NfJbdm6i2vXiyu3QY6fteLJplWfNPjhQqBbF)

This effect is somewhat similar to the Faces effects i.e uses many of the same concepts.

However there are a number of differences and therefore this effect can be used when there are a number of ‘non standard’ elements that you wish to control. You can define upto 40 different combinations of channels to turn on and off (each combination via a state setting).

There are pre defined state values to support numbers and color options to cycle through or allocate specific colors to specific number digits.

## Definition

Create a new Custom Model via the layout tab, named ‘Bruno’ (representing the reindeer image) for this example . Similar to other custom models, create or import the channel setup.

![](https://lh5.googleusercontent.com/AA3G2U65ZcWksfNfoi0D\_1qzM9czlAp1SnFE58vUZ7rqMyQ9N\_aua8IMRKhtr8zEi8X5ZUQe\_f1NByymNYxkQS9UzBFUW6028UJY69mdTF7LUPb-OccEnE8e1Kkc5vRzMkgDHaXN)

In a second example in this section , a custom model named ‘TuneTo’ has been created (representing the numbers in the Tune To image).

Then click on the State Property, to open up the State definition window.

![](https://lh6.googleusercontent.com/IzliaKYCvu9bVkuZHmg9Q8UPIk0w3TWamSRF3EIU\_FBOl9-DyPvnQTlsNfAwolxI9c6EhSEcuxIcec-dnSpWlHGOnB-gt7pAsB\_OndrEoaXyzpeNxAt1CBqL0gw2bqheE88Apm37)

Click on Add and specify a Name for the State (‘State1’ in this example). From the drop down box , select either Single Range or Node ranges.

You can specify upto 40 different combinations of states along with the channels to be turned on for each state. In the example , ‘wink’ will turn on channels 1,5 and 8 and ‘blink’ will turn on channels 1,2,5,and 8. For this type of effect, any words can be used - just ensure that the same words are used on the timing track and the matching nodes will be turned on.

To can define additional or different combinations by creating a new state definition (say State2) and having another set of upto 40 States defined.

The colors to be turned on, by default are sourced from the model properties, but you can force a specific color to be turned on by selecting the ‘Force Customs Colors’ option which then provides a column to specify the color.

Clicking in a cell in the Color column displays the color palette to pick a color.

Similar to other custom models, create or import the channel setup via the Mode Data attribute of the Model definition.

![](https://lh5.googleusercontent.com/XdycEnE7cuLlTD9t-yb1dL-JEpA-DnOYRp\_kc3Zzf1h65srvZn1kuEZ9Q58UMeTPecBHPsV6HksCgIBVBwDq065hZSxLoAi61\_3bAbz5SSkXhB8QFly9OCzAUJQvVe2fytHdI8vr)

![](https://lh5.googleusercontent.com/rqwjnTFONeOLv56DYWArSl3sF0sC4bEaT\_0JZ\_-WpVzxc3O9ub7OOFsMojvGAjpSyuh9hemHCU2EmDqicN\_WO5rLewdffMQX1qp3ATqTDSSnFo52HFhUr8rwYw4JkAtPPqv8cmOh)

On the sequencer tab, drop the State effect against the Custom model (Bruno in this example).

Edit the timing track and enter the labels to match the state definitions. In this example, select the timing track ‘New Timing’ , create two timing bars (press lower case ‘t’ with the cursor in the waveform area), then double click on the white horizontal line between the two timing marks and enter the label text (eyesleft, eyesright etc) in the pop up window. Ensure that the text exactly matches one of the states defined.

In the Effects setting window, select ‘State1’ as the state definition, enable and select the Timing Track ‘New Timing’ as the source and select ‘Iterate’ as the Mode.

![](https://lh5.googleusercontent.com/qsjwecNo68H2eneRn6K5XbFxPxYvIykEufN8gNurPQlwkxx6gASPFon8KtT2znELdR5t7swztG2rwK7mtl8QW6D0Fmw6ixZNlWZPy6gwd5GbR7fyP0kPkDCjWkLrME6eKi03IhbE)

Similar to the way phonemes work on the Faces effect , this will cause the states ‘eyesleft’, ‘eyesright’ and ‘wink’ to be activated. Iterate causes it to loop around equally for the timespan duration selected for the effect.

You can create multiple Timing tracks and add labels to each track matching the defined states if required. You can also select a specific State to turn on instead of using the Timing track by checking the State attribute and selecting the State value (wink or another from the drop down list).

If you select ‘Default’ as the mode, then the selected states will be activated once (with equal duration).

The Color attribute has the following options:

* Graduate will start from the first color selected and then transition to the next color.
* Cycle will change color  at the end of each timing mark.
* Allocate will allocate a color to each state (‘eyesleft’, ‘eyesright’, ‘wink’) and turn that color on when that state is activated. The allocation depends on how many colors you have selected and how many states are defined.

Number is used (for number states) , to turn the matching number on to that color.

![](https://lh5.googleusercontent.com/uOyW-X6U2yfeKjRY5G32ocM553SuI-quN8m39GuRYSPc0oVP-4h7KivccwVAeSdF1XpLtvLeiVeioiQpolny4H6iZ\_tc5GRGRs537cSeNM67s8-iERiExNq-i68CY1yiAVVh1cKL)

In the example of a 7 segment display below, each number has been created as a state and nodes assigned to it.

The ‘Countdown’ mode is used to Countdown from a specific number to zero. Specify the starting number in the label (if 123 was used in the example just above in this mode , then it would count down from 123 to zero).

The ‘Time Countdown’ mode is used to Countdown in seconds from a specific time until the effect duration runs out. Specify the starting time in the label (if 1.30 was used in the example just above in this mode , then it would count down from 1 minute 30 seconds).

In the 4 digit example, States 1 through 0 control the right most digit, States 00 to 90 control the second last digit from the right, 100 to 900 control the 3rd digit from the right and 1000 to 9000 control the first digit.

![](https://lh4.googleusercontent.com/gtH\_MWUKLE0NppAo7ho2ipgTS7DJhebMvMQh2BdSlW7vha\_y1TqABf2Uir\_J11f3jhdIXFCdiU-UDH\_Zqwdb6qiN9gsJrGL5\_SqW5BchIOGp6Del0LkhxEufPYNaqPmgHwEJdFFM)

In the default mode, if you wish to turn on the number ‘123’, then you would specify ‘100,20,3’ (without quotes) in the label on the timing grid.

‘Colon’ and ‘Dot’ represent the colon and dot respectively.

These state names are predefined to work for a seven segment display. The nodes however can be assigned to each State/ Number as required.
