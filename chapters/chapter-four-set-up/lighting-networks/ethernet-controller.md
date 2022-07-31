# Ethernet Controller

## Ethernet Controller

![](<../../../.gitbook/assets/image (1120).png>)

Ethernet Controller type is used to define a E1.31, Artnet, DDP or ZCPP controller. The controller will be attached to the PC thought the ethernet or Wifi interface.

![](<../../../.gitbook/assets/image (967).png>)

Click the Add Ethernet button to add a new Ethernet controller. Select a row to highlight the controller and change the settings.

## Ethernet Controller Settings

![](<../../../.gitbook/assets/image (1091).png>)

### Multicast

**(ArtNet/E1.31)** When enabled, Multicast will send Ethernet data to all subscribed Ethernet controller on the network. IP address is not needed when enabled.

![](<../../../.gitbook/assets/image (1032).png>)

### IP Address

Sets the IP Address of the Ethernet controller. The host name can also be entered in this field.

### Protocol

| Protocol | Description                                                                                                                                                                                                                                                                                                                                                                                                                 |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ArtNet   | ArtNet is a protocol for sending DMX512 data over Ethernet or Wifi. Similar to E1.31, ArtNet  group channels into Universes. ArtNet is upported by most ethernet based controllers.                                                                                                                                                                                                                                         |
| DDP      | Distributed Display Protocol is a high efficiency data protocol. It is more efficiency than ArtNET or E.131. Currently, this protocol is not supported by all Ethernet based controllers. (only HinksPix, FPP 2.x+, Falcon v3 FW 2.58+ and Minleon)                                                                                                                                                                         |
| E1.31    | E1.31 (also called Streaming ACN or sACN) is a protocol for sending DMX512 data over Ethernet or Wifi. Channels of are grouped into blocks of channels called, Universes. Universes are can be any size up to 512 channels. Universe Size of 510 or 512 are supported by most devices. E1.31 is an industry standard and supported by most ethernet controllers.                                                            |
| OPC      | Open Pixel Control is a protocol for controlling DIY Pixel Controllers. Used by some DIY Arduino/Raspberry controllers.                                                                                                                                                                                                                                                                                                     |
| ZCPP     | Zero Configuration Pixel Protocol is a high efficiency specific data protocol with build in configuration data for the controller outputs. It was designed to automatically configure the controller outputs in real time. It is more efficiency than ArtNET or E.131. Currently, this protocol is not supported by all Ethernet/Wifi based controllers. (only Falcons v3 FW 2.5+ and ESPixelStick FW 3 based controllers)  |

### Priority

**(ZCPP/E1.31)** Priority is supported by some controllers and is used to determine which data packet to use is multiple packets are received controlling the same channels.

### Start Universe

**(ArtNet/E1.31)** This sets what is the first universe for the controller to listen for data on. **** Can be any value from 1 to 63999. It is recommend to not overlap universe between controllers.

### Universe Count

**(ArtNet/E1.31)** The number of universe sets the number of channels allocated for the controller. This is multiplied by the universe size to get the total channels. If using Auto Size this will be grayed out and set automatically.

### **Universe Size**

**(ArtNet/E1.31)** This **** sets the number of channel per universe. Universe can be any size up to 512 channels. Some controllers require a size of 510 or 512. 510 is recommended.

### Individual Sizes

**(ArtNet/E1.31)** When Enabled, this allows the user to manually set each universe size independent of each other. Not recommended.

![](<../../../.gitbook/assets/image (982).png>)

### Channels Per Packet

**(DDP)** The number of channels sent in each packet, this should be left to the default of 1440.&#x20;

### Keep Channels Per Packet

**(DDP)** If checked absolute channel numbers will be sent, this sends the channel numbers to the controller. If unchecked the first channel sent to the DDP controller will be channel 1. Enabled is recommended.

### Channels

**(ZCPP/DDP)** Channels is the total number of channels that the controller is using. If using Auto Size this will be grayed out and set automatically.
