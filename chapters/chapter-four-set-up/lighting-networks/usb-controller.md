# USB Controller

## USB Controller

![](<../../../.gitbook/assets/image (456).png>)

USB Controller type is used to define a DMX, Pixelnet-Open, LOR dongle, LOR optimized, D-Light, Renard, or OpenDMX setup. The USB  type can be used to for physical serial ports on the PC or "virtual" serial ports using a USB FTDI adapter.

![](<../../../.gitbook/assets/image (31).png>)

Click the Add USB button to add a new USB controller. Select a row to highlight the controller and change the settings.

![](<../../../.gitbook/assets/image (58).png>)

## USB Controller Settings

![](<../../../.gitbook/assets/image (468).png>)

### Port

Sets the serial port used for the the serial device. The dropdown will populate with all the connected devices. Select "Not Connected" if the device is not currently attached.

### Speed

Sets the speed of the serial device, normally listed as baud-rate or bit-rate.

### Channels

Number of channels of the serial device. For most DMX devices this needs to be 512.

### Protocol

| Protocol       | Description                                                                                                                                                                                                                                                                                              |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DMX            | Compatible with Entec Pro, Lynx DMX, DIYC RPM, DMXking.com, and DIYblinky.com dongles. Universes are exactly 512 bytes, except for DIYblinky, where they can be up to 3036 bytes.                                                                                                                        |
| LOR            | LOR controllers attached to any LOR dongle. Max of 8 channels at 9600 baud. Max of 48 channels at 57600 baud. Max of 96 channels at 115200 baud.                                                                                                                                                         |
| LOR Optimised  | LOR controllers attached to any LOR dongle. LOR Optimised is designed to use some of the more advanced commands to reduce the amount of bytes sent out the LOR network. Setup all the controllers that are on this LOR network so that xLights will know which Unit ID's to utilize for each controller. |
| OpenDMX        | Compatible with Entec Open DMX, LOR dongle, D-Light dongle, and any other FTDI-based USB to RS-485 converter.                                                                                                                                                                                            |
| Pixelnet -Open | Pixelnet controllers attached to a generic USB to RS485 dongle with FTDI chipset.                                                                                                                                                                                                                        |
| Renard         | Renard controllers connected to a serial port or a USB dongle. 2 stop bits are set automatically. Max of 42 channels at 9600 baud. Max of 260 channels at 57600 baud                                                                                                                                     |
| D-Light        | D-Light controllers attached to a D-Light dongle. Max of 8 channels at 9600 baud. Max of 48 channels at 57600 baud. Max of 96 channels at 115200 baud.                                                                                                                                                   |
| Generic Serial | Generic Serial type sends raw channel data to the serial port. This is intended for Arduino type controllers. Eight data bits, no parity bit, and one stop bit (8N1) is the only support configuration.                                                                                                  |

## LOR Optimised

LOR Optimized is much closer to true LOR protocol and utilizes some of the more advanced commands.&#x20;

![](<../../../.gitbook/assets/image (38).png>)

First, set an ID of the output, this is **not** the LOR unit ID of a controller box, it is a unique ID that xLights will use to direct the channel data to this output. The port is the COM port of the dongle in use, Baud Rate is adjustable. NOTE: Older black or white LOR dongles do not support speeds over 115200, Only the red LOR dongle will support higher speeds. Description is user defined value to identify the controller. The Devices setting sets the number of LOR Controller. Based on the Devices number, the settings grid will add setting for each LOR controller.

![](<../../../.gitbook/assets/image (32).png>)

The settings grid will list the LOR controller. Each controller will be listed by controller type, **Unit ID**, Channels, and Address Mode. Note: xLights cannot set the unit ID to the controller, this must be done via the LOR software or from the DIP switches on the controller board if applicable.

Select the LOR controller type, the available choices are: AC Controller, RGB controller, CCR, CCB, and the 3 Pixie Controllers (4 ,8, 16 output boards). Then select the number of channels for this controller board. Next is the unit ID. This can be very confusing as LOR uses a hexadecimal system for numbering their UNIT ID's. Units 1 to 16 are 0x01-0x0F and units 17-32 are 0x11-0x1F. Make sure the hex number in bold matches the LOR unit ID in their software. Set the addressing mode as normal, legacy, and split. A description for each controller can be provided.
