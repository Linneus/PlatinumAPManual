# Downloading and Installing Archipelago, AP Manual, Universal Tracker, and the Platinum Manual

Archipelago (often abbreviated as 'AP') is a multiworld randomizer project designed to randomize different games together, but also functions as a hub for individual randomizers. Further information can be found on [their website, archipelago.gg](https://archipelago.gg/).

They have their own [setup guide found here](https://archipelago.gg/tutorial/Archipelago/setup/en), and I'd suggest following that (especially if you have interest in the greater scope of AP randomizers), but I'll be making a guide here specifically for the purposes of playing this Manual Platinum Randomizer.

"Manual for Archipelago" is a separate project that creates a simple form factor for structuring a randomizer without needing a full understanding of software development. They have [their own GitHub](https://github.com/ManualForArchipelago/Manual/), and all info on the project is contained within [their Discord server, along with all of the Manual projects](https://discord.gg/8AS8XgyzBk).

1. First, [download the latest version of Archipelago and install it](https://github.com/ArchipelagoMW/Archipelago/releases/latest). 

![Archipelago Installation](https://i.imgur.com/AhIjpJd.png)

2. Making a shortcut to the Archipelago folder during installation will make it easy to refer back to it throughout setup. Regardless, on Windows, your Archipelago install will default to **C:\ProgramData\Archipelago**. 

![The "Archipelago Folder" shortcut](https://i.imgur.com/xWlGU2g.png)

3. Next, [download the latest version of Manual](https://github.com/ManualForArchipelago/Manual/releases/latest). 

![An example of a Manual APWorld release](https://i.imgur.com/AyPfxot.png)

4. And [download the latest version of Universal Tracker](https://github.com/FarisTheAncient/Archipelago/releases/latest). 

![An example of a Universal Tracker APWorld release](https://i.imgur.com/WbRM7g8.png)

5. These are APWorld files, which give Archipelago its functionalities. They go in the "custom worlds" folder of your Archipelago install. 

![AP's 'custom worlds' folder](https://i.imgur.com/rtZNZeU.png)

6. Lastly, from this own project, [download the latest version of the PlatinumAPManual](https://github.com/Linneus/PlatinumAPManual/releases/latest). 

![This project's 2.1 release](https://i.imgur.com/LGZOhYk.png)

These are all of the pieces necessary to start playing. Well... aside from a Platinum v1.1 ROM and a way to play it. But you can figure that part out, can't you?

# Generating a seed

Within the PlatinumAPManual zip file is...

APWorld and YAML
- `manual_pokemonplatinum_linneus.apworld`
- `Manual_PokemonPlatinum_Linneus.yaml`

`UP Randomizer ZX Edit`, `.cht` files, `AR Codes.txt`, `.xdelta` files, and the xDelta program.

1. Put the .apworld in the custom worlds folder along with the Manual and Tracker from earlier. 

![The APWorlds in the custom worlds folder](https://i.imgur.com/hrECr85.png)

2. Using [the guide on the main page](https://github.com/Linneus/PlatinumAPManual/blob/main/README.md)...
   - Make a patched ROM for yourself.
   - Randomize that ROM with the Universal Pokémon Randomizer ZX edit. 

![UP Randomizer ZX having just successfully randomized a ROM](https://i.imgur.com/EEcIbtW.png)

3. Now, to create settings for any AP randomizer, a settings file in the `.yaml` format/language must be made so that you can decide how you'd like your game to be randomized. These settings files are referred to as "YAMLs", given their language, and they all have a template for you to work from. As an aside, it would be good practice to tell you how to generate your own templates:
   - Open `ArchipelagoLauncher.exe` and click the "Generate Template Options" button. This will make a folder of template YAMLs for every AP World you have installed (bear in mind that your Archipelago install comes with a number of supported games). 
   - The aforementioned `Manual_PokemonPlatinum_Linneus.yaml` included in your download is identical to what you can generate yourself, so feel free to work off of that. 

![The 'Generate Template Options' button in the Launcher highlighted.](https://i.imgur.com/ROkN11f.png)

4. Open the YAML in your preferred plain text editor (the following screenshots are taken in Notepad++, but regular Notepad will work fine for this).
   - There is an explanation at the top of the YAML explaining how to format your choices, but I'll go over that as well.
   - First and most importantly is your slot name. The randomizer will use this to refer to you as you play, and you have 16 characters (anything over that will be truncated). 

![I've inputted my name as 'Linneus'. In actuality, I always write something goofy.](https://i.imgur.com/9sFq99V.png)

   - Secondly, if there is any option you do not understand, feel free to skip it and leave it as is. 

![The 'filler traps' option. This one won't really do anything for this randomizer.](https://i.imgur.com/NVqeniR.png)

   - To 'choose' your settings, it's as simple as changing the numbers in front of the answers. By default, this formatting has `randomize_hidden_items` set to `'true'`. If you would like Hidden Items to _not_ be randomized, just change true to `0` and false to `50`.

![Hidden Items On](https://i.imgur.com/kxnbhkw.png)

![Hidden Items Off](https://i.imgur.com/HBg2f9m.png)

   - The reason for this formatting is that options themselves can be randomized. If you want the randomizer itself to decide what settings you have, referring back to our previous example, you can set both `true` _and_ `false` to `25`. If you put different numbers, this changes the odds. Consider that it's like placing marbles in a bag; if `true` is set to `40` and `false` is set to `60`, there are 40 'true' marbles and 60 'false' marbles in your bag, and you'll reach in and take one at random.
   - When you've got all the settings the way you'd like them, save the YAML (retain the `.yaml` File Extension, but feel free to name the file whatever you like). It then needs to be placed in the Players folder in your Archipelago install. 

![My YAML, with all of my favorite settings.](https://i.imgur.com/Xej21Zb.png)

5. From here, you can generate a game. Run `ArchipelagoGenerate.exe`.
   - IMPORTANT: This will make a _single_ game for _all_ of the YAMLs currently in your Players folder. (This does not include subfolders.) If you place two YAMLs in the folder, you will generate a multiworld, where the items are shuffled between the games. Make sure that only the YAMLs for the games you intend to generate (or the single YAML if you are playing a single game) are in the Players folder.
   - This will make a .zip file in the output folder. If this folder did not exist, it will be created. 

![My generated seed data](https://i.imgur.com/8tDSSkb.png)
  
# Playing the game

1. To play the generated game, a 'room' must be hosted for it. There are two ways to do this:
   - Option 1: Go to the [Archipelago website's "Host Game" page](https://archipelago.gg/uploads). Upload your .zip file and press "Create New Room". Take note of the `archipelago.gg:` code on this page. This is your server port, and will be used shortly. 

![A generated room on archipelago.gg](https://i.imgur.com/P6v2Gtz.png)

   - Option 2: Locate `ArchipelagoServer.exe` in your Archipelago folder and run it. You will be prompted for a .zip file; provide the one in your output folder that you created. Take note of the `[::]:` number on this screen. This is your server port, and will be used shortly. 

![The localhost window](https://i.imgur.com/JONjI9a.png)

2. For this Manual, run `ArchipelagoLauncher.exe` again and open the Manual Client (located on the right side). In the server section, if you hosted on the website, write `archipelago.gg:` followed by your port number. If you hosted using `ArchipelagoServer.exe`, make sure that the window is still open and write `localhost:` followed by your port number. 

![The Archipelago Launcher, with the Manual Client highlighted.](https://i.imgur.com/14c2HMN.png)

![Entering server ports in the Manual client](https://i.imgur.com/02ClqO6.png)

3. You will be prompted for your slot name, which you set in your YAML, so type that in. 

![Entering my very normal slot name, as I wrote earlier](https://i.imgur.com/YPdLbqG.png)

4. The Manual client is now running! As long as the YAML you used to make this seed was still in the Players folder when you opened the client, you will be able to track your progress as you play.
5. Open and set up your emulator of choice, [as gone over here in the main guide](https://github.com/Linneus/PlatinumAPManual#cheat-files), and run the game.
6. Now, as you play, simply click the buttons in the `Manual` tab in your client to mark your progress as you make it in game! 

![Picking up the hidden item in front of Jubilife City and clicking the corresponding button](https://i.imgur.com/63LH0sd.png)

7. In the `All` and `Archipelago` tabs, you will be told what you told what you've received. 

![Pro tip: Open the Launcher and open a separate Text Client so you don't have to keep switching tabs.](https://i.imgur.com/E50D4Nu.png)

8. To get your items in-game, visit the AP Items Room, located in the basement of every Pokémon Center. 

![Picking up the aforementioned Hyper Potion in the AP Items Room](https://i.imgur.com/V37Oheo.png)

This should cover everything needed! Repeat any steps as needed to generate more games, and keep an eye on this GitHub for future updates!
