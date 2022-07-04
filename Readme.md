In the startup options for steam use the following `swfoc MODPATH=Mods\Caspar`

For adding units do the following:
   1. Download the XML Files from https://www.gamemaps.com/foc/tools
   2. Add your unit to the XML Files
      1. For example C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\XML\UNIQUEUNITS.XML
   1. Add Text and descriptions using the dat Editor http://www.petrolution.net/item-172
       1. Use the file located in "C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\Text\mastertextfile_english.dat"
   2. Add the image for the unit
       1. Get the textures from the base game using the Eaw_file_Extractor https://www.moddb.com/downloads/eaw-file-extractor
       2. Use the file "C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Data\textures.meg" for force of curruption
       3. Obtain an .tga file for the icon
       4. Uing the MED Editor open the MT_COMMANDBAR.MTD file in C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\ART\TEXTURES
       5. There open MT_COMMANDBAR.TGA.
       6. Add the image you want to use
   3. Now make the unit available in galactic conquest and skyrimish
   4. Skyrimish
       1. Open C:\Program Files (x86)\Steam\steamapps\common\Star Wars Empire at War\corruption\Mods\Source\Data\XML\STARBASES.XML
       2. Go to Skirmish_Empire_Star_Base_3 or whatever base you want to use
       3. Add it to Tactical_Buildable_Objects_Multiplayer
       4. Add for all starbases afterwards
   5. For adding to galactic conquest
       1. For the AI
          1. Open STORY_EMPIRE_AI_HEROES_EXP.XML
          2. Make a new event at the tech level for example 
       2. For the player
          1. Find the file you need to edit in CAMPAIGNS_UNDERWORLD_GC.XML
          2. For example search for `<Campaign Name="Sandbox_Equal_Footing_Empire">`
          3. Find the Empire_Story_Name tag
          4. Open the corresponding file, for example STORY_SANDBOX_56_EMPIRE.XML
          5. Add the entry under <!-- Spawn Tech Level 1 Heroes -->
   6. You're done, have fun!
       
