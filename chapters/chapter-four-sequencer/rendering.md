# Rendering



### Render Buffer

The Render Buffer is used to generated Effects data onto. For each Model/Group/Submodel, xLights creates a Rectangular Grid to render effects on to. The size of the buffer depends on the model type and settings. 16 strand by 40 pixels Mega Tree will have a 16x40 render buffer.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

The Effect is overlaid onto the render buffer to calculate the color data of the individual pixels or lights.

<figure><img src="../../.gitbook/assets/render1.gif" alt=""><figcaption><p>Matix Render Buffer</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/render.gif" alt=""><figcaption><p>Custom Model Render Buffer</p></figcaption></figure>



### Group Render Buffer

Default Minimal Grid will Draws a 2D grip over the models in the group and attempt to put each pixel in its own box, Up to the Max Grid Size, Normally 400x400.

<figure><img src="https://lh7-rt.googleusercontent.com/slidesz/AGV_vUczyTTS52yvM3s0r22roSTXII8KMXFtsIisgK6_JOQvKRAhHiX905wvuGvDP8yBO5Lum-UbjLGl9rzaET-bOR1fW4sGRMmO_x0cFR49xjeBamL-GypUP5QjdRH3qVWEzC578qELX3UeRoeT9cf04FIf8Hrtsg=s2048?key=1gBjmeJmolgwdkZH-qLraA" alt=""><figcaption></figcaption></figure>



### Model Rendering Low Level Model

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/xLights Rendering.pptx.png" alt=""><figcaption><p>Credit: Keith Westley</p></figcaption></figure>

</div>
