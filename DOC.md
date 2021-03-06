# sbtool-mrmt
# documentation
last updated 2017-07-23 for version 0.1

## usage

The Minimalist Race Mod Template is NOT a mod. It is a suite of templates that I made initially just for my own uses. Please, enjoy using it and let me know if you run into any issues.

The tag used for search and replace, `.mrmtname.`, should be written including the periods on either side of the string. This should funtion identically in plaintext as it does in regex.

If you already have a functioning race mod you can skip [the base](#the-base) and go straight to [additional modules](#additional-modules).

You can observe an outline of the folder structure [here](#the-folder-structure).

### the base

The function of the base module is to select groups of features that can't be called by reference.
Image assets includes the humanoid sprite sheets, a ship for the intro mission, and the ai files as they are used in certain cases.
Text assets include your species file and any essential patches for the species to be playable.
Instructions are as follows:

1. Come to terms with the fact that you will never make anything remotely close to as cool as the Munari.

2. Make a copy of the base template you will be using, place it in your mods folder, and name it anything you want.

3. Within this copy search and replace the following as it appears in text files, file names, and folder names.
  * `.mrmtname.` with your species name. It is recomended that you use all lowercase alphanumeric characters and do not use spaces, hyphens, periods, or any other special characters.

4. Start your mod! All other modules included are optional.

> Base module based on the [Skittles Race Mod] by [Miss Skittles]. Distributed with permission.

### additional modules

#### npcs

The function of the npc module is to add your species to the most common npc types and to generation added by the MRMT Initialization mod.
Instructions are as follows:

1. Make a copy of 'mrmt-npcs'. It does not matter where you make it or what you call it as it is temporary.

2. Within this copy search and replace multiple different items appearing only in text files, not in any file or folder names.
  * `.mrmtname.` with the same name you chose for the base module search and replace.
  * `.mrmtgeartype.` with the name of the vanilla species whos clothing you would like to borrow.

3. If you do not want your species appearing as a certain npc type find the associated type in '/projectiles/spawner' and simply delete the .patch file. In the case of wanting to remove the Letheia ships crew from Frackin Universe you would also have to delete the '/objects' folder.

4. Copy the contents of your copy of 'mrmt-npcs' into the folder of your mod. Remove the old empty folder.

#### dialog options

The function of the dialog module is to add themed dialog to your species, lest they default to the default dialogs.
The vast majority of this text is ripped from vanilla assets.
Instructions are as follows:

1. Pick a dialog style.
  * Direct will duplicate all dialog from the vanilla species you choose. your species would be talk and be reffered to as a memeber of that vanilla species.
  * Rename will mimic the dialog of the species you choose replacing any references to self by species name with the species name of your choice.
  * Generic will mimic the dialog of the species you choose replacing any references to self by species name with pronouns when feasable and by the species name of your choice elsewise.
    * Generic and rename styles can be found inside the folder marked for that species.

2. Make a copy of the folder you choose. It does not matter where you make it or what you call it as it is temporary.

3. Within this copy search and replace multiple different items appearing only in text files, not in any file or folder names.
  * `.mrmtname.` with the same name you chose for the base module search and replace.
  * `.mrmttitlename.` with the name of your species written with proper capitalization, or however you want it presented.
  * `.mrmtcapname.` with the name of your species written in all caps.
  * `.mrmtdialtype.` with the name of the vanilla species whos dialog you would like to borrow.

4. Copy the contents of your copy of the dialog module into the folder of your mod. Remove the old empty folder.

#### object description

The function of the object description module is to add themed description text to your species, lest they default to the default desriptions.
The OOC module functions best when used in conjunction with [Role-Play Emotes]!
The entirety of this text is ripped from vanilla assets.
Instructions are as follows:

1. Pick an object description style.
  * Direct
    * Copy will duplicate all dialog from the vanilla species you choose. your species would be refered to as a memeber of that vanilla species.
    * Repeat will make every description the same string. Useful if you want your species to look at everything and go '...'.
  * OOC will mimic the default description for each object but with `((` and `))` on either side of it.
    * Full will use the regular description.
    * Short will use the object name.
  * Species will mimic the descriptions of the selected vanilla species. References to self are mixed, some are changed to your species name, some are unchanged leaving in the original species name. This is chosen depending on if the entity is actually refering to itself or its own species, OR looking at an object belonging to the base species.

2. Make a copy of the folder you choose. It does not matter where you make it or what you call it as it is temporary. **ADVANCED USAGE** Start with an OOC module then merge your selection on top of it opting to replace existing files. This way any missing links default to an OOC description.

3. Within this copy search and replace multiple different items appearing only in file text, not in any file or folder names.
  * `.mrmtname.` with the same name you chose for the base module search and replace.
  * `.mrmttitlename.` with the name of your species written with proper capitalization, or however you want it presented.
  * `.mrmtdialtype.` with the name of the vanilla species whos dialog you would like to borrow.
  * `.descstring.` with the text you would like your species to repeat on inspecting something, only used for 'repeat' style.

4. Copy the contents of your copy of the object description module into the folder of your mod. Remove the old empty folder.

> Description module generated with help from [Starbound Race Description Patcher - Compiler tool] by [GTG3000].

#### extras

Templates for dungeons and unique npcs will be released as a seperate project.

### the folder structure

* base templates
  * apex
  * avian
  * brew
  * floran
  * glitch
  * human
  * hylotl
  * novakid
* dialog options
  * direct
  * floranlike
    * generic
    * rename
  * glitchlike
    * generic
    * rename
* npcs
* object description options
  * direct
    * copy
    * repeat
  * floranlike
  * glitchlike
  * ooc
    * full
    * short

### licensing

Attribution is *not* required when publishing a project made with this template. It is still appreciated.

[Miss Skittles]: http://community.playstarbound.com/members/96422/

[Skittles Race Mod]: http://community.playstarbound.com/resources/956/

[Role-Play Emotes]: ../../../sbmod-rpemote

[GTG3000]: http://community.playstarbound.com/members/191401/

[Starbound Race Description Patcher - Compiler tool]: http://community.playstarbound.com/resources/4306/

---

@license MIT
@author IHCaTHB
