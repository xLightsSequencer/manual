# Servo

![Icon](<../../.gitbook/assets/image (394).png>)

![Sequencer Grid](<../../.gitbook/assets/image (557).png>)

![](<../../.gitbook/assets/image (1019).png>)

The Servo Effect is intended to drive server motors. Select the DMX channel to use and the value. It supports both 8 bit and 16 bit values. 16 bit will use two channels of data.

You set a start and end value for the position; the effect interpolates between them over its duration (each value can be driven by a Value Curve for more complex movement). Alternatively the position can be driven from a timing track for lip-sync style animation.

| **Options/Setting** | **Description** |
| --- | --- |
| **Base Channel** | Selects which channel on the DMX model to control. The channel list is populated from the model's node names. |
| **16 bit** | When enabled, outputs a 16-bit value across two channels (coarse and fine) for higher precision servo positioning. When disabled, uses a single 8-bit channel. Default True. |
| **Use Timing Track** | When enabled, the servo position is driven by phoneme data from a timing track instead of the start/end value sliders, useful for lip-sync animations. Default False. |
| **Timing Track** | Selects which timing track to use for phoneme-driven servo positioning when Use Timing Track is enabled. |
