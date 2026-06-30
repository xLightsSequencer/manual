# Arches Model

## Arches Model

The ‘# Arches’ value can be set to the number of arches that the model represents (normally one). Similarly you can set the nodes per arch and lights per node (normally 1). The Arc Degrees determines the portion of a circle's circumference the arches use. 180 degrees mean the arch is half the circumference of a circle and 90 would be one forth circumference of a circle. The Arch Tilt will tilt the arches "hops" left or right. This is useful for arches on a incline.

![](<../../../.gitbook/assets/image (597).png>)

![](<../../../.gitbook/assets/image (813).png>)

The example above will contain two arches of 25 pixels each, for a total of 50 pixels. Each pixel contains 3 LED per pixel so there are 3 lights per node.

### Layered Arch

![](<../../../.gitbook/assets/image (286).png>)

With Layered Arch enabled,  a multi layered arch will be created. The Layers attribute value describe the concentric arches in the model. This will create node count settings for each layer. The sum of the node counts must add up to the number of nodes in the model. 'Hollow %' will set the space "under" the arch.

![](<../../../.gitbook/assets/image (999).png>)

## Model Settings

<!-- TODO: screenshot -->

| **Options/Setting** | **Description** |
| --- | --- |
| **Layered Arches** | When enabled, builds a multi-layered (concentric) arch instead of a single arch. Toggling this switches the property set between the single-arch and layered-arch options below. |
| **# Arches** | Number of separate arches the model represents (single-arch mode). Range 1-100, normally 1. |
| **Nodes Per Arch** | Number of nodes along each arch. Range 1-1000 in single-arch mode (1-10000 as **Nodes** in layered mode). |
| **Nodes** | (Layered mode) Total number of nodes in the layered arch. Range 1-10000. |
| **Layers** | (Layered mode) Number of concentric arch layers. Each layer gets its own node-count entry, and the layer node counts must sum to the total node count. |
| **Hollow %** | (Layered mode) Sets the empty space "under" the arch as a percentage. Range 0-95. |
| **Zig-Zag Layers** | (Layered mode) When enabled, wiring zig-zags between layers. |
| **Lights Per Node** | Number of individual lights/LEDs per node. Range 1-250, normally 1. |
| **Arc Degrees** | Portion of a circle's circumference the arch spans. 180 = a half circle, 90 = a quarter circle. Range 1-180. |
| **Arch Tilt** | Tilts the arch "hops" left or right, useful for arches on an incline. Range -180 to 180. |
| **Gap Between Arches** | (Single-arch mode) Spacing inserted between each arch. Range 0-500. |
| **Starting Location** | Sets the corner/side where the wiring starts (e.g. Green Square / Blue Square, with inside/outside variants in layered mode). |
