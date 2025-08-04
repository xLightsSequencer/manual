# Other

## Other

<figure><img src="../../../../.gitbook/assets/image (1206).png" alt=""><figcaption></figcaption></figure>

### eMail Address

This settings allows the user to provide a contact email for when xLights submits a crash report. This is completely optional.

### Hardware Video Decoder

This setting allows xLights to use the computer's GPU to render video files. If you are having issues with video file's not displaying, it is recommended to disable this setting.



<figure><img src="../../../../.gitbook/assets/image (1207).png" alt=""><figcaption></figcaption></figure>

Configure the Hardware Engine used to Decode Video Files.&#x20;

<table><thead><tr><th width="169.33331298828125"></th><th width="588"></th></tr></thead><tbody><tr><td>DirectX11</td><td>Use Native DirectX 11 Media Library on Windows</td></tr><tr><td>FFmpeg Auto</td><td>FFmpeg library include in xLight will determine the Hardware Render</td></tr><tr><td>FFmpeg CUDA</td><td>FFmpeg library will use the Nvidia Hardware Render</td></tr><tr><td>FFmpeg QSV</td><td>FFmpeg library will use the Intel Quick Sync Hardware Render</td></tr><tr><td>FFmpeg Vulkan</td><td>FFmpeg library will use the Vulkan Hardware Render(Not Recommended)</td></tr><tr><td>FFmpeg AMF</td><td>FFmpeg library will use the AMD Radian Hardware Render</td></tr><tr><td>FFmpeg DirectX11</td><td>Use FFmpeg DirectX 11 Media Library Wrapper</td></tr></tbody></table>

### Shader On Background Threads

This setting allows xLights to compile shader effects on a background. This can help improve render times of shaders.

### Prompt issues during batch render

If enabled this will prompt the user of error during batch render. These errors could be related to missing models and missing effect files. If disables these errors will be ignored and render will be skipped for the models involved. This will cause batch render to pause and require the user to interact with the process.

### Purge download cache on startup

Clear out the Vender Model Download Cache on Startup. This will redownload the Vender Model list on every startup, this will make sure the model list is always up to date. It is recommended to enable this option on fast internet connections.

## Packaged Sequences

### Exclude Presets

If selected, when a sequence is packaged with the Package Sequence option, all effects presets are stripped from the xlights\_rgbeffects.xml file.

### Exclude Audio

If selected, when a sequence is packaged the audio file is skipped as it is generally not legal to share audio files with other people. When the recipient opens the sequence they will need to point to where the audio file is on their computer.

{% hint style="warning" %}
If excluding the audio from a packaged sequence, it is necessary to provide the source of the audio file to those the package sequence is being sent to. This is best done by filling on the metadata on the sequence settings for the song, artist, album, and music URL (link for download).
{% endhint %}

## Video Export Settings

### Video Codec

Set the Video Codec and bitrate used by the Export House Preview Menu Dropdown. H.264 is recommended new Macs (M1, M1 Max, M2) with hardware video rendering. MPEG-4 is an older/slower standard that will create large video files.

### Bitrate

Set the bitrate of the Exported Video File, 0 is Auto.

### Link Controller Upload

When Uploading Controller Inputs and Outputs, this will cause xLights to do both upload actions when Upload Output is clicked.

![](<../../../../.gitbook/assets/image (809).png>)

### Ignore vender model recommendation

Don't Disable, Will be removed in future versions.

### Controller ping interval in seconds

How often xLights pings the controllers in the Controllers Tab.

## Tip of the Day

Set the 'Level' of tips of the day, you will receive. Off will disable Tip of the day.

![](<../../../../.gitbook/assets/image (48).png>)
