# Roll20 NPC Importer, for 5e OGL
A module for FoundryVTT, used to import DND5e NPC sheets from the popular Roll20 application.
Only works for 5e NPC characters that use the OGL sheet version.

Download and put the roll20npcimporter folder into FoundryVTT/public/modules

Instructions to import NPCs from Roll20:
1. Have the browser plugin VTT Enhancement Suit (https://ssstormy.github.io/roll20-enhancement-suite/features.html)
2. Open the Roll20 game containing the NPC and open the sheet
3. Use the export function in the "Export and Overwrite" tab
4. Select the .json file(s) you wish to import
5. press import


Advanced Options:
- Legendary Action and Reaction Prefix
   - Sets a Prefix for those 2 types of Features to distinguish them from regular Features since Foundry doesnt have seperate Items for them yet
- Default HP
   - A fallback HP value. If A regular HP cant be found the importer first trys to roll the HP Formula, if that also fails, this Default HP will be used
- Default Source
  - Sets a Value forthe Source of the Actor
- Display Options for Token Nameplate and Bars
- Bar 1 and Bar 2 Attribute
   - By default the Importer will put the token values into value and max value for bar 1 and 2. If either one is set to HP this will be ignored and the HP will be used for the corresponding bar.
- Compendium Integration
   - You can choose to import an Actor either as a regular Actor into the Actor List or into a Compendium. If you want to Import into a compendium you have to choose a Compendium from the list. It only lists Actor compendiums that are local to the World and ignores Compendie outside of the World folder.
   - You can choose a Spell Compendium if you want. This will allow the Importer to pull a spell from the chosen compendium (if found) instead of creating a new Spell. This way you can use the preformated and icon'd Spells instead of Spells containing unformated, raw text. If a spell can't be found it will still create the spell, so you do not lose any spells. 

Shaped Charactersheet Support is currently in beta, for anything missed or not correctly imported, contact me in discord (Felix#6196) or per email (syl3r31@gmail.com). Make sure to include the .json file of the character that has the issue.

Planed features for the future:
- Fallback in case a spellcasting npc has no spellslot information saved


Big thanks to Atropos for troubleshooting and Sillvva for providing a good example with the DNDBeyond importer.

If you feel like supporting my work, feel free to leave a tip at my paypal felix.mueller.86@web.de
