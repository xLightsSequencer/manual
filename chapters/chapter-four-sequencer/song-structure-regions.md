# Song Structure Regions

Song Structure Regions let you divide the sequence timeline into named, colored sections - for example *Intro*, *Verse*, *Chorus*, *Bridge* and *Outro* - and then act on each section as a whole. Once a song is broken into regions you can copy the effects from one region to another, recolor every effect in a region, and export individual regions (or all of them) as brand new sequences. Regions are drawn as a colored tint behind the timeline ruler, with the region name shown above the band and a vertical boundary line between adjacent regions.

<!-- TODO: screenshot -->

## Creating Regions

Regions are bounded by *boundaries*. Each pair of adjacent boundaries (and the start and end of the sequence) defines a region. There are two ways to create them.

### Adding Boundaries Manually

Right click on the timeline ruler (the area above the grid where the time scale and waveform are shown) at the point where you want a section to begin, and choose **Add Song Structure Boundary Here**. Repeat at each point where a new section starts. To remove a boundary, right click near it and choose **Delete Song Structure Boundary**.

<!-- TODO: screenshot -->

### Creating Regions from a Timing Track

If you already have a timing track that marks the sections of the song (for example a track whose marks are labelled with the section names), you can turn it into regions in one step. Right click the timing track name in the row headings area and choose **Create Song Regions from Timing Track**.

xLights creates one region for each timing mark, using the timing mark's label as the region name and assigning each a color from the palette. Any gaps between marks - and the lead-in before the first mark or the tail after the last - are filled with unnamed filler regions so the whole timeline is covered. If song structure already exists you are asked to confirm, as this replaces the current regions.

{% hint style="info" %}
Only named regions are included when you export *all* regions, so the unnamed filler regions created to cover gaps are skipped during a bulk export.
{% endhint %}

## Editing a Region

Right click inside a region on the ruler and choose **Edit Region "..."** to open the region editor. Here you can give the region a name and pick a color swatch from the built-in palette. The chosen color is used for the band tint and the boundary, making it easy to see the structure of the song at a glance.

<!-- TODO: screenshot -->

## Per-Region Bulk Actions

Right clicking inside a region offers actions that operate on every effect that falls within that region's time range, across all model rows (timing tracks are not affected).

| Action | What it does |
|---|---|
| **Edit Region** | Rename the region and choose its color. |
| **Copy Effects to Region** | Submenu listing the other regions. Copies all effects in the current region into the chosen target region, shifting them by the difference in start times. Effects are only placed where the target is empty, so existing effects are not overwritten. |
| **Apply Selected Effect Palette to Region** | Applies the color palette of the currently selected effect to every effect in the region. This item is only enabled when an effect is selected in the grid. |
| **Export Song Region as New Sequence** | Saves just this region as a new `.xsq` sequence (see below). |

Copy and palette operations are added to the undo history, so they can be reversed with the normal undo command.

{% hint style="success" %}
**Copy Effects to Region** is ideal for repeated sections. Build the effects for your first chorus, then copy them onto every other chorus region in a couple of clicks - the effects land in the same relative position within each region.
{% endhint %}

## Exporting Regions as Sequences

Each region can be saved as a standalone sequence, which is useful for reusing a section or working on it in isolation.

* **Export Song Region as New Sequence** - right click inside a region and choose this option. A save dialog opens with the region name pre-filled; the region is written out as a new `.xsq` file.
* **Export All Song Regions as Sequences** - available whenever regions exist. Choose a destination folder and xLights writes each *named* region to its own `.xsq` file (unnamed filler regions are skipped). A progress dialog shows the export and can be cancelled.

## Song Structure Views

You can keep more than one arrangement of regions for the same sequence using **Song Structure Views**. The Song Structure Views submenu lets you create a **New View**, **Duplicate Current View**, **Rename Current View** or **Delete Current View**, and select which view is active from the list. Each view holds its own set of regions, so you can, for example, keep one coarse view of the major sections and another, finer breakdown.

## Clearing Regions

To remove all song structure from the sequence, right click on the ruler and choose **Clear Song Structure**.

{% hint style="info" %}
Song structure is saved with the sequence, so your regions and views are still there the next time you open it.
{% endhint %}
