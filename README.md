# elgeis-resourcepack
Crowdsourced resource pack for Elgeis Minecraft Server

Requires Optifine (or something like the CIT Resewn mod for non Optifine clients) to work properly - without it nothing will break, you just won't see changed textures!

To start us off, an example texture "Goatem of Undying" is provided for reference.

# Rules for Contributing
- All changed textures are through the Optifine CIT system, see documentation: https://optifine.readthedocs.io/cit.html
- Do not make changes to any default MC textures, only renamable custom items throught Optifine CIT as seen above
- Only do this to "your own stuff", e.g. don't make a retexture for "Montrosian Standard-Issue Sword" without the approval of the people who make such items
- For example, if making changes to a Brewery recipe's texture, you must have the approval of the person who originally contributed the recipe
- Harmful or disruptive additions to the pack may result in your removal from the community, so best behavior please!
- Staff reserve the right to reject contributions or request revisions if such contributions fall afoul of these rules or general good-faith participation.

# The Simple Tutorial

*A sample "Goatem of Undying" is provided for your reference at assets/minecraft/optifine/cit/goatem*

1. Create a folder for each item you wish to retexture inside assets/minecraft/optifine/cit/. That folder should be named the custom name or a shorthand (for housekeeping).
2. Inside that folder provide a (reasonably sized) icon for the texture, named the same as your folder (for simplicity).
3. Also inside that folder, create a file with the name of the item you want replaced and suffix .properties (e.g. totem_of_undying.properties)
4. The .properties file should contain the following 3 lines (without the brackets):
    type=item
   
    matchItems=minecraft:<item you want retextured>
    
    texture=<your texture>.png
   
    nbt.display.Name=<Your Name>
    
.

    **For example, the Goatem of Undying's properties are:**

    type=item
   
    matchItems=minecraft:totem_of_undying
   
    texture=goatem.png
   
    nbt.display.Name=Goatem of Undying
   
6. Success! Submit your changes as a pull request and ask a staff member to check your work.
