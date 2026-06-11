# spiral_knights_tracking
a place to collect all the stuff for Spiral Knights, in json form.  

This json is a new project in the works to keep a singular collective location for any tools that may want to access the current items in the game that are able to be possessed by players. even the ones that are no longer obtainable, but remain in the games code, as a historical collection.  
  
the intent behind this json is to collectively add every single item in the game to create a simple one stop shop for any app or tool that may need to reference data for anything that exists within Spiral Knights. the games main page can be found here:   
the main game site: https://www.spiralknights.com/  
the wiki: https://wiki.spiralknights.com/Main_Page  
the forums: https://forums.spiralknights.com/en/forum/15  
the steam page: https://store.steampowered.com/app/99900/Spiral_Knights/  

why:  
this json file is the result of me creating an item tracking app in Godot engine, to be used as a standalone companion app, to help players in tracking their collections as they play the game.  
though as i get deeper into the project, and the more things i add, the more in depth the data keeps getting, so i need a way to drive all this information cleanly.  
the wiki is great, however it is not always current, and it is not ideal for an app to ping the wiki to scrape data constantly.  
you can find the beta release here: https://github.com/Tranzorro/spiral_knights_tracking/releases/tag/DST-beta-release  or by clicking the release tags to the right of this page.
  
what to do:  
it's a json, if you feel there is information missing, or the format needs adjusting, i encourage you to add on to it.  
at the top of the json is a template that shows what options are available to use for the datasets that currently exist within my tracker app. (linked above when available)  
these booleans will help track what item comes from which source, what its category is, how much the recipe costs, alchmey crafts cost, materials needed, all that.  
this template at the top also is intended to be universal, so it will still work the same for the battle sprites, their skills, materials, all use the same structured formatting.  
if any piece of the template doesnt apply to the entry you are adding, then simply leave out that portion, it won't break anything.  
of course, try not to leave a bunch of empty defaults in your entry, if you have trouble figuring out how an item entry should look, try copy pasting an existing one, and replacing the data.  
  
if a value for a boolean is false, like "bound: false" you can simply leave it out. all missing values will be assumed false by default.  

what not to do:  
don't: make entries that are false.   
  
don't: add a recpie as its own entry, this is implied on the item it will craft if it has one.  
  
don't: make entries about an npc on its own. the npc can be referenced as shown in the template, and on the items that already exist.  
  
don't: add non inventory items. these entries are meant to be things the player was meant to be able to collect, it goes into your inventory. that means, costumes, battle sprites, materials, armors, weapons, rarities, recipes etc.  
  
don't: use fake links in the wiki link slot. any contributions attempting to do so will be ignored and any future contribution attempts from you will be ignored as well. i'm trusting you not to bung up a data set with trolls or nepharious links.  
