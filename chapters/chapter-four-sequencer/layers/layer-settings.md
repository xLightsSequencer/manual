# Layer Settings

## Layer Settings

![](<../../../.gitbook/assets/image (936).png>)

The Layer Settings window can be opened by clicking on the Layer Settings icon from the toolbar, or via the View, Windows menu.

![](<../../../.gitbook/assets/image (904).png>)

#### Reset panel when changing effects

![](<../../../.gitbook/assets/image (1105).png>)

This will reset the Layer Setting back to default every time you select or create a new effect. Checked is the recommended setting for most users.

## Buffer

![](<../../../.gitbook/assets/image (1123).png>)

#### Render Style

This attribute controls how the buffer is laid out for a model or model group when the effect is rendered. Every model has a ‘Default’ buffer which can be view by opening the model's node layout in the Layout Tab.

![Arch Model Render Styles ](<../../../.gitbook/assets/image (953).png>)

For example, for Arches – the default buffer treats each arch as a single line and stacks the arches on top of eachother, for a Star model, the default is a square grid that cases effects to chase across the face of a star.

Additional options are available to change the buffer representation for the model or group. The list of values that are selectable are dynamic depending on the type of model.

![](<../../../.gitbook/assets/image (235).png>)

For model groups, additional buffer render styles are available. The list below discrips all model render styles.

| Render Style                | ​Description                                                                                                                             |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Default                     | Uses the Default buffer for a model or SubModel and Per Preview for a Model Group.                                                       |
| Per Preview                 | This will render the way the model has been laid out in the preview.                                                                     |
| Single Line                 | Places all the strings/stands end to end and renders the effect on the resulting one pixel high line.                                    |
| As Pixel                    | Treats all the model nodes as one pixel.                                                                                                 |
| Horizontal Stacked          | Places each Model next to each other horizontally in a single row that is aligned to the bottom                                          |
| Vertically Stacked          | Places each Model on top of each other Vertically in a single column, aligned to the left side.                                          |
| Horizontal Stacked - Scaled | Places each Model next to each other horizontally in a single row, scales  each models buffer size to be the same.                       |
| Vertically Stacked - Scaled | Places each Model on top of each other Vertically in a single column, scales  each models buffer size to be the same.                    |
| Horizontal Per Model        | Each Model's nodes are setup as a single row in the buffer horizontally and then each model is stacked vertically.                       |
| Vertical Per Model          | Each Model's nodes are setup as a single column in the buffer vertically and then each model is place horizontally next to each other.   |
| Horizontal Per Model/Strand | Each Model's strands are setup as a single row in the buffer horizontally and then each model is stacked vertically.                     |
| Vertical Per Model/Strand   | Each Model's strands are setup as a single column in the buffer vertically and then each model is place horizontally next to each other. |
| Overlay -  Centered         | Model are "set" on top of each other and the buffers are Centered                                                                        |
| Overlay - Scaled            | Model are "set' on top of each other and the buffer sizes are scaled to be the same.                                                     |
| Single Line as a Pixel      | Each Model is represented as a single Pixel and placed in a single line.                                                                 |
| Per Model Default           | Render the Effects on Each Individual Model using the model's default buffer                                                             |
| Per Model Per Preview       | Render the Effects on Each Individual Model using Per Preview                                                                            |
| Per Model Single Line       | Render the Effects on Each Individual Model using Single Line                                                                            |

#### Camera

When using the "Per Preview" render style, this dropdown allows the user to select which viewpoint to use. 2D is the default.

![](<../../../.gitbook/assets/image (158).png>)

#### Transformation

The transformation attributes can be used to rotate the effect clockwise, counter clockwise (90 or 180 degrees) or to flip it either horizontally or vertically.

![](<../../../.gitbook/assets/image (461).png>)

{% hint style="info" %}
While some effects have settings to do similar things this is now the standard way to flip or rotate an effect.
{% endhint %}

#### Blur

This attribute will cause the effect to ‘blur’ i.e. the colors become less distinct (hazy) and the edges of two colors will fade into each other i.e. will not have sharp edges. The level of haziness can be increased from 0 onwards using the slider or adjusted using the Value Curve functionality by clicking on the Value Curve icon.

![](<../../../.gitbook/assets/image (1050).png>)

#### Sub Buffer Selection

The Sub Buffer selection can be used to limit the area that an effect is active. This basically redefines the size of the model/group (on a per effect basis). This option is different than masking, because the entire effect is rendered based on this new model size, whereas a mask covers up what you specify.

![](<../../../.gitbook/assets/image (613).png>)

So if you only want the effect to be on the top half of the model or group, bring the bottom part of the dotted yellow line to the middle of the black box. The ‘handles’ of the yellow grid are in the corners. Double Clicking will reset the defaults to the full size.

{% hint style="success" %}
If you right click on the black box you can access and select some of the common buffer settings. ‘Full Buffer’ will reset to the full size. The "Edit" option allows the user to manually input the X/Y locations and use value curves.
{% endhint %}

As an example, drop the Fire effect on a Model Group covering your ‘whole house’.

Then adjust the yellow dotted lines of the box inwards and look at the effect it has on your house preview. You can limit the effect to say the left side of your house, with another similar one of a different color on the right side of the house applied on another layer.

{% hint style="info" %}
The Sub-Buffer area selection also supports Value Curves. The bounding box handles will appear Red when a value curve is in use.
{% endhint %}

#### Persistent

The Persistent option when enabled does not clear the display buffer before rendering each frame. The result is the preview frame remains until overwritten by a subsequent frame. For example, drop the balls or fan effect on a model, select the blending to “Effect 1”, then toggle Persistent on/off. You will see a huge difference. Doing the same for a “Chase” effect also results in a very different look.

![](<../../../.gitbook/assets/image (558).png>)

The term came from high persistence scopes where each trace just kept layering on top of previous traces.

## Roto-Zoom

The Roto-Zoom functionality enables the effect to be Rotated as well as have aspects of the effect Zoomed.

![](<../../../.gitbook/assets/image (993).png>)

The Preset defines the type of rotation to be applied to the effect. The effect can be continuously rotated clockwise or counterclockwise, made to explode outwards , implode inwards , shake etc.

The Rotation attribute changes the orientation of the effect. The attribute cannot be used if a Rotation Preset has been selected.

The Pivot Point attributes work if the Rotation attribute has been used by moving the point at which the effect rotates along the other axes.

The Zoom attribute increases the size of the effect - for a Text effect - the text will be made larger. The Zoom quality increase or decreases the pixels when the zoom attribute is used. These two attributes cannot be used if a Zoom (i.e. explode or implode ) Preset has been selected.

Application Order specifies which order to apply the rotation in.

{% hint style="success" %}
Select the Preset of ‘None - Reset’ to reset the settings before trying another combination or if the rotation / zoom settings appear to be different to what is expected.
{% endhint %}
