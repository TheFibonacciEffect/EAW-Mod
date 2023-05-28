This is a mod for the game Star Wars Empire at War - Force of Corruption


# Units Added
- Reprisal Star Destroyer
  - Star Destroyer of Admiral Ozzel
- 501 Legion
  - Has doubble the firerate of ordinary stormtroopers and the ability to sprint
- Eli Vanto
  - Aid of Leutanant Thrawn
  - Redruces Price of Tartan Patrol Cruisers
  - Gives a slight movement speed bonus in combat
  - Reduces Production Time for Vehicles by half
  - Reduces Production time for Tartan Patrol Cruisers by 75%
  - Also appears in Campaign Equal footing in Era 3
- Emperor Palpetine
  - Emperor Palpetine now comes with two imperial Guards
- Jedi Outlaw
  - to balance this out a bit the Rebels receive the ability to train jedis
  - based on luke skywalker
  - Can throw lightsaber
  - Buildable in Rebel command center
  - [ ] Adjust Texture
  - [ ] Make buildable in campaign, perferably only on certain planets like the cantina
  - [ ] Spaceship, use `Jedi_Cruiser`

# Installation
- Clone/download the repository.
- Create a new directory inside your Steam copy of FoC's "Mods" folder (e.g.: "\corruption\Mods\UFoCP1.0")
- Create a subdirectory "<modname>/Data/"
- Paste repository contents into Data folder.
- Launch the Steam copy of FoC with the launch option "MODPATH=Mods\##Folder Name##."

# Contributing
Just do a Pull Request or open an Issue, everything is welcome and I am glad to help within my capabilities
If you change any binaries in your pull request or branch, write [binaries changed] into the branch name.
## How to add a simple unit in Empire at War using XML
Place all your stuff into `C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods`, if the `Mods` Folder does not exist, create it. In unix the files can be found under `/home/caspar/local/share/Steam`
For adding units do the following:
   1. Download the XML Files from https://www.gamemaps.com/foc/tools
   2. Add your unit to the XML Files
      1. For example C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\XML\UNIQUEUNITS.XML
      2. if it is a hero, set the techlevel to 6 or higher
      3. If you changed the abilities, you may need to change the `<LandBehavior>` tag and add `ABILITY_COUNTDOWN` for example
      4. For ground units, you have to edit the container, team and company (for example GroundInfantry, Container, HeroCompany for 501)
   3. Add Text and descriptions using the dat Editor http://www.petrolution.net/item-172
       1. Use the file located in "C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\Text\mastertextfile_english.dat"
   4. Add the image for the unit
       1. Get the textures from the base game using the Eaw_file_Extractor https://www.moddb.com/downloads/eaw-file-extractor
       2. Use the file "C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Data\textures.meg" for force of curruption
       3. Obtain an .tga file for the icon
          1. Use GIMP
          2. Get some Picture from the internet (make sure you have the rights to use it)
          3. (Put a vigniette on the image, use `Filters → Light and Shadow → Vignette` and use transparent color)
          4. Scale it to 50x50 pixels, use `Image>Scale Image`
          5. Save as .tga
       4. Uing the MED Editor open the MT_COMMANDBAR.MTD file in C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\ART\TEXTURES
       5. There open MT_COMMANDBAR.TGA.
       6. Add the image you want to use
   5. Now make the unit available in galactic conquest and skyrimish
   6. Skyrimish
       1. Open C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\XML\STARBASES.XML
       2. Go to Skirmish_Empire_Star_Base_3 or add it to `Imperial_Command_Center` in `XML\SPECIALSTRUCTURES.XML` whatever base you want to use
       3. Add it to `<Tactical_Buildable_Objects_Multiplayer>` tag
       4. Add for all starbases of higher level
   7. For adding to galactic conquest
       1. For the AI
          1. Open STORY_EMPIRE_AI_HEROES_EXP.XML
          2. Make a new event at the tech level for example 
       2. For the player
          1. Find the file you need to edit in CAMPAIGNS_UNDERWORLD_GC.XML
          2. For example search for `<Campaign Name="Sandbox_Equal_Footing_Empire">`
          3. Find the Empire_Story_Name tag
          4. Open the corresponding file, for example STORY_SANDBOX_56_EMPIRE.XML
          5. Add the entry under `<!-- Spawn Tech Level 1 Heroes -->`
   8. You're done, have fun!
