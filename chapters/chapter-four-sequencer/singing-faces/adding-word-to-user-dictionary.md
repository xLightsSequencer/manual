# Adding Word to User Dictionary

{% hint style="warning" %}
This is an advance method, It is recommended to use the User Lyric Dictionary Dialog instead.&#x20;
{% endhint %}

{% content-ref url="../../chapter-five-menus/tools/" %}
[tools](../../chapter-five-menus/tools/)
{% endcontent-ref %}

## User Dictionary File Location

The standard\_library and extended\_library are built-in dictionaries which contain information that assist xLights in converting each word into phonemes. Each word in the dictionary is listed with its associated phonemes. As xLights proceeds with the breakdown process there may occasionally be a word that it cannot find in these dictionary files. When this happens there is a simple process to add that word to the user\_dictionary.

When xLights is first installed, this file is located in this folder:  C:\Program Files\xLights\  This folder is the default folder that xLights is installed into. This can change if you decide to install xLights somewhere else.

To keep this file from being overwritten in future installs you should move the user\_dictionary file to the folder where you store your sequences.

The user\_dictionary can be moved to the Show Directory and xLights will read it from there. If you do this xLights will load the user\_dictionary in the show directory and skip the user\_dictionary in Program Files.&#x20;

## Editing the User Dictionary

The user\_dictionary is a simple text file which can be edited by using a text editor such as windows notepad or any other text editor, such as Notepad++, to open this file. This is only dictionary file that you should make any additions to because the other two files will be overwritten each time xLights is installed. When you first open the user\_dictionary file it will contain the information shown below.

![](<../../../.gitbook/assets/pasted image 0 (21).png>)

Before continuing, create a text file containing all the words that xLights did not have an associated  phoneme breakdown created. Name this something easily identifiable, such as ‘missing words.txt’ and put it in the same folder as the sequences. There is no special formatting, just a list of words, one per line, is required. One thing to note here is that if you have any hyphenated words such as ‘screa-um’ you should break the word into two words such as ‘screa’ and ‘um’’ for this list.

Then in your internet browser open to the following webpage… [http://www.speech.cs.cmu.edu/tools/lextool.html](http://www.speech.cs.cmu.edu/tools/lextool.html) as shown here:

![](<../../../.gitbook/assets/pasted image 0 (22).png>)

Then click the ‘'Choose File' button and browse to find the file you created or enter this name into the file box.

Then click the 'Compile' button.

Once the processing has completed another web page will appear similar to this:

![](<../../../.gitbook/assets/pasted image 0 (23).png>)

Click the work 'link'

Another web page similar to this will appear.

![](<../../../.gitbook/assets/pasted image 0 (24).png>)

Here click the file with the .dict extension such as 0548.dict, then a web page will appear with the words and their phoneme breakdown as shown below.

![](<../../../.gitbook/assets/pasted image 0 (25).png>)

Before following the rest of this process, close the current sequence and exit xLights.

If your user\_dictionary is not open, open it now. Highlight and copy this list and paste it into your open user\_dictionary and save the newly modified file. There is a small bug in xLights at the time this document was written which you need to compensate for. After pasting in the newly added words do a search and replace with a ‘ ‘ (space) for any ‘tab’ characters in the user\_dictionary. Between the "word" and the "phonemes" requires two spaces ('  ') and one space(' ') is required between phonemes.

![](<../../../.gitbook/assets/image (561).png>)



This process will work for one to how ever many words that you have. But if you just want to quickly check one word past the following link into your browser.

[http://www.speech.cs.cmu.edu/cgi-bin/cmudict](http://www.speech.cs.cmu.edu/cgi-bin/cmudict)

This is the online CMU Pronouncing Dictionary. Here you will look up each word that Papagayo did not find in its dictionaries. Let’s take the first word 'ooky'. There is a box below the title ‘Look up the pronunciation for a word or a sentence in CMUdict (v. 0.7a)’ where you will enter this word. Then click the 'Pronounce it!’ button. If a red dot appears with the phrase ‘not in dictionary; consider using the LOGIOS tool discussed above, which is able to generate missing pronunciations by rule.’ Then you need to click the ‘LOGIOS’ link which takes you to the previously discussed web page.

Now that you have updated the user dictionary you should reopen xLights and load the previously saved sequence and find the newly added dictionary words and do a right click ‘Breakdown Word’ for the missing phonemes.  The image now shows the results after adding the word ‘honkey’ to the user\_dictionary file.

![](<../../../.gitbook/assets/pasted image 0 (26).png>)
