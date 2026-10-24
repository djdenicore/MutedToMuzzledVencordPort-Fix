# MutedToMuzzled (PupCord)

A Vencord **QuickCSS stylesheet**, not a standalone Vencord plugin. It adds puppy-themed icons and wording to Discord's voice controls.

## What it changes

- **Microphone button:** shows `bark.png` when the mic is enabled and `dog.png` when muted or blocked.
- **Headphones button:** shows `cage2.png` while listening and `cage.png` while deafened.
- **Participant state icons:** replaces the microphone-muted and deafened icons where Discord displays them in voice channels.
- **Tooltips:** uses `Bark!!`, `Muzzled`, `Cage`, and `Caged`, regardless of Discord's UI language.
- **Typing indicator:** changes typing text to barking-themed wording.

The microphone icon indicates whether the mic is enabled; it does not detect when someone is actively speaking.

## Install

1. Open **Discord Settings → Vencord → Themes → Edit QuickCSS**. The exact menu wording can vary by Vencord version.
2. Add this line at the very top of your QuickCSS file:

   ```css
   @import url("https://raw.githubusercontent.com/djdenicore/MutedToMuzzledVencordPort-Fix/master/MutedToMuzzled.css");
   ```

3. Save the file. If the changes do not appear, make sure **Enable Custom CSS** is enabled in Vencord settings and reload Discord.

You can open the [raw stylesheet](https://raw.githubusercontent.com/djdenicore/MutedToMuzzledVencordPort-Fix/master/MutedToMuzzled.css) to confirm that the import URL loads plain CSS.

## Compatibility notes

- The stylesheet uses modern CSS features, including `:has()` and CSS nesting, so it requires a reasonably recent Discord/Vencord build.
- Discord's generated class names and inline SVG paths can change after Discord updates. If an icon stops being replaced, those selectors may need updating.
- The image files are loaded from the public [zoez22/muzzlemute repository](https://github.com/zoez22/muzzlemute).

## Credits

Based on the MutedToMuzzled BetterDiscord plugin by 1xzozz. Puppy icon assets are hosted by [zoez22/muzzlemute](https://github.com/zoez22/muzzlemute).
