# Roll20 NPC Importer, for 5e
A module for FoundryVTT, used to import DND5e NPC sheets from the popular Roll20 application.
Only works for 5e NPC characters that use the OGL or Shaped sheet version.

## Installation
1. Download the [roll20npcimporter.zip](https://github.com/syl3r86/roll20npcimporter/raw/master/roll20npcimporter.zip)
2. Unzip it into FoundryVTT/public/modules
3. Restart Foundry if it was running.

You'll see this button in the actors list after correctly installing the module.

![npc import button](https://i.imgur.com/EN6a9Ho.png)

If it doesn't show up make sure you are the GM of the game. If you are, and it still won't show up, feel free to contact me.
A common misconception is that the FVTT Enhancement Suit by Sillvva adds an import and export button as well, but these do not work with Data from Roll20. 

## Instructions to import NPCs from Roll20
1. Have the browser plugin VTT Enhancement Suit (https://ssstormy.github.io/roll20-enhancement-suite/features.html)
2. Open the Roll20 game containing the NPC and open the sheet
3. Use the export function in the "Export and Overwrite" tab
4. Select the .json file(s) you wish to import
5. press import


## Advanced Options
- Legendary Action and Reaction Prefix
   - Sets a Prefix for those 2 types of Features to distinguish them from regular Features since Foundry doesnt have seperate Items for them yet
- Default HP
   - A fallback HP value. If A regular HP cant be found the importer first trys to roll the HP Formula, if that also fails, this Default HP will be used
- Default Source
  - Sets a Value forthe Source of the Actor
- Use TokenImage as Avatar
   - this option will overwrite the default Avatar picture with the picture used for the token
- Use Images from public folder
   - If you want to use token or avatar images that you already have somewhere in your public folder, you can use them instead of the images that are defined in the imported data.
   - Avatar and Token Image Path
      - This is where you define where the images are stored that you want to use. You can use @name to use the actors name as part of the Path or Filename.
- Display Options for Token Nameplate and Bars
   - Ignore Token Lighting
      - lets you ignore light data from the roll20 token if you prefere your tokens to be blind
   - Bar 1 and Bar 2 Attribute
      - By default the Importer will put the token values into value and max value for bar 1 and 2. If either one is set to HP this will be ignored and the HP will be used for the corresponding bar.
- Compendium Integration
   - You can choose to import an Actor either as a regular Actor into the Actor List or into a Compendium. If you want to Import into a compendium you have to choose a Compendium from the list. It only lists Actor compendiums that are local to the World and ignores Compendie outside of the World folder.
   - You can choose a Spell Compendium if you want. This will allow the Importer to pull a spell from the chosen compendium (if found) instead of creating a new Spell. This way you can use the preformated and icon'd Spells instead of Spells containing unformated, raw text. If a spell can't be found it will still create the spell, so you do not lose any spells. 

If you encounter any issues, contact me in discord (Felix#6196) or per email (syl3r31@gmail.com). Make sure to include the .json file of the character that causes the issue, if applicable.

## Contribution
Big thanks to Atropos for troubleshooting and Sillvva for providing a good example with the DNDBeyond importer.

If you feel like supporting my work, feel free to leave a tip at my paypal felix.mueller.86@web.de

## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Roll20 NPC Importer - a module for Foundry VTT -</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/syl3r86?tab=repositories" property="cc:attributionName" rel="cc:attributionURL">Felix</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

This work is licensed under Foundry Virtual Tabletop [EULA - Limited License Agreement for module development v 0.1.6](http://foundryvtt.com/pages/license.html).
