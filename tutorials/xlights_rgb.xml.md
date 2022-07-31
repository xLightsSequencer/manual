# Editing xLights\_rgb.xml

## Editing the xlights\_rgb.xml File

{% hint style="warning" %}
This is **very dangerous** proceed at your own risk.
{% endhint %}

Most of the configuration data is stored in an xml file ‘xLights\_rgbeffcts.xml’ in your show directory. Occasionally, a corruption of a component of the file may occur and you will be asked to edit this file. This section describes the contents of this file and how to safely edit it . Before you edit the file, backup the file (F10 from when in xLights will back up this and other xml files from your show directory).

### Using Notepad++

One of the most useful free utilities is Notepad++. Download and install the latest version of Notepad ++ if you do not already have it installed.  The following description has been based on Notepad++ version 6.9 running on Windows. Depending on your version, the screen and options may be slightly different.  Once installed, install/activate the XML Tools Plugin.

![](https://lh4.googleusercontent.com/bUjDAveOwSlRuklQB6Eed\_W8V8LLQNY1mcmoW93v8sGk6t5ZukmByzTS3BxIxvdFunmIFeIfICFdSgtnnJGluyZpcDEWFh5wBAztTMO6TegXqNuSN-zEtLQ4pEt6i9hxGXYiuCqS)

### The rgb.xml Effects File

Navigate to your show directory (or where you have the file that is to be edited) and open the ‘xlights\_rgbeffects.xml ‘ file.

![](https://lh6.googleusercontent.com/n3K\_Qd3UotfEzzOXPN3CboY3xfccJZC3myWxQ3HEyp7QJMFfIxJZfWvxXfRHhA70ZMMbJirEnIkR\_KnXKLxaNpbBM7NL9WJO-Qbv2nGKpWVJkfcPveFlBFhxNsc8EwGO2Gn3EG5Y)

When open and compressed, the xml structure is similar to the following:

![](https://lh6.googleusercontent.com/T673NdsyjtaXURCfnYLf90sO5RWtw3NINy8ziuYYAkQrH7\_vG\_yKExWA6mS0LcnblG5saarZwk2kyuetLHCB5bQijcLwfEi-mPgUgbtG-hiKiIOWMTNR9eRqbK8zk\_uxwEQECWmG)

The xml file contains the definitions of your Models, Effects, Palettes, Views, Model Groups, Perspectives, Settings etc.  Click on the ‘+’ sign to expand that section. In the following image, the View section has been expanded.

![](https://lh3.googleusercontent.com/0lUNt5E\_LyIa2GM\_cqitbAHjajI1x27pou0fExaimk\_N3KVVuOhcc1M5-PhVAcKR3vrxGrqNdOMcRWX2pYfcCX8frwsNpUuyLDISHAVBGnrWAJzWZcoTZRJlEBGz8\_PhrxhJBpk7)

In the following image, the Settings section has been expanded.

![](https://lh6.googleusercontent.com/DQaya4zt7iKO2dlEAixJJkr57JsiQ9K\_CE\_NXkF51itU\_Xo3joQS2FFVGSUaiQu3si3\_f2rdO8nBj3ctPR4gnb6X4HL4Q\_O13g9r01L6x\_8eHNpzNAupylsyfKkChwYcioK4Tw0x)

In the following image, the Models section has been expanded.

![](https://lh6.googleusercontent.com/b02GjDfl86Yxwc0Nnqj-DJDxiHIOQoX4KKJ6IRJ2ju-aQXVRl1XO3bpfPel96N3McnVe2wIItZL9Bxb3T5xvOY8Qc-HzeAPhACJrHSujQuS1kh-V6IfkMa5Aym4FQ7f2e2qcMddI)

In the following image, the Models Groups section has been expanded.

![](https://lh6.googleusercontent.com/CEwIadxhfQqzihW\_dBypV7ee2\_\_SuyGLP9hnPliQpq3\_NnR568k0DJD\_cH28BfoQpiQnp8hIpoLypjfblgfG4BbDu8JhZmGvnbBWG4EeoJAyMSfcwEncIJGQOjVn\_Q7jDifZl4FJ)

Each xml section is made up of a pair of matching tags. When you highlight a tag , notepad will highlight the end tag pair. This could be on the same line or after a few lines.

![](https://lh4.googleusercontent.com/x0Y1fTFHF3c1BV6gf17roGGpAzgB6aQzSu2LXjGfjfwrd5DHRRt7rVMbfL1mfj2Goyiz\_m6WUqRu2W0h\_oHXldumEXarE-lCfJ7xBv78ksTfMoXQO1QkMCT\_q\_JSL4wqKrybTDPp)

Ctrl Alt Shift B and Ctrl Alt Shift A will indent and expand the individual attributes.

{% hint style="info" %}
If you have been requested to delete a section, highlight the beginning and end tags and press delete.
{% endhint %}

When complete, click on the ‘Validate now’ to ensure that the xml is complete and well formed.

![](https://lh3.googleusercontent.com/aps\_lWiJXBsiGZXMoC3tXh-dJnfsypGUVuRxl8icXpBddE8yau-ldjLN9ZGBz82izKKdWb0Csd86tu-tFKbVzHm-EIw8LOEZA-uuUM-Eas1auqG4yvprK8epyc\_EsGRm1JtOJBjQ)

Click on Save to save the file and press ok.
