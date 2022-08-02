# Controllers Settings

{% hint style="info" %}
As described under [Quick Start Guide](../chapter-two-quick-start-guide/), you can start with a default set of configuration values and then come back to change or update the details before testing your lights physical output. Or you can chose to not define any network information at the beginning until you wish to test from within xLights.
{% endhint %}

## Controllers List

![](<../../.gitbook/assets/image (877).png>)

The Controller Panel is divided into two parts. The list on left displays all the controllers defined by the user. The right grid displays the setting for the currently highlighted controller.

Each controller should be defined as single line in controller list. These controllers are then used to determine the start channels for the models in the layout tab. The start channels can be automatically set by xLights or manually setup by the user.

![](<../../.gitbook/assets/image (879).png>)

### Controller Types

| Type     | Description                                                                       |
| -------- | --------------------------------------------------------------------------------- |
| USB      | DMX, Pixelnet, LOR dongle, LOR optimized, D-Light, Renard, or OpenDMX Controllers |
| Ethernet | Artnet, E1.31, DDP, or ZCPP Controllers                                           |
| Null     | "Empty" Controllers                                                               |

### Save

Clicking on Save will save the current configuration to the "xlights\_networks.xml" file in the current show directory. After any changes are made to the Controller tab the Save button will turn red to identify there are unsaved changes.

### Adding Controller

To add a controller, click the add button for the desired controller type.

![](<../../.gitbook/assets/image (424).png>)

### Discovery

This will automatically find ZCPP and DDP controllers already attached to the local network.

## Controller Settings Grid

![](<../../.gitbook/assets/image (873).png>)

The controller setting grid displays the settings for the currently selected controller. If no controller is selected , the settings grid will display global settings that affect all the controllers. The controllers settings vary based on the controller type and the settings selection.

### Name

The controller name needs to be unique for each controller. This name is used by xLights to map the models to the controllers.

![](<../../.gitbook/assets/image (56).png>)

### Description

The description field can be added by the user to add more details about the controller.

### Id

![](<../../.gitbook/assets/image (229).png>)

For Artnet and E1.31 controllers, The ID field is used for the Universe ID's for the controller to receive data on. For other controller types the ID Filed can be see to an unique ID for use with start channel addressing.&#x20;

### Active

![](<../../.gitbook/assets/image (757).png>)

The "Active" drop-down determines if a controller is used when "Output to lights" is turned on. When "Active" xLights will output channel data to the controller. If "xLights Only" is selected, data will only be sent from xLights. If using xSchedule or when Uploading to FPP this controller will be set inactive. This is intended for FPP type controllers being used in Master/Slave mode. If set to "Inactive", no data output occurs. For example, if you have a controller not plugged in (testing a different controller) disabling that controller would not attempt to send anything to that specific controller. Trying to send data to a controller that is not connected and in some cases cause delays and lags on the output. When an controller is deactivated the row will be "grayed out" to show that it is not enabled.

### Vendor, Controller, & Variant

![](<../../.gitbook/assets/image (60).png>)

The Vendor, Controller, and Variant fields are used to setup which hardware controller will be used. xLights will use this information to determine what protocols are supported and the max number of universe and/or channels allowed. Not all controller types require the variant field to be populated. If the controller being used is not listed, leave the fields blank.

### Auto Size

![](<../../.gitbook/assets/image (92).png>)

When "Auto Size" is enabled, xLights will automatically adjust the controllers channel size based on the controller connections. This option only works when "Auto Layout Models" is enabled. It will **not** work with absolute or universe addressing.

### Auto Layout Models

![](<../../.gitbook/assets/image (52).png>)

When "Auto Layout Models" is enabled, xLights will automatically change the models start channels based on the controller connections.

### Auto Upload Configuration

![](<../../.gitbook/assets/image (882).png>)

When enabled, xLights will automatically upload the controller configuration when output to lights is turned on. This only works with FPP based controllers.

