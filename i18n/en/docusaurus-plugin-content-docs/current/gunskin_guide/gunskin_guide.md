## Skin Resource Pack Creation Guide

## Before You Begin ##
Welcome to the tac skin resource pack creation guide from LesRaisins.

### Please note:  
1. This guide is not an art tutorial for texturing or modelling the skins themselves, but simply a document to help the reader to properly create gun models/textures, and to actualise the skins textures and models that have already been created into the game, and to avoid any dyslexia, please make sure that you have a good understanding of the basics of Resource Pack creation and the concepts involved in it when reading through the contents of this section; 
2. some pages and sections of this guide may be marked with a `legacy` symbol, which means that the content may not be applicable to the latest version of TaC, please refer to the corresponding page for details.  
3. Many of the example files in this guide are contained in the assets folder of TaC itself, so if you feel that this guide is not intuitive enough for you, you may want to open the source files directly to see them, which may help you understand them.

## Some notes
### About the model
The `complete model` of the gun that tac eventually presents in the game is a combination of a series of models from different files;  

For the purposes of this guide, we will refer to these models as `model parts` or `components`;  


## Making a gun skin
For information on how to get the source material right and start skinning, see [Section: Skinning Help](. /gunskin_guide/paint.md)

## Describe file format
To allow the module to read the gun skins in the resource pack, you need to add a json file to the resource pack to describe the skins.  
The specific path is
`assets/<namespace>/models/gunskin/skin.json`.  
You can put this file in any namespace you want, which will determine the namespace of your next skin. (where `<namespace>` for TaC is `tac`)

For details on `description files`, see [section: Description file format](. /gunskin_guide/description_file.md)


## Getting a skined gun
It's easy, `/give @s tac:ak47{Skin:"<skin namespace>:<skin identifier>"}`, you can leave out the namespace, it defaults to `tac`.
For example, if there is a skin for an ak, `skin.json` is placed in the `tac` namespace, such as the gold and silver ak in the above example.
is `/give @s tac:ak47{Skin: "golden"}` `/give @s tac:ak47{Skin: "tac:silver"}`
