# Shader

![Icon](<../../.gitbook/assets/image (496).png>)

![](<../../.gitbook/assets/image (538).png>)

![](<../../.gitbook/assets/image (428).png>)

The Shader Effects used the computers graphics card to render predefined shader program/algorithm files. This files are commonly used in video games to render graphics. xLights only support a few shader files formats. Known working shader files can be downloaded with the "Download" button. Once a shader file is loaded, additional settings slider could appear related to the shadder. These setting are defined by the shader files itself and change parameters used by the underlying shader program/algorithm. Some shader files require canvas mode to be enabled, hover over the file name and the tooltip will display this information.

| Option/Settings    | Description                                                                  |
| ------------------ | ---------------------------------------------------------------------------- |
| **Shader File**    | Location on Disk of the shader file.                                         |
| **Lead in frames** | Number of Frames to skip before displaying the effect.                       |
| **Time Speed**     | Speed of the Shader. Positive for Forward Time, Negative for Backwards Time. |

{% hint style="warning" %}
If The Shader Effect appears Red, Yellow, or Cyan(Light Blue) on the model, it represents a render issue.

Red: The Shader File cannot be found on disk.

Yellow: The Shader File cannot be compiled. Shadder is a incompatible Shader File format.

Cyan(Light Blue): The computer graphics card does not support OpenGL 3.0 which is required for the shader effect. Verify in xLights the OpenGL setting is set to Auto Detect or OpenGL 3.0. Try upgrading the graphics drivers software and/or graphics card.
{% endhint %}
