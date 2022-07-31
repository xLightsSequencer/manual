# Convert

## Convert

The Convert function is commonly used to convert a sequence file from one sequencer format to the format of another sequencer or to the format (.fseq) required to run via Falcon Player on a Raspberry Pi or BeagleBone Black controller.

![](https://lh3.googleusercontent.com/f2m\_JsfnS2zBWjhM3gnV0WSCT0f2i2I9V-7xGS8npXF1XVvUB-nuT3A-hyi37N78KJ9AD-b2aIGVNcZv\_0OlhBbYuoUvHfWzp\_wWFuxvJ7sQrQWoGVx4WgkV1n8DEv7UmW3bf\_4N)

It is not to be used to convert into an xLights sequence – use the Data Layer or Import, Import Effects options to achieve that.

Supported input/output formats are:

![](<../../../.gitbook/assets/image (104).png>)

![Convert Dialog](<../../../.gitbook/assets/image (486).png>)

1.  Click on Choose Files, and on the subsequent window, change the file type to the type of file that you wish to convert and navigate to where your input file (i.e. LOR LMS file etc) is located. Select the file and Click Open or Double click to select the file.

    ![](https://lh5.googleusercontent.com/MQcuNYXk4uJuK23C2MRkXGoA4GPAq9k8NuMQnG\_iHXhCVc3UJ--O-Bp88X3vf11Z5iBjb0PL0Og9iLmegqfhyyoimZPhqMbPPpRM0TnT\_C7uWosnhoHcDApnGyuDcAsXNjEuqFbt)
2. Select the output Format to convert to. Supported output formats are:
3. Specify whether all channels should be turned off at the end of the sequence. (Tick if unsure)
4. Select the Show Verbose Channel Map.  This option will display messages pertaining to the input sequencer channel mapping  for some inputs and is useful to identify missing or misaligned channel information.
5. Select the options specific to LOR conversion.
6. Specify the time resolution i.e. (25ms, 50ms, 100ms). These correspond to (40 fps, 20 fps, and 10 fps respectively).  Select 50ms if not sure.
7. Click on Start Conversion.
8. Conversion messages are displayed. If successfully converted, a file of the same name but with a different extension (i.e. as specified for the Output Format) will be created in your show directory.

![](https://lh6.googleusercontent.com/Rnt913O-guwOx5TLfYEWzs1WXCPw9khRaAsUjnUAwosiy25v75TuPZdihFhRQzWi9wYTOo8eB8aWVAnJRzgIsvPTxWUh1Q6cCkZ7xzihVHb2\_0aeRdNYlQoRZ7f\_gp4bR66ea46N)

With the ‘Show Verbose Channel Map’ selected, the conversion messages display which channels have been converted to equivalent xLights channels. This information can then be used to amend the channel mapping and/or define additional LOR controllers as required.
