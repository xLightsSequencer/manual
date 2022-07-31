# Show Directory

## **Show** Directory

![](<../../.gitbook/assets/image (595).png>)

The xLights Show Directory is where all the required xLights sequences, pictures, and user configuration files used to run the sequences are kept. When a sequence (.xsq) is saved and a binary file (.fseq) rendered, both files are created in the show directory. This is the same location where xLights configuration files can be found and the default location where the program will first prompt for, or look for files pertaining to several functions of xLights.

Specifying or changing the location of the Show directories can be done by clicking on the Change button found on the Controller tab screen.

{% hint style="success" %}
It is useful to have separate show directories for each major event i.e. one for Halloween, one for Christmas or one for the next year. Start a new year directory by copying sequences from the Show Directory of the previous year.
{% endhint %}

{% hint style="success" %}
Keep the folder name, containing the 'xlights\_rgbeffects.xml' file the same when creating a new show folder. Create the new folders in the lower level directory and xlights will automatic adjust file paths. As an example, use "2018/Christmas" then "2019/Christmas" (the last sub folder folder is the same) instead of "Christmas/2018" and "Christmas/2019".
{% endhint %}

{% hint style="danger" %}
Images used for pictures and faces use an absolute location reference. If you are not using the suggested structure, then the location won’t be found if you change your show directory.
{% endhint %}

In some cases if you copy your show directory to another location or drive xLights may still be able to successfully locate image files despite the absolute reference (in the case where the the last sub folder of the location has the same name).

If you have a show folder c:\show and you move it to e:\xxx\yyy\show it will seamlessly work as long as all the files your sequence needs are in the show folder or one of its subdirectories. Anything located elsewhere will not be seamlessly moved but if they are still there they will be used.

{% hint style="warning" %}
This is useful if you are moving your setup to a USB drive or Dropbox. If however you move it to c:\show\_old and try to set that as the show directory, then the files won't be referenced.
{% endhint %}

### Change Permanently

![](<../../.gitbook/assets/image (595).png>)

The "Change Permanently" button will allow the user to specify the location of the their primary show directory on disk. This show directory location will be remembered when xLights is closed and reopened.

### Change Temporarily

The "Change Temporarily" button will allow the user to temporary switch show directories. The show directory path name will turn the color yellow to signify a temporary show directory is being used. When xLights is closed and reopened, this "temporary" show directory will be forgotten and xLights will resume use of the "Permanent" Show directory. The "Restore to Permanent" button will also switch back to the "Permanent" Show directory. The "temporary" show directory should be used when importing a sequence.

![](<../../.gitbook/assets/image (390).png>)
