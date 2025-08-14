## Obsidian TTRPG Tools

This project is a collection of code and templates I've created in an effort to automate building a TTRPG content library with Obsidian. 

## Prerequisites and Assumptions

We're beginning with the assumption that you already have some basic experience using Obsidian including installing Community plug-ins. 

### Required Plug-Ins

This project uses the following list of Obsidian Community plug-ins. 

+ [Modal Forms](https://github.com/danielo515/obsidian-modal-form)
+ [Templater](https://github.com/SilentVoid13/Templater)
+ [Quick Add](https://github.com/chhoumann/quickadd)
+ [Dataview](https://blacksmithgu.github.io/obsidian-dataview/)

**Modal Forms** generates user input forms to capture TTRPG data and convert it to a note in Obsidian. 
**Templater** essentially maps individual template files to a specific folder location (for example, the NPC template file to the NPC folder.)
**Quick Add** is used to launch the modal form and kick off the whole workflow.
**Dataview** translates inline variables within the template file to the values captured from the form. 

*Optional* Once you have this workflow functioning, you can enhance it with a plug-in like [Meta Bind](https://github.com/mProjectsCode/obsidian-meta-bind-plugin) to create a button that calls the Quick Add command from inside a note. 

### Directory Structure

You are welcome to structure the folders in your vault to your preference, but you will need to adjust some of the files contained here to match your changes. Below is a portion of the directory structure in my vault for your reference. 

+ MECHANICS
++ Beastiary
++ NPCs
++ Strategy
+++ Dangers
++++ Hazards
++++ Obstacles
++++ Terrain
++++ Traps
+ Z_ASSETS
++ Global Templates
+++ _ModalForm-NewNaturalDanger.md_
+++ _ModalForm-NewNPC.md_
+++ _ModalForm-NewObstacle.md_
+++ _ModalForm-NewTrap.md_

### Templates

**ModalForm-NewNaturalDanger** This template is used to generate two types of notes - Hazards or Dangerous Terrain. 
**ModalForm-NewNPC** This template is used to generate NPC notes. 
**ModalForm-NewObstacle** This template is used to generate notes pertaining to Obstacles in the party's path. 
**ModalForm-NewTrap** This template is used to generate notes about Traps. 