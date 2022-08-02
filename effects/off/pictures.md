# Pictures

![Icon](<../../.gitbook/assets/image (783).png>)

![Sequencer Grid](<../../.gitbook/assets/image (684).png>)

{% tabs %}
{% tab title="Start Position" %}
![](<../../.gitbook/assets/image (427).png>)
{% endtab %}

{% tab title="End Position" %}
![](<../../.gitbook/assets/image (322).png>)
{% endtab %}

{% tab title="Start Scale" %}
![](<../../.gitbook/assets/image (777).png>)
{% endtab %}

{% tab title="End Scale" %}
![](<../../.gitbook/assets/image (167) (1).png>)
{% endtab %}
{% endtabs %}

The Pictures effect is used to import a supported image type (gif, bmp, jpg etc) and render that image as an effect while also allowing the image to be manipulated and edited within xLights. You will need a image that is to be imported. Save the image as a GIF file and make the background color transparent if you don’t want the original (white) background of the image.

Place the Picture effect in on timing cells that you wish to have the effect on a model. Click on the effect on the grid and amend the parameters as required. First click on the Browse button and navigate to the location of your image, select the image and click open or double click to select the image.

| Option/Settings | Description |
| --------------- | ----------- |

| **Movement** | <p>Controls how the image will move across the model layout.</p><p>In addition to directional options such as left, right, wiggle etc, there are a number of special options, such as peekaboo, flag wave.</p> |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

| **Movement Speed** | Controls how fast the image moves across within the effect timeframe. |
| ------------------ | --------------------------------------------------------------------- |

| **Frame Rate Adj** | When using the pictures effect to play an GIF, this setting is used to set the playback speed if needed to speed up or slow down the playback. |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |

| **Offset in Pixels** | Used to specify exact number of pixels rather than % for the start and end positions offset. |
| -------------------- | -------------------------------------------------------------------------------------------- |

|   | <p>"No Scaling" Image file will not be resize and excess pixels will be chopped off.</p><p>"Scale to Fit" Image file will be resize to your model. Vertical and horizontal dimension will be scaled independently.</p><p>"Scale Keep Aspect Ratio" Image file will be resize to your model but the dimension are scaled together to keep the original aspect ratio.</p> |
| - | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

| **Shimmer** | Fade in and out random pixels in the image. |
| ----------- | ------------------------------------------- |

| **Loop Animated GIF** | Replay GIF animation, if GIF is shorter than effect length. |
| --------------------- | ----------------------------------------------------------- |

| **Suppress GIF Background** | Remove GIF background color and make it transparent. |
| --------------------------- | ---------------------------------------------------- |

| **Transparent Black** | Allow black pixel to be transparent. Slider adjust at what level "black" becomes transparent. |
| --------------------- | --------------------------------------------------------------------------------------------- |

| **Start Position: (x,y)** | Sets the position of the image if it does not need to be centered on the model. |
| ------------------------- | ------------------------------------------------------------------------------- |

| **Start Position: (wrap x)** | Used to bound the picture image within the model. Defines and controls the coordinates of the ‘bottom left’ start corner. |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------- |

| **End Position: (x,y)** | Used to bound the picture image within the model. Defines and controls the coordinates of the ‘top right’ end corner. |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------- |

| **Start Scale** | Set the starting position scale (0 - 1000%) independently of the start position. |
| --------------- | -------------------------------------------------------------------------------- |

| **End Scale** | Set the ending position scale (0 - 1000%) independently of the end position. |
| ------------- | ---------------------------------------------------------------------------- |

{% hint style="success" %}
The playback rate is influenced by the length of the effect. So if you change the time length of your effect and have an image that is non stationary, the rate of movement will adjust according to the new time length.
{% endhint %}

{% hint style="danger" %}
If you move the image that you have used for the picture effect to a different location or delete it, when you next run the sequencer, if the image is not found, an error message will not be displayed, but the picture effect will render a blank image. The only time this won’t happen is if only the drive letter has changed, and the rest of the path is the same.
{% endhint %}