### Full xLights Control

![](<../../.gitbook/assets/image (702).png>)

When "Full xLights Control" is enabled, xLights will erase all the current controller settings when preforming the upload process.

### Suppress Duplicate Frames

![](<../../.gitbook/assets/image (886).png>)

By default, data will be sent every output frame, If this option is enabled, xLights will only output data if the data is different from the previous frame. This is useful for slow controllers to prevent lag. Most E1.31 and DDP controllers should not enable this option.&#x20;

### FPP Proxy IP/Hostname

![](<../../.gitbook/assets/image (626).png>)

This is needed when a FPP device is being used as proxy or bridge between your home network and show network, where the controller are attached.  This is typically the WIFI IP of a FPP instance that bridges the wifi and Ethernet networks. The FPP Proxy IP/Host option is used in conjunction with FPP 2.8+ Controller Proxy.

## USB Controller

USB Controller type is used to define a DMX, Pixelnet-Open, LOR dongle, LOR optimized, D-Light, Renard, or OpenDMX controller. The USB type can be used to for physical serial ports on the PC or "virtual" serial ports using a USB FTDI adapter.

![](<../../.gitbook/assets/image (125).png>)

{% content-ref url="lighting-networks/usb-controller.md" %}
[usb-controller.md](lighting-networks/usb-controller.md)
{% endcontent-ref %}

## Ethernet Controller

Ethernet Controller type is used to define a E1.31, Artnet, DDP or ZCPP controller. The controller will be attached to the PC thought the ethernet or Wifi interface.

![](<../../.gitbook/assets/image (880).png>)

{% content-ref url="lighting-networks/ethernet-controller.md" %}
[ethernet-controller.md](lighting-networks/ethernet-controller.md)
{% endcontent-ref %}

## NULL Controller

NULL controller type is used to generate channel blocks with no physical hardware or controller. This type of controller is used in setups, where the sequence output will not be used by xLights as a show player, but output data to be used for playback on a standalone controller.

![](<../../.gitbook/assets/image (270).png>)

{% content-ref url="lighting-networks/null-controller.md" %}
[null-controller.md](lighting-networks/null-controller.md)
{% endcontent-ref %}

## Controller Buttons

![](<../../.gitbook/assets/image (594).png>)

### Visualise

The Visualise buttons allows the user to visually arrange which models are connected to each controller.

{% content-ref url="lighting-networks/controller-visualizer.md" %}
[controller-visualizer.md](lighting-networks/controller-visualizer.md)
{% endcontent-ref %}

###

### Upload Input

Upload Input will copy all the E1.31 universe inputs defined to the selected controller. This requires a valid IP address, and that multicast is not being used. The E1.31 Input Definition's will only be preformed for the controller selected.

{% hint style="info" %}
Input Upload is only required for E1.31 or ArtNET controllers. i.e FPP, Falcon, and SanDevices. Output Upload is required for all supported controllers types.
{% endhint %}

### Upload Output

Upload Output uses the parameters from models controller connections in the Layout tab/Visualise and uploads these settings to the controller. This feature is available for the following boards : Falcon, Pixlite/Pixcon, SanDevices, J1SYS, AlphaPix, HinksPix, Espixelstick, and most FPP caps and capes. This feature is compatible with both universe/channel addressing and absolute addressing.

{% hint style="info" %}
The Visualise, Upload Inputs/Output functions will not work if the controller is displaying unmanaged mode. Unmanaged mode is set automatically by xLights when two controller outputs have the same IP address. While valid, this is highly **not** recommended and will disable these xLights functionality.
{% endhint %}

### Open Controller

Open the currently selected controller in the default web browser.

### Delete

This will delete the selected controller.

### Controller Status Indicator&#x20;

![](<../../.gitbook/assets/image (317).png>)

The green indicator identifies if the controller is connected and responding to ping requests. For serial ports this will indicate if the Com port can be opened. If red the controller is not responding.&#x20;
