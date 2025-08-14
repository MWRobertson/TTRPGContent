## Obsidian TTRPG Tools

This project is a collection of code and templates I've created in an effort to automate building a TTRPG content library with Obsidian. 

## Prerequisites and Assumptions

We're beginning with the assumption that you already have some basic experience using Obsidian including installing Community plug-ins. While it may not be strictly necessary to read through and understand the JSON data files contained here to implement these tools, a general knowledge of JSON formatting would be helpful in the event that any of these files need to be modified to fit your environment. 

### Required Plug-Ins

This project uses the following list of Obsidian Community plug-ins. 

+ [Modal Forms](https://github.com/danielo515/obsidian-modal-form)
+ [Templater](https://github.com/SilentVoid13/Templater)
+ [Quick Add](https://github.com/chhoumann/quickadd)
+ [Dataview](https://blacksmithgu.github.io/obsidian-dataview/)
+ [Columns](https://github.com/tnichols217/obsidian-columns)

**Modal Forms** generates user input forms to capture TTRPG data and convert it to a note in Obsidian. 
**Templater** essentially maps individual template files to a specific folder location (for example, the NPC template file to the NPC folder.)
**Quick Add** is used to launch the modal form and kick off the whole workflow.
**Dataview** translates inline variables within the template file to the values captured from the form. 
**Columns** is just used in the formatting of finished notes. As the name implies, it adds ability to create separate columns in a note. 

*Optional* Once you have this workflow functioning, you can enhance it with a plug-in like [Meta Bind](https://github.com/mProjectsCode/obsidian-meta-bind-plugin) to create a button that calls a Quick Add command. These buttons can be added to a note to create a dashboard for launching forms. 

### Directory Structure

You are welcome to structure the folders in your vault to your preference, but you will need to adjust some of the files contained here to match your changes. Below is a portion of the directory structure in my vault for your reference. 

+ MECHANICS
    + Beastiary
    + NPCs
    + Strategy
        + Dangers
        + Hazards
        + Obstacles
        + Terrain
        + Traps
+ Z_ASSETS
    + Global Templates
        + _ModalForm-NewNaturalDanger.md_
        + _ModalForm-NewNPC.md_
        + _ModalForm-NewObstacle.md_
        + _ModalForm-NewTrap.md_

### Templates

**TEMPLATE-NewNaturalDanger** This template is used to generate two types of notes - Hazards or Dangerous Terrain. 
**TEMPLATE-NewNPC** This template is used to generate NPC notes. 
**TEMPLATE-NewObstacle** This template is used to generate notes pertaining to Obstacles in the party's path. 
**TEMPLATE-NewTrap** This template is used to generate notes about Traps. 