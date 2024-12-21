Vanilla Tooltips
================

A [MonkeyLoader](https://github.com/MonkeyModdingTroop/MonkeyLoader) mod for
[Resonite](https://resonite.com) that adds Tooltip label data for the vanilla UI.


## Install

First, make sure you've installed MonkeyLoader and the necessary GamePacks - combined releases can be found on the page of the Resonite GamePack here: https://github.com/ResoniteModdingGroup/MonkeyLoader.GamePacks.Resonite/releases/

Then all you have to do is placing the provided `VanillaTooltips.nupkg` into your `Resonite/MonkeyLoader/Mods/` folder.  


## Contributing

To contribute, simply fork this repository and add or modify the correct
`Locale/*.json` file for your language.
Start a draft pull request as soon as you created a commit in your repository
so that other people can see what changes are already being worked on.
The file format and requirements work exactly like they do on the
[Yellow-Dog-Man/Locale](https://github.com/Yellow-Dog-Man/Locale) repository.

### Finding the Locale Key

To find out which locale key you need to use for a given button in the Resonite UI,
simply toggle on the tooltip debugging data option in the Resonite Game Pack settings.
Any not yet defined but supported buttons will then show the necessary locale key
(e.g. `Tooltip.Slot.ResetScale`) as a tooltip instead of nothing.  
Any useful data that could be included in the tooltip is also written to
the log at Debug level when this option is enabled.
It is advisable to use enable the logging console for this to avoid having to dig through the file.

The tooltip locale key has the format: `Tooltip.{TypeName}.{MethodName}` for all OnPressed actions.