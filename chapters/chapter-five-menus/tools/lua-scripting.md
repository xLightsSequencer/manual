# Lua Scripting

### Overview

xLights includes an embedded Lua interpreter that lets you automate repetitive tasks — things like importing effects across dozens of sequences, batch-exporting models, uploading configurations to FPP instances, or renaming/renumbering elements — without clicking through the UI for every sequence or model. Anything exposed to Lua runs against the currently open show folder, so a script can iterate over every sequence in your show and perform the same operation on each one.

Lua scripting is reached from **Tools → Run Scripts**. This opens a dialog where you can browse to a `.lua` file, run it, and view its output/log in real time.

\{% hint style="info" %\} Lua automation is aimed at users comfortable with a little scripting. If you've never used Lua before, the [Lua 5.x reference manual](https://www.lua.org/manual/5.4/) covers the language itself (variables, loops, tables, functions); this page covers the xLights-specific functions layered on top of it. \{% endhint %\}

### Where scripts live

* Scripts are plain text `.lua` files. You can keep them anywhere on disk; the Run Scripts dialog lets you browse to any location.
* Many users keep a personal scripts folder outside their show folder so the same scripts can be reused across multiple shows/seasons.
* Community-contributed scripts are published on GitHub rather than bundled inside the xLights installer — this keeps the install size down and lets scripts be updated independently of xLights releases. A good starting point is browsing existing example scripts (search GitHub for "xlights\_scripts") to see working patterns before writing your own.

### Running a script

1. Open the show folder / sequence(s) you want the script to act on (some functions require a sequence to be open; others, like bulk model exports, don't).
2. **Tools → Run Scripts**.
3. Browse to your `.lua` file.
4. Click **Run**.
5. Watch the output pane — scripts typically log progress with `Print()` calls, and any `xlDisplayError`/`xlDisplayWarning` calls will pop a dialog.

Because a script can modify or overwrite files in your show folder (sequences, exports, uploads to controllers), **back up your show folder before running an unfamiliar script**, the same way you would before a batch render.

### What you can automate

Broadly, the Lua automation surface covers:

* **Sequence lifecycle** — creating, opening, closing, and saving sequences programmatically, so a script can loop over every sequence in a folder.
* **Effects** — adding effects to the timeline, cloning effects from one sequence to another (useful for propagating a "flourish" effect across a whole show), and triggering renders.
* **Import / mapping** — driving the sequence import and AI-assisted model auto-mapping workflow from a script, so a repetitive import (e.g., applying the same donor sequence to many target sequences) doesn't need to be repeated by hand in the Import dialog each time.
* **Model export** — bulk-exporting rendered video for one or more models, including selecting the export format (e.g., MP4, lossless RGB, ProRes variants).
* **FPP integration** — uploading FPP configuration and/or sequences to a Falcon Player instance, similar to what FPP Connect does interactively, but scriptable and repeatable across many controllers.
* **User interaction** — simple prompts and message/error/warning dialogs so a script can ask the user a question mid-run or report problems clearly instead of failing silently.

### User interaction functions

These give a script a way to talk to the person running it:

| Function                           | Purpose                                                             |
| ---------------------------------- | ------------------------------------------------------------------- |
| `Print(text)`                      | Writes a line to the script's output/log pane.                      |
| `xlDisplayMessage(text)`           | Shows an informational popup.                                       |
| `xlDisplayWarning(text)`           | Shows a warning popup.                                              |
| `xlDisplayError(text)`             | Shows an error popup — good for aborting a run with a clear reason. |
| `xlPrompt(text)`                   | Prompts the user for free-text input, returning what they typed.    |
| `xlPromptSelection(text, options)` | Prompts the user to choose from a list of options.                  |

### Common automation functions

The exact set of available functions and their parameters can change between xLights releases as new automation is added (recent releases, for example, added scripting support for sequence import/auto-mapping and expanded the set of video export formats reachable from a script). Rather than duplicate a list here that can drift out of date, use the **Run Scripts** dialog itself as the authoritative reference — it lists the functions available in your installed version, which is always the source of truth for exact names and arguments.

That said, the general shape of the API is stable across versions and typically includes functions to:

```
-- lifecycle
newSequence(...)
openSequence(path)
saveSequence()
saveSequenceAs(path)
closeSequence()

-- effects & rendering
addEffect(...)
render()
renderAll()

-- export
exportModel(modelName, folder, format)
exportModelWithRender(modelName, folder, format)

-- FPP
uploadFPPConfig(ip)
uploadSequence(ip)
```

Treat the snippet above as illustrative of the categories, not a guaranteed-accurate function signature list — confirm exact names/parameters against your version before relying on them in a production script.

### Example: batch export a model from every sequence

lua

```lua
-- Example pattern only — verify function names/args against
-- your installed version's Run Scripts reference before use.

local sequences = {"song1.xsq", "song2.xsq", "song3.xsq"}
local exportFolder = "C:/xLights/exports"

for _, seq in ipairs(sequences) do
    Print("Processing " .. seq)
    openSequence(seq)
    render()
    exportModel("MyTree", exportFolder, "mp4")
    closeSequence()
end

Print("Batch export complete.")
```

### Writing your own scripts

* Start from a small, working example (your own or a community one) and modify it incrementally rather than writing from scratch — it's much faster to debug one changed line than a whole new script.
* Use `Print()` liberally while developing; it's the easiest way to confirm the script is doing what you expect at each step.
* Wrap risky operations (file paths that might not exist, uploads that might fail) so a bad run reports a clear `xlDisplayError` message rather than leaving you guessing.
* Keep destructive operations (overwriting sequences, uploading to live controllers) behind an explicit confirmation prompt (`xlPromptSelection`) until the script is well-tested.

### Getting help

* Check the **Run Scripts** dialog's built-in function reference for the current, version-accurate list of available calls.
* The xLights [Facebook group](https://www.facebook.com/groups/xlights) and [GitHub Discussions/Issues](https://github.com/xLightsSequencer/xLights) are good places to ask about specific automation functions or share scripts.
* If you write something broadly useful, consider publishing it (with a license) so other users can adapt it — most community scripts circulate this way rather than being bundled with xLights itself.
