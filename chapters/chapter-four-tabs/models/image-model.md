# Image Model

### Image Model

![Image Model](<../../../.gitbook/assets/image (641).png>)

The Image Model is used to represent single channel props like blow-molds, inflatables or incandescent cutouts/wire-frames. You load a picture of the prop and xLights will illuminate the picture based on the channel value. The Off brightness can be set to a value above zero(10% in the example) so it is still visible in the layout when the channel is off. This Model only works with Single Channel or Single Channel Intensity string types not RGB lights or pixels.

![Image Model Settings](<../../../.gitbook/assets/image (552).png>)

When a JPG image includes an orientation (EXIF) tag, xLights honors it so the picture is displayed the right way up automatically, matching how it appears in other photo viewers.

## Model Settings

<!-- TODO: screenshot -->

| **Options/Setting** | **Description** |
| --- | --- |
| **Image** | The picture file used to represent the prop. Supported formats include PNG, BMP, JPG/JPEG, GIF and WebP. |
| **Off Brightness** | Brightness used to display the image when the channel is off, so the prop stays visible in the layout. Range 0&ndash;200; a value above 0 (for example 10%) keeps a dim outline visible when the channel value is zero. |
| **Read White As Alpha** | When enabled, white/grey pixels in the image are treated as transparency (alpha) based on their brightness, letting the background show through instead of appearing as solid white. |
