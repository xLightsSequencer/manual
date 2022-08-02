# Output

## Output

![](<../../../../.gitbook/assets/image (111) (1).png>)

### Use Frame Sync

To use ArtNET or E1.31 frame synchronization then you need to enable it using this option. When enabled xLights will emit at the end of the frame a sync packet which supported controllers will use to trigger light output. This can make your show look a lot sharper but very few controllers support these packets.

For ArtNET you just need to select this option.

For E1.31 you also need to set a universe number on the controller tab … this universe number needs to be a universe you are not otherwise using.

![](<../../../../.gitbook/assets/image (113).png>)

### Force Local IP

By default xLights automatically selects which network interface to send out network data on and sometimes it selects the wrong one. To force xLights to send to a particular adapter select this option and select the IP Address of the adapter you want to use. Select the top blank line to disable forced IP mode and return to the default option of auto.

![](<../../../../.gitbook/assets/image (2) (1).png>)

### Duplicate Frames To Suppress

![](<../../../../.gitbook/assets/image (685).png>)

This selection allows xLights to "skip" frames that contain the same data as the previous frame. This can help with lagging, as it will reduce network traffic. xSchedule will also use this setting when outputting data.

### xFade/xSchedule

![](<../../../../.gitbook/assets/image (381) (1).png>)

When using the Jukebox Panel with xFade or xSchedule, this determines which instance of xLight to select the effect from.
