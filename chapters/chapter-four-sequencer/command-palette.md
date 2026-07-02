# Command Palette

The Command Palette is a searchable launcher that lets you find and run almost anything in xLights without hunting through the menus. Press **Ctrl+Shift+K** (Windows/Linux) or **Cmd+Shift+K** (macOS) anywhere in the sequencer to open it, start typing, and pick what you want.

<!-- TODO: screenshot -->

## Opening the Palette

The palette appears near the top-centre of the main window with the search box already focused, so you can begin typing immediately. Press **Escape** at any time to close it without doing anything.

## Searching

Type into the search box to filter the list. Matching is fuzzy: you can type the letters of a command in order without typing them consecutively, so a short query like `rendall` will find **Render All**. The characters that matched your query are highlighted in each result, and the closest matches are sorted to the top - entries that match at the start of a word or command name rank higher.

You can also match on a command's location. Each result shows the menu it lives under (for example `Edit` or `Tools > ...`), and typing part of that category will narrow the list as well.

## Navigating and Running

The first result is selected automatically. Use the **Up** and **Down** arrow keys to move through the list, then press **Enter** to run the highlighted item. You can also double-click any result to run it. If you start typing while the results list has focus, the text is sent straight to the search box so you can keep refining your query.

## What You Can Launch

The palette gathers two kinds of items:

* **Menu commands** - every enabled command from the xLights menu bar, including items inside submenus. Each result shows the menu path it came from, and any command that has a keyboard shortcut displays that shortcut as a badge on the right. Running a menu command from the palette behaves exactly as if you had chosen it from the menu.
* **Effects** - every available effect, listed under the **Add Effect** category with the effect's icon shown beside its name. Choosing an effect adds it to the currently selected cell in the sequencer grid using the current effect settings, just like dropping the effect onto the timeline, and the newly added effect is selected for you.

{% hint style="info" %}
Only commands that are currently enabled appear in the palette. If a command depends on a sequence being open or on a selection, open the sequence or make the selection first and it will show up.
{% endhint %}
