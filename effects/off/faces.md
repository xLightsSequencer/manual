# Faces

![Icon](<../../.gitbook/assets/image (652).png>)

![Sequencer Grid](<../../.gitbook/assets/image (30) (1).png>)

![](<../../.gitbook/assets/image (210).png>)

The Faces effect is used by xLights to generate singing and talking face effects. It is used and placed on the sequencer as part of the Papagayo import functionality, if the target in xLights is a Coro face.

It is also used within xLights functionality to generate Singing Faces. The use of this effect is described in the section describing Singing Faces.

| **Option/Settings**           | Description                                                                                                                              |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **Phoneme**                   | Sets Face to specific mouth position.                                                                                                    |
| **Timing Track**              | Sets Timing Track to use for Lyrics/Phonemes                                                                                             |
| **Face Definition**           | Sets Face Definition to use. These are setup in the model preference under the 'Faces' option.                                           |
| **Eyes**                      | Sets if the Eyes are 'Open', 'Close', 'Automatic', or '(off)'.  'Automatic' blinks the eye based on frequency. '(off)' disables the eye. |
| **Eye Blink Frequency**       | Set the speed of Automatic Eye Blinking                                                                                                  |
| **Show Outline**              | Show outline if defined in the Face Definition.                                                                                          |
| **Suppress Shimmer**          | Skip '-shimmer' tags in Timing Tracks lyrics.                                                                                            |
| **Use State as outline**      | Use a State Definition for 'coloring' the Outline                                                                                        |
| **Suppress when not singing** | If set, the Face will disappear if not lyrics are present, in the timing track.                                                          |
| **Lead In/Out Frames**        | Number of frames the face will appear before the lyrics start/end, Only available if 'Suppress when not singing' is enabled.             |
| **Fade during lead in/out**   | Fade the face in and out during the Lead in/out frames, Only available if 'Suppress when not singing' is enabled.                        |
| **Transparent Black**         | Sets the black pixels transparent to show effects on lower layers.                                                                       |

### Color Pallet

The color pallet is used to determine the color of the signing face. If force custom colors is enabled in the model's face definition, the custom colors takes precedence and the color pallet will not change the effects color.

![](<../../.gitbook/assets/image (138).png>)

![](<../../.gitbook/assets/image (408).png>)

| Pallet Color     | Face Nodes              |
| ---------------- | ----------------------- |
| 1st Pallet Color | Mouth Nodes             |
| 2nd Pallet Color | Eyes Open/Close Nodes   |
| 3rd Pallet Color | Outline Nodes           |
| 4th Pallet Color | Outline2 Nodes          |
| 5th Pallet Color | Eyes Open2/Close2 Nodes |
| 6th Pallet Color | Eyes Open3/Close3 Nodes |

{% content-ref url="../../chapters/chapter-four-sequencer/singing-faces/" %}
[singing-faces](../../chapters/chapter-four-sequencer/singing-faces/)
{% endcontent-ref %}
