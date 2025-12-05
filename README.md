# elgeis-resourcepack
Crowdsourced resource pack for the one and only **Elgeis Minecraft Server**!

Allows community members to add custom textures to be displayed for items renamed to specific text

Requires Optifine (or something like the CIT Resewn mod for non Optifine clients) to work properly - without it nothing will break, you just won't see changed textures!

# Rules for Contributing
- All changed textures are through the Optifine CIT system, see documentation: https://optifine.readthedocs.io/cit.html
- If you are thinking about doing something extra like adding an enchantment glint or other conditions listed in the CIT documentation above, we'd prefer you didn't, but check with a staff member first if it's really that important.
- Do not make changes to any default MC textures, only renamable custom items through Optifine CIT as seen above
- Only do this to "your own stuff", e.g. don't make a retexture for "Montrosian Standard-Issue Sword" without the approval of the people who make such items
- For example, if making changes to a Brewery recipe's texture, you must have the approval of the person who originally contributed the recipe
- Textures should be purely cosmetic & not deceptive or used for ingame advantage i.e. no making dirt look like diamonds in order to trick people or somesuch
- Harmful or disruptive additions to the pack may result in your removal from the community, so best behavior please!
- Staff reserve the right to reject contributions or request revisions if such contributions fall afoul of these rules or general good-faith participation.

# The Simple Tutorial

The purpose of this tutorial is to add a texture to a renamed item - for example, renaming a totem to "Goatem of Undying" will result in the goatem.png texture being displayed for that item.

*A sample setup for "Goatem of Undying" is provided for your reference at [assets/minecraft/optifine/cit/goatem](https://github.com/Fishbowl1864/elgeis-resourcepack/tree/main/assets/minecraft/optifine/cit/goatem)*

1. Create a folder for each item you wish to retexture inside [assets/minecraft/optifine/cit/](https://github.com/Fishbowl1864/elgeis-resourcepack/tree/main/assets/minecraft/optifine/cit). That folder should be named the custom name or a shorthand (for housekeeping).
2. Inside that folder provide a *(32x32 or smaller)* icon for the texture, named the same as your folder (for simplicity).
3. Also inside that folder, create a file with the name of the item you want replaced and suffix .properties (e.g. totem_of_undying.properties)
4. The .properties file should contain the following 3 lines (without the brackets):
   
    type=item
   
    matchItems=minecraft:\[item you want retextured\]
    
    texture=\[your texture\].png
   
    nbt.display.Name=\[Your Name\]
    

    **For example, the Goatem of Undying's properties are:**

    type=item
   
    matchItems=minecraft:totem_of_undying
   
    texture=goatem.png
   
    nbt.display.Name=Goatem of Undying
   
6. Success! Submit your changes as a pull request and ask a staff member to check your work.
