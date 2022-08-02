# Value Curves

## Value Curves

The Value Curves functionality effectively changes the way an “effect” or setting works over time in a nonlinear fashion, based on the type of Value Curve selected and other parameters off the curve. This is best explained via an example.

![](<../../.gitbook/assets/image (72) (2).png>)

Consider the Bars effect. It has two attributes ‘Palette Rep’ and ‘Cycles’ that can be linearly adjusted using the sliders. They are currently set to 5 and 3 respectively. This means that the palette will repeat 5 times over the duration of the effect and the effect will cycle through three times. Both will be applied evenly across the duration.

However, if you click on the Value Curve icon for either of these attributes, you will be presented with options to change how these repetitions are applied.

![Value Curve Dialog](<../../.gitbook/assets/image (719).png>)

The Flat option is the same as the default linear option. The level can be used to adjust the intensity.

The other sliders are labelled ‘N/A’ as they are not applicable to the context and type of Value Curve thats is being used.

In other scenarios, Value Curves and for other effects, different sliders are available.

Click on the drop down link and a number of options are presented.

![Value Curve Types](<../../.gitbook/assets/image (279).png>)

Select the Ramp Value curve. As the image indicates, this will cause the selected attribute (say Palette Reps), to increase (ramp up) over time, starting from 20% and ending at 80%. Note that the Start level and End level sliders are now active.

![](<../../.gitbook/assets/image (203).png>)

Another type of Value Curve is the Sawtooth variation. The selected attribute to which this is being applied (palette reps) will increase and decrease twice (controlled by the Cycles selected) from a start level to and End level.

![](<../../.gitbook/assets/image (748).png>)

Custom Value Curves can also be created. Select the Custom option from the drop-down. You can then click on the waveform to add new points and drag them as necessary.

### Load and Export

Value curves can be loaded and exported as a .XVC file. By default, the files will be loaded and previewed if they are in the 'valuecurves' folder automatically created in the current show folder.

![](<../../.gitbook/assets/image (250) (1).png>)

![](<../../.gitbook/assets/image (808).png>)
