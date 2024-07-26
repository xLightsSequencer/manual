# Rendering



### Render Buffer

The Render Buffer is used to generated Effects data onto. For each Model/Group/Submodel, xLights creates a Rectangular Grid to render effects on to. The size of the buffer depends on the model type and settings. 16 strand by 40 pixels Mega Tree will have a 16x40 render buffer.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

The Effect is overlaid onto the render buffer to calculate the color data of the individual pixels or lights.

<figure><img src="../../.gitbook/assets/render1.gif" alt=""><figcaption><p>Matix Render Buffer</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/render.gif" alt=""><figcaption><p>Custom Model Render Buffer</p></figcaption></figure>



### Model Rendering Low Level Model

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/xLights Rendering.pptx.png" alt=""><figcaption><p>Credit: Keith Westley</p></figcaption></figure>

</div>
