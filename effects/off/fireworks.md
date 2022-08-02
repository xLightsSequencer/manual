# Fireworks

![Icon](<../../.gitbook/assets/image (142) (1).png>)

![Sequencer Grid](<../../.gitbook/assets/image (625).png>)

![](<../../.gitbook/assets/image (93).png>)

The Fireworks effect creates a fireworks type of effect of exploding lights in a burst. Used most effectively on models such as a mega tree or a matrix.

One or multiple colors can be used for the effect. If multiple colors are selected, then the lights in the explosion will be made up of the selected colors.

| Option/Settings            | Description                                                                                                                                                                                                                                             |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Number of Explosions**   | Defines the number of explosions to be created.                                                                                                                                                                                                         |
| **Particles in Explosion** | Controls the number of particles in the explosion.                                                                                                                                                                                                      |
| **Velocity of Particles**  | Controls the speed of the particles exploding.                                                                                                                                                                                                          |
| **X Velocity**             | Left/Right Movement of the Firework                                                                                                                                                                                                                     |
| **Y Velocity**             | Top/Bottom Movement of the Firework                                                                                                                                                                                                                     |
| **X Location**             | Left/Right Location of the firework within the buffer (0-100%). '-1' indicates random location.                                                                                                                                                         |
| **Y Location**             | Top/Bottom Location of the firework within the buffer (0-100%). '-1' indicates random location.                                                                                                                                                         |
| **Hold Color**             | If "true" keeps the same color for the lifetime of the firework. If "false" colors change throughout the lifetime of the firework.                                                                                                                      |
| **Gravity**                | Sets if the firework particles fall down to the ground.                                                                                                                                                                                                 |
| **Particle Fade**          | Defines the speed at which the particles should fade in the explosion after the initial burst.                                                                                                                                                          |
| **Fire with Music**        | Controls whether the audio signal should be used to control the effect. If not selected then a set number of fireworks are triggered instead.                                                                                                           |
| **Trigger level**          | Controls how high the music level needs to be before the effect will be triggered, if ‘Fire with Music’ is selected. Where the waveform is relatively flat, the fireworks may trigger repeatedly if the waveform does not drop below the trigger level. |
| **Fire with Timing Track** | When selected the effect will trigger a firework at every timing mark in the selected timing track.                                                                                                                                                     |

{% hint style="success" %}
Add multiple layers of fireworks with different colors on each layer to get more explosions with multiple colors at the same time. Set different velocities and number of explosions on each layer.
{% endhint %}
