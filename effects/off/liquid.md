# Liquid

## Liquid

![Icon](<../../.gitbook/assets/image (4) (1) (1).png>)

![Sequencer Grid](<../../.gitbook/assets/image (1092).png>)

![](<../../.gitbook/assets/image (238).png>)

The Liquid effect is based on a liquid particle simulation algorithm. Up to four liquid particle sources can be enabled. Based on Google's LiquidFun fluid simulation. [http://google.github.io/liquidfun/](http://google.github.io/liquidfun/)

The simulation is frame-rate independent, so a sequence rendered at a different frame rate produces visually the same result. Particle flow is measured in particles per second rather than per frame.

| Option/Settings                                                                  | Description                                                                               |
| -------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| <p><strong>Top, Bottom,</strong></p><p><strong>Left, Right Barriers</strong></p> | Prevent Liquid particles from leaving the Checked Values side of the effect.              |
| **Hold Particle Colors**                                                         | Keep each particle color constant over time.                                              |
| **Mix Colors**                                                                   | Change particle color over time.                                                          |
| **Type**                                                                         | Select the liquid type.                                                                   |
| **Lifetime**                                                                     | Lifetime of a particle before it disappears.                                              |
| **Size**                                                                         | Size of particles.                                                                        |
| **Warm Up Time**                                                                 | Throw away start up time (in hundredths of a second) so the effect begins from a settled state. Replaces the older Warm Up Frames setting; existing sequences are migrated automatically. |
| **Despeckle Threshold**                                                          | Spacing of the particles.                                                                 |
| **Gravity**                                                                      | Pull Factor away from the liquid source.                                                  |
| **Enabled**                                                                      | Enables or disables an individual particle source. The first particle source is enabled by default. |
| **X**                                                                            | X location of the liquid source.                                                          |
| **Y**                                                                            | Y location of the liquid source.                                                          |
| **Direction**                                                                    | Rotation of the liquid source.                                                            |
| **Velocity**                                                                     | Rate of movement of the particles.                                                        |
| **Flow**                                                                         | Number of particles dispensed per second. The slider is non-linear, giving finer control at low values and a much higher particle rate at the top of the range. |
| **Source Size**                                                                  | Size of the liquid source that particles will appear from.                                |
