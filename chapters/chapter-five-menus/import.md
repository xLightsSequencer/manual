# Import

## Import

![](https://lh4.googleusercontent.com/mz1p3hcPqQzqsND1uZfsrQWudnTZ8rOs3r8gNpNuFQmUFPc6YKTIXauBf\_QwHlpBMDfwmOXhQrQiEVrEC7nS4jiuIAKBSRekkhJ6WEa\_lQ\_AGfSvKndsPYUBCaiX4HiRySDd9u\_d)

### Import Effects

The import effects dialog allows the user to import effects from other sequences in the currently open sequence. This option should be used when importing purchased sequences from different vendors.

![](<../../.gitbook/assets/image (747).png>)

The Import Effect dialog supports multiple sequence file formats. xLights, Light-o-rama S4, S5, SuperStar, Vixen 2, Vixen 3(limited), HLS, LSP, VSA File formats are all supported.

![](<../../.gitbook/assets/image (370).png>)

### Importing an xLights Sequence

The following example describes how to use this function to import an effects from an xLights XSQ/XML sequence.

* First ensure that you have created or opened an existing sequence that has the models added to the sequencer that you wish to import to.  Note you must select a View first. If there are no models or groups displayed on the Sequencer, then you won’t be presented with any models to import to.

This process can be used to

* Import effects from a xLights sequence from another user
* Import effects from another of your (e.g. older) xLights sequence into an existing xLights sequence

Step 1

Create a new directory and unzip the sequence files to that directory. It is recommended to create this directory within your show folder. The zip file should contain the xlights\_rgbeffects.xml, the sequence.xsq or sequence.xml and any other required files(image, shader, etc files). Change the show folder in xLights to point to the new directory. Copy the music file to the new folder if missing.

![](<../../.gitbook/assets/image (206) (1).png>)

Open the sequence, click on Render All and Save the sequence. You should be able to see how the lights flow in the layout window. Study the sequence and determine which models you wish to copy to your own models.

![](<../../.gitbook/assets/image (409) (1).png>)

{% hint style="success" %}
Print out the model names from the shared sequence as you will need to know those when you import.
{% endhint %}

Look for the correct quantity of elements in the donor sequence that will match your elements. For example If you have 4 windows but the donor sequence has 8, pick the 4 windows that you want to copy.

Make a note of the names of each donor model you want to copy to a model of your own layout. Watch the sequence several times.

Step 2

Make sure you have the appropriate music file in your own media show directory. Close the sequence you were watching, go to the controller tab and change the show folder back to your own directories.

If importing into a new sequence, then

* Create a new musical sequence, select timings and add your display elements or select a view.
* Save the sequence.

Else

* Open the sequence you want to import into,  add your display elements or select a view.

{% hint style="success" %}
Ensure that your models are in your sequencer view before you start the import , else you won’t have any models to import into.
{% endhint %}

Select Import, Import Effects

![](https://lh5.googleusercontent.com/PAlQ\_M7fJADeDZNTGdzSYxNmp53MGXyZLV5f9CqKUIui\_N3RtE5sKS7f1L6Wf8AighmPgoG3WBjXw9AL7vjtDEz5UkhVEqfz8C91j-sSFwf\_3cJxVmG9XH6uR67o49lcclUUJWjI)

Select the file type of XML by changed the dropdown at the bottom right. Select the donor sequence xLights XML.

![](https://lh3.googleusercontent.com/BCgV\_tWskJEVIjxHuRE37WThmi\_KGKaOM9cjm8tMMS8s457-1ZWJu8TCBzbtPgxCNeS6B9WBM\_IfyUk0-lCNEybYAfGYOOe9ISeVG1wAtJC3eRk2jXWaB8Vow75TkngFdTB8YWCd)

A model mapping window is displayed. On the top left is a list containing the timing tracks to import. On the left are the models and model groups from YOUR layout/sequencer tab("Model"). 'Blue' items are Model Groups. On the right is a list of models/groups/submodels ("Available") that contain effects from the sequence being imported. Click and drag a model name from the right list to the ‘Map To’ column in the row that you want to import the model to. You may also highlight the "Map To" cell and double click on a "Available" model to map it or highlight a "Available" model and double click the "Map To" cell.

![Import Dialog](<../../.gitbook/assets/image (143).png>)

Models in the "Available" list will turn gray when used. These items can still be used multiple times even when grayed out.

![](<../../.gitbook/assets/image (5) (1).png>)

When done, select "Save Mapping", and save the XMAP file. This XMAP file can then be loaded in the future when mapping another sequence from the same layout.

![](<../../.gitbook/assets/image (453) (1).png>)

Click OK when done.

### Importing a SuperStar Sequence

Change the File Type drop-down to SUP. Then select the SuperStar Sequence File.

![File Select Dialog](<../../.gitbook/assets/image (358).png>)

The SuperStar Import Dialog will then appear. Select the xlights model to import the SuperStar file onto.

![](<../../.gitbook/assets/image (527).png>)

xLights will create pictures from the SuperStar files. The next dialog asks the user to select a folder to save these pictures files too. In the file name field set the 'base' file name. This 'base' name is used as the file name root of all the saved image files. In most cases just set the 'base' name to the SUP file name.

![](<../../.gitbook/assets/image (134).png>)

The SUP file will then be imported to the specified model as picture and morph effects.

![](<../../.gitbook/assets/image (287).png>)

### Importing a LOR Sequence

Importing a LOR sequence follows the same steps as described above. However, depending on the LOR hardware setup, channel definitions in LOR and correspondingly in xLights need to align. See discussion within Tutorials Section, Coming Over from LOR.

{% content-ref url="../../tutorials/coming-from-lor.md" %}
[coming-from-lor.md](../../tutorials/coming-from-lor.md)
{% endcontent-ref %}
