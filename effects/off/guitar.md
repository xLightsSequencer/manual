# Guitar

The Guitar effect turns MIDI note data into an animated stringed-instrument visualization. Using note data from a MIDI timing track it lights up strings and fret positions in time with the music, and can be styled as a guitar, bass guitar, banjo or violin.

<!-- TODO: screenshot -->

| **Options/Setting** | **Description** |
| --- | --- |
| **Type** | Selects the instrument type, which determines the number of strings and tuning used to map MIDI notes to fret positions. Options: Guitar, Bass Guitar, Banjo, Violin. Default Guitar. |
| **Track** | The timing track containing MIDI note data that drives the guitar visualization. |
| **String Appearance** | How active strings are drawn. On fills a solid band for each string; Wave draws a sine wave oscillation simulating a vibrating string. Options: On, Wave. Default On. |
| **Fret Count** | Maximum number of frets on the instrument neck. Higher fret notes are drawn shorter across the buffer width. Range 8-30. Default 19. |
| **Base Wavelength** | Base wavelength multiplier for the wave string appearance. Higher values produce longer, smoother waves. Range 0.1-10.0. Default 1.0. |
| **Vary Wavelength By String** | How much the wavelength varies between strings. Higher values make lower-pitched strings wave more slowly than higher strings. Range 0.0-10.0. Default 0.0. |
| **Fade** | When enabled, notes fade out over their duration by reducing alpha transparency. Default False. |
| **Collapse** | When enabled, the height of each string's visual shrinks over the note duration, simulating a decaying vibration. Default False. |
| **Show Strings** | When enabled, draws a thin line for each string beyond the fret position, showing the unfretted portion of the string. Default False. |
| **Vary Wavelength By Fret** | When enabled, the wave wavelength varies based on fret position so that higher frets produce shorter, tighter waves. Default True. |
