# Sketch

<!-- TODO: screenshot -->

The Sketch effect lets you trace out a path (a "sketch") and have it progressively drawn onto your model over the duration of the effect. You define the sketch in the **Effect Assist** panel, optionally tracing over a background reference image, and the effect then renders that path being drawn on. Each separate path in the sketch is drawn in the next color from the selected palette.

You can either have the sketch draw in over a set percentage of the effect (with the fully drawn sketch held for the remainder), or enable **Motion** so the path is continuously drawn and erased to create simple "motion graphics" style elements.

<!-- TODO: screenshot -->

The actual path is created and edited in the Effect Assist panel rather than on the main effect settings panel. There you trace the sketch, optionally loading a background image to trace over, and the resulting definition is shown back on the effect panel.

| **Options/Setting** | **Description** |
| --- | --- |
| **Sketch** | Read-only display of the active sketch definition string. The sketch itself is drawn and edited in the Effect Assist panel; this field just shows the resulting definition. |
| **Background** | An image used as a tracing reference inside the Effect Assist panel. The image is not rendered into the effect output — it is only there to help you trace the sketch. |
| **Opacity** | Opacity (0-255) of the background tracing image as shown inside the Effect Assist panel. Has no effect on rendering; it only controls how prominent the reference image is while you sketch. |
| **Draw Percentage** | Percentage of the effect duration over which the sketch progressively draws on. The remaining duration shows the fully drawn sketch. Disabled when Motion is enabled. Can be adjusted via the Value Curves option. |
| **Thickness** | Line thickness, in pixels, used when drawing the sketch. Can be adjusted via the Value Curves option. |
| **Motion** | When enabled, the sketch is drawn over the entire effect duration but only a percentage of it is rendered at any given moment, creating simple motion-graphics-like effects. Enabling Motion disables Draw Percentage. |
| **Motion Percentage** | When Motion is enabled, the percentage of the sketch to render at any given time. Only used when Motion is enabled. Can be adjusted via the Value Curves option. |

{% hint style="info" %}
The sketch path is traced and edited in the **Effect Assist** panel. Load a background image there to trace over a reference picture; the background image and its opacity only affect what you see while sketching and are never rendered into the effect output.
{% endhint %}
