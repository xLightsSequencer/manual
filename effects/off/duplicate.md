# Duplicate

Copy Effect Data from another model. Each Individual Layer has to be "duplicated" to reproduce all the effects across two models.

<!-- TODO: screenshot -->

| **Options/Setting** | **Description** |
| --- | --- |
| **Model** | The source model, submodel, or strand whose effects will be duplicated onto the current model. |
| **Layer** | The layer number on the source model to duplicate effects from. Layer 1 is the first (bottom) layer. Range 1-1000. Default 1. |
| **Override duplicated Palette** | When enabled, the color palette from this effect is used instead of the palette from the duplicated source effect. Default False. |
| **Override duplicated Color settings** | When enabled, the color settings (sparkles, brightness, etc.) from this effect override those from the duplicated source. Default False. |
| **Override duplicated Layer Blending settings** | When enabled, the layer blending and transition settings from this effect override those from the duplicated source. Default False. |
| **Override duplicated Layer settings** | When enabled, the buffer/layer settings (rotation, zoom, etc.) from this effect override those from the duplicated source. Default False. |
| **Include Submodels** | When enabled, also duplicates effects from matching submodels of the source model onto the corresponding submodels of the current model (matched by name). Default False. |
