# MutedToMuzzled (PupCord)

A Vencord **QuickCSS stylesheet**, not a standalone Vencord plugin. It replaces Discord's voice-control icons and wording with puppy-themed assets.

## Icon mapping

- **Microphone enabled:** `bark.png`
- **Microphone muted, server-muted, or blocked by channel permissions:** `dog.png` (Muzz)
- **Listening / headphones enabled:** `cage2.png` (open cage)
- **Deafen enabled:** `cage.png` (closed cage)
- **Participant status icons:** applies Muzz to regular microphone mute and server/permission mute; applies the closed cage only to the crossed-out headset icon.
- **Tooltips:** `Bark!!`, `Muzzled`, `Cage`, and `Caged`.
- **Typing indicator:** uses barking-themed wording.

The local button selectors are scoped to the user-panel voice controls instead of every matching button across Discord. This helps avoid changing camera or call controls when the webcam is enabled. Discord's markup can still change between releases.

## Install

1. Open **Discord Settings → Vencord → Themes → Edit QuickCSS**.
2. Put this import at the very top of your QuickCSS file:

   ```css
   @import url("https://raw.githubusercontent.com/djdenicore/MutedToMuzzledVencordPort-Fix/master/MutedToMuzzled.css");
   ```

3. Save the file and reload Discord if the changes are not visible.

## Compatibility notes

- Uses modern CSS features, including `:has()`, `:is()`, and CSS nesting.
- Discord class names and SVG paths may change after updates. If a particular status icon stops being replaced, the relevant selector may need updating.
- Icon assets are hosted in the public [zoez22/muzzlemute repository](https://github.com/zoez22/muzzlemute).

## Credits

Based on the MutedToMuzzled BetterDiscord plugin by 1xzozz. Puppy icon assets are hosted by [zoez22/muzzlemute](https://github.com/zoez22/muzzlemute).
