# Arches Model

## Arches Model

The ‘# Arches’ value can be set to the number of arches that the model represents (normally one). Similarly you can set the nodes per arch and lights per node (normally 1). The Arc Degrees determines the portion of a circle's circumference the arches use. 180 degrees mean the arch is half the circumference of a circle and 90 would be one forth circumference of a circle. The Arch Tilt will tilt the arches "hops" left or right. This is useful for arches on a incline.

![](<../../../.gitbook/assets/image (507).png>)

![](<../../../.gitbook/assets/image (296).png>)

The example above will contain two arches of 25 pixels each, for a total of 50 pixels. Each pixel contains 3 LED per pixel so there are 3 lights per node.

### Layered Arch

![](<../../../.gitbook/assets/image (588).png>)

With Layered Arch enabled,  a multi layered arch will be created. The Layers attribute value describe the concentric arches in the model. This will create node count settings for each layer. The sum of the node counts must add up to the number of nodes in the model. 'Hollow %' will set the space "under" the arch.

![](<../../../.gitbook/assets/image (416).png>)
