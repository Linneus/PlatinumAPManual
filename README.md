# PlatinumAPManual
A Manual Randomizer for Pokémon Platinum, for use with the [Archipelago Manual](https://github.com/ManualForArchipelago) Project.

![Giratina from the Platinum title screen, with the Pokémon Platinum logo above it. The logo reads "Pokémon Platinum AP Manual"](https://github.com/Linneus/PlatinumAPManual/blob/main/Giratina_PlatinumManual_Screen.png?raw=true)

# Archipelago Setup

Everything that follows is a guide written for those already familiar with both Archipelago and the Manual Project. If you are starting from no knowledge on either of those, start with [this guide](https://github.com/Linneus/PlatinumAPManual/blob/main/Full%20Archipelago%20Setup%20Guide.md).

If you already have an Archipelago install, and are at least moderately familiar with the Manual project, continue on.


## Patching and Randomizing Your ROM

Included with your download is two xdelta patches and the xdelta program.
Open xdeltaUI.exe, and then choose whether you’d like to play in the original 30FPS, or with the patched 60FPS game, then open the corresponding .xdelta file as your Patch, your Pokémon Platinum ROM (which must be a clean Rev 1, also known as 1.1, which is the most common variant of the game) as your Source File, and then you’ll select a spot to save your modified ROM in Output File. Be sure to add “.nds” to the name of the file. If you don’t do this, you’ll have to add the file extension after the fact.

![An image of the xDelta UI](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUjFKWcgVj2IERUmCoOjX-qn6nkTZgdOtJHUErtlpq2kZnp7Cnbx8SFlgkIT-wMIyirVOrTd_uVRcvW_DBI8aq70EgA9Z0KdQFNB7b9RwEH32Az2kS1IoSK0kww2mYw_VQ0rO24pj4s7-Z0yZhaVXJQlDG?key=QmhoNGvKP18WJBxH2sPV0g)

## 30FPS vs. 60FPS

The normal patch will leave the game unchanged compared to its original DS release. However, the 60FPS patch will speed up many sections and aspects of the game, most noticeable in making all battle animations much snappier. This is slightly more taxing on one’s computer, and certain areas (most noticeably Eterna Forest) struggle to maintain a constant framerate with this patch. The Super Rod, which requires very precise timing in 30FPS, becomes nearly unreactable in 60FPS as well.

## Downloading and Using the Randomizer

Next, a modified version of [Universal Pokémon Randomizer ZX](https://github.com/Ajarmar/universal-pokemon-randomizer-zx) is included with the download. Open the program with the launcher file. In the top right, click “Open ROM” and open your modified ROM.

![an image of the Universal Pokémon Randomizer ZX UI, showing "Support: Unofficial ROM"](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdYFKFQfgvMwvGgbo9k2qvpq6Ml5RRJI_WBcPipHJXbDgRhXartMlt5mWmQjCgu-6AC6C-MH0wXmEHlskqAokVm5DnlO_QvJzXHupBhlvOdMHJKK2Sr8epyUdAkXsyxyPgpylwrT9rH-bK2ff2uAjr1abE?key=QmhoNGvKP18WJBxH2sPV0g)

Given that you just opened a modified ROM, you can expect to see the red text and the “Unofficial ROM” support. From here, modify your settings just as you would with any randomizer! For the most part, any and all settings are entirely up to you, but I will discuss a few of them, both for what this Manual is built around and what you can expect from these settings.


## TM/HMs & Tutors

If you are randomizing TMs, you must keep Field Moves! Otherwise, you lose access to TM70 (Flash) and Flash is considered in-logic for this randomizer. Consider it like Rock Smash in Crystal. This has the side effect of keeping TM28 as Dig.
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXepAylS737ZsQsfB5k91BzSHxIqmaYZw4qeU3isu50Aq5nTDltf3TKxZ0DI1oo6GSb1lYb60G5LbVja1IZSCXj_R2IPCXFmUGrDPTUm0xvprO_vcfycxlmMj1X7itVqblwOXCCmn7rjt0HBBgCT-Xq7HrrL?key=QmhoNGvKP18WJBxH2sPV0g)

## Items

Randomizing items allows you to ignore just about all the filler items you receive through the Archipelago client and just treat the pickups in-game *as* your filler.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfPFucqGjpDGnRr20DZFAlYrbK3naEbsRlo_pflgNUtzSCVykoqHOa_y0yk-Hd5ch5ZELBGqkcDmzuP0t1_6y7jGSW9K5YW24JDa2Lk6Cseg7Ktx8YQqSBj7sh-PppvNe1gqHQk80fbNSVWlQkJaaJzMpcf?key=QmhoNGvKP18WJBxH2sPV0g)

Most importantly, not only will the "Ban Bad Items" option will remove things like mail and useless berries (which are not in the Manual’s item pool to begin with), but this modified program will ALSO prevent Plates from showing up anywhere in the game. Using this option will force you to rely only on Plates obtained from the AP Items Room, which will be more immersive for the Plate Hunt goal.

## Foe Pokémon

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfvc2Rx79Msajo_wYHefg5Ix6qDFlRCdboMD4dF0VTBkE3-pzI3CT4oWIXS4uhfgXDfqoFNERY7rh7aERDuCwCFFdA8yXT_Ln2hGBrj4viAmJgn2Runhn9MisdFXZLhVlF2DfiCTNlYV0hLGjBasoStT9ei?key=QmhoNGvKP18WJBxH2sPV0g)
These options will be the primary source of difficulty for you. Bear in mind that you could get sent as far as Stark Mountain, fighting trainers with Level 60 Pokémon, so be mindful of how difficult you want to make the game.

Raising the level of trainers is straightforward (you may want to raise the level of Wild Pokémon to compensate), and giving them fully evolved Pokémon will also make for a more consistently challenging game.

I’ve found that, above everything else, “Better Movesets” was one of the most consistently challenge-raising options I would encounter, as opponents would frequently have excellent moves to deal with me, even if I was ten or twenty levels higher than them.

Extra Pokémon and held items will only increase the difficulty from there. Lastly is Double Battle Mode, which is exactly what it implies; bear in mind that every trainer will have at least two Pokémon and be a double battle. (If you’ve played Emerald AP and tried to use the 100% Double Battle chance, you’ll understand why I explain this.)

Similarly, there are options for an easier game, so tailor the experience to what you desire! With just a few of these options bumped up, I’ve found that this is absolutely the hardest Pokémon game I’ve played in Archipelago.

## Saving your ROM

When you’re done, hit “Randomize (Save)” in the top right to name/save your newly randomized ROM somewhere. You may also consider using the “Save Settings” option to revisit your options easily in the future.
After saving, I would also recommend using the "Produce File" button to easily reproduce your ROM with the exact randomization in case of any issue that may require a new ROM or patch.

## Cheat Files

Blind trainers and experience modifiers (found in the yamls for the other Pokémon games) are handled with Action Replay cheat codes.
This randomizer is built for either **DeSmuME** or **EmuHawk**.

For DeSmuME, load your ROM and then go to **Tools > Cheats List** and add the Action Replay codes included in the **AR Codes.txt** file. These will persist whenever you load that particular ROM.

For EmuHawk, load your ROM and then go to **Tools > Cheats** and open one of the .cht files (Blind Trainers is bundled with them both). This will only persist for that session, and you'll have to reopen the cheats file every time you Reboot Core.

# Using the Manual

## Opening the Launcher

All releases will have a link to the Archipelago Manual APWorld and Universal Tracker. If you have those downloaded and in your custom worlds folder, begin by making sure that the YAML you used for generation is currently in the Players folder. Then, navigate to your Archipelago install, open ArchipelagoLauncher.exe, and then from that, open the Manual Client on the right side. Select the name of the Manual in the dropdown list (Manual_PokemonPlatinum_Linneus), your room's code and, when prompted, your slot name.

## Sending and receiving Locations and Items

Sending checks is done by clicking on the corresponding buttons in the client. The buttons will not work unless you are clicked into the client's window.

![The Archipelago Launcher, with the Manual Client highlighted.](https://i.imgur.com/yUZD5xL.png)
![The Manual Client with Platinum loaded.](https://i.imgur.com/8laRClc.png)

Located in the basements of all 18 Pokémon Centers is the AP Items Room. Cross-reference with the left side of the Manual Client and pick up items there throughout your playthrough.

![The Pokémon Center escalator](https://i.imgur.com/XUBgXfd.png)
![The AP Items Room](https://i.imgur.com/t4v6TGS.png)

If the player is only in need of a Progression Item needed to proceed in the game, press the R Button to bring up the AP PDA menu, and select an item at virtually any time.

![A menu with options for Key Items, HMs, Badges, Pokétch, Pokédex, and Berries is on the screen on Route 205. A text box reads "Hello! AP Items Room here. What category are you looking into?"](https://i.imgur.com/hAkRTQK.png)
