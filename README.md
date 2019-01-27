# Roll20 NPC Importer
A module for FoundryVTT, used to import DND5e NPC sheets from the popular Roll20 application

Download and put the roll20npcimporter folder into FoundryVTT/public/modules

Instructions to import NPCs from Roll20:
1. Have the browser plugin VTT Enhancement Suit (https://ssstormy.github.io/roll20-enhancement-suite/features.html)
2. Open the Roll20 game containing the NPC and open the sheet
3. Use the export function in the "Export and Overwrite" tab
4. Post the contents of the downloaded .json file
5. press import

Big thanks to Atropos for troubleshooting and Sillvva for providing a good example with the DNDBeyond importer.

Known shortcomings to be fixed in the future:
- improvement on the senses/passive perception display
- proper cleaning of the Monstertype string
- importing directly into a compendium
