# FPP Connect

## FPP Connect

![FPP Connect Dialog](<../../../.gitbook/assets/image (271).png>)

The FPP Connect Dialog is used to upload files to a Falcon Player(FPP) that is being used as a show player, remote player, or in bridge mode. The channel inputs, channel outputs, model configurations and one or more sequences (including associated audio) can be uploaded to one or more FPP instances. FPP Connect only supports FPP 2.0 and newer.

On startup, xLights will attempt to auto-discover all the FPP instances on your network. If none are found, Click the Add FPP button to manually add a device by its IP Address.

![List of FPP Devices](<../../../.gitbook/assets/image (44).png>)

The Upload Checkbox Column will "Enable" the FPP instances for xLights to upload data to it. If unchecked xLights will not upload any data to that device.

![Upload Enable Column](<../../../.gitbook/assets/image (487).png>)

The Location Column will display the DNS host name and IP address. The Description Column DNS Host description value. The Version Column is the FPP software version installed on the device.

![FPP Host Information, IP Address and Version ](<../../../.gitbook/assets/image (792).png>)

The FSEQ Type Column allows the user to select which FSEQ file version to upload to each FPP device. V1 FSEQ files are required for FPP 2.5 and lower. The V2 FSEQ file format is a compressed files format that only works with FPP 2.6 and newer. The V2 FSEQ Sparse file format is the same a V2 but limits the channel range to what is required for that FPP instances output devices. If using FPP 2.6 or newer, it is recommended to use the V2 file format on the Standalone/Master FPP devices and the V2 Sparse file format on FPP remote devices. For FPP 2.5 and lower, V1 file format must be used. xLights will select a default FSEQ version based on the FPP version and if a Pixel Hat/Cap is attached or if a LED matrix is set up. This can be changed by the user if needed.

![FSEQ Version Selector](<../../../.gitbook/assets/image (539).png>)

If the Media checkbox is selected, xLights will upload the Media Files.

![Media Upload Column](<../../../.gitbook/assets/image (583).png>)

If the Model checkbox is selected, xLights will upload the Model Data for the display testing page.

![Model Upload Column](<../../../.gitbook/assets/image (596).png>)

The UDP Out dropdown will enable xLights to upload The E1.31 and DDP Channel Output definitions from the Setup Tab in xLights. 'All' will uploads All the E1.31 and DDP Channel Output Definitions, 'Proxied' will only upload E1.31 and DDP Ouput Channel Definitions of proxied controllers on that FPP instance. 'All' should be selected on Standalone/Master FPP Devices and 'Proxied' should be used for Remote FPP Devices that act as a tunnel to other controllers like a F16v3.

![](<../../../.gitbook/assets/image (896).png>)

The Playlist drop allows the user to select a predefined Playlist in FPP to add the uploaded Sequences too.

![PlayList Drop-Down](<../../../.gitbook/assets/image (800).png>)

The Pixel Hat/Cap Column will display if a Output device is attached and configured. Devices like PiCaps, Matrix PiHat, F8-B, etc will appear if they are configured in FPP. If the Checkbox is selected the input channels will be configure. For Matrix PiHat the panel start channel will also be configured.

![Hat/Cap Information](<../../../.gitbook/assets/image (227).png>)

You can then select one or more sequences to upload. The sequence FSEQ files are listed here. If the sequence is an audio sequence then the media file will also be uploaded if the media checkbox is selected.

![Sequence Selection](<../../../.gitbook/assets/image (300).png>)

There is a Right Click Menu to Select All Sequences, Clear Selections, Select Highlighted, or Deselect Highlighted.

![](<../../../.gitbook/assets/image (490).png>)

When the upload button is clicked all selected items will be uploaded to the FPP instances with the Upload Option checked and the dialog will close. Cancel will close the dialog without uploading any changes.

![Add FPP, Upload, and Cancel Button](<../../../.gitbook/assets/image (621).png>)
