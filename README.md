# Nine-Patch-Button-for-Godot-3.x

## What Is This?
A new type of node that combines the features of the NinePatchRect, the Button and the TextureButton, with the NinePatchRect being used as the base. We also took the liberty to add a custom sound system to the NinePatchButton, which allows you to assign sounds for pressing it, hovering over it, attempting to press it while it is disabled, and focusing it.

*Note: We've been having issues with getting text to display correctly on the NinePatchButton, so we've had to disable that feature for now. We'll revisit this at a later time. For now you could use a Label (or something similar) and add text to the button manually. If you can manage to integrate the text you want to display into the button's texture then that could work as well.*

## Why Did We Make This?
The Texture Button stretches the custom textures you add to it, which is especially noticable when trying to use pixel art. The NinePatchRect doesn't have this issue, so the sensible thing to do would be to use the NinePatchRect's method to add custom textures to our buttons instead, so we combined the features of the NinePatchRect with those of the Button. The TextureButton still had some good features though, so we added some of them into the mix as well, along with a our custom sound system.

## Usage Guide
To set up the NinePatchRect button texturing simply load your texture into

## Got Any Feedback?
If you have any feedback, be it a bug report or a suggestion, feel free to open an issue on GitHub. All we ask is that you try to label your issue suitably with the provided labels and that you try to prevent posting an issue about a topic that an issue already exists for. If an issue on that topic already exists, instead add on to that issue with a comment of your own.

We appreciate any kind of constructive feedback you can give us as it is important for us to know if something isn't working as expected or if you have any suggestions for us on how to improve the plugin.


## Future plans
- Fix the text display issue.
- Add the `Click Mask` property from the Texture Button to enable the user to set up their own click masks to fit their custom textures for the button.
- Add the `Flip H` property from the Texture Button, renamed to `Texture Flip H` for clarity.
- Add the `Flip V` property from the Texture Button, renamed to `Texture Flip V` for clarity.
- Add Texture Button-esque button texturing? It might not work... but it could be useful to have as an alternative to the already-implemented NinePatchRect-esque button texturing.
- Add [Conditional Export Properties](http://kehomsforge.com/tutorials/single/gdConditionalProperty)? It could be used for giving the option between using Texture Button-esque button texturing and NinePatchRect-esque button texturing without clogging up the Inspector. It would help make it more user-friendly, but would hugely increase the length of the plugin's script.
- Add exported properties to custom property groups? It would help make it more user-friendly and somewhat declog the Inspector, but would also increase the length of the plugin's script.
- Port the plugin to Godot 4, complete with a separate Asset Library page and GitHub repository. A link to the ported Godot 4 version of the plugin will be included here once it is done.

## Changelog:
### v2.0.0
- Initial public release of the plugin on the [Asset Library](https://godotengine.org/asset-library) as well as the setup of the GitHub repository and everything else that goes with those two things.

### v1.3.0
- Added a new custom `Focused Sound` property, based on the Texture Button's `Focused Texture` property.
- Added the `Focused Texture` property from the Texture Button.
- Added the `Action Mode` property from the Button.
- Fixed a typo in one of the properties.
- Fixed the default values of some properties that were mistakenly left undefined
- Removed the deprecated `Enabled Focus Mode` property from the Button (according to its own tooltip it is deprecated and scheduled for removal in Godot 4 anyways).
- Cleaned up the plugin's code.

### v1.2.1
- Fixed a bug.

### v1.2.0
- Added `tool` to the plugin's scripts to allow it to run in the editor.
- Removed the now-redundant `NinePatchButton.tscn`.

### v1.1.0
- Fixed a bug.
- Changed the names of the plugin's scripts.
- Cleaned up the plugin's code.

### v1.0.1
- Added a custom icon for the plugin.

### v1.0.0
- Initial private release of the plugin for in-house testing and development.
