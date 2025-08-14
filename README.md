## Obsidian TTRPG Tools

This project is a collection of code and templates I've created in an effort to automate building a TTRPG content library with Obsidian. 

## Prerequisites and Assumptions

We're beginning with the assumption that you already have some basic experience using Obsidian including installing Community plug-ins. While it may not be strictly necessary to read through and understand the JSON data files contained here to implement these tools, a general knowledge of JSON formatting would be helpful in the event that any of these files need to be modified to fit your environment. 

### Required Plug-Ins

This project uses the following list of Obsidian Community plug-ins. 

+ [Quick Add](https://github.com/chhoumann/quickadd)
+ [Modal Forms](https://github.com/danielo515/obsidian-modal-form)
+ [Templater](https://github.com/SilentVoid13/Templater)
+ [Dataview](https://blacksmithgu.github.io/obsidian-dataview/)
+ [Columns](https://github.com/tnichols217/obsidian-columns)

![Workflow Diagram for each plug-in](/images/image_workflow.png "Workflow Diagram for each plug-in")

**Quick Add** is used to launch the modal form and kick off the whole workflow.<br>
**Modal Forms** generates user input forms to capture TTRPG data and convert it to a note in Obsidian. <br>
**Templater** essentially maps individual template files to a specific folder location (for example, the NPC template file to the NPC folder.)<br>
**Dataview** uses inline variables to translate the information from a note's frontmatter into values in the note itself.<br>
**Columns** is just used in the formatting of finished notes. As the name implies, it adds ability to create separate columns in a note. <br>

*Optional* Once you have this workflow functioning, you can enhance it with a plug-in like [Meta Bind](https://github.com/mProjectsCode/obsidian-meta-bind-plugin) to create buttons that call each Quick Add command. These buttons can be added to a note to create a dashboard for launching forms. 

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

## Usage

### Customizing the Quick Add plug-in

If you are installing Quick Add from scratch, you can import the settings for all of the commands I've used by ovewriting a data file in the plug-in folder: 

1. Navigate to the directory `(Your_Vault_Directory_Path)/.obsidian/plugins/quickadd/` (Please note, the `.obsidian` folder is hidden by default so you will need to show hidden files first to see it.)
2. Rename the file `(Your_Vault_Directory_Path)/.obsidian/plugins/quickadd/data.json` to `data.json.BACKUP`
3. Copy `QuickAdd_data.json` to `(Your_Vault_Directory_Path)/.obsidian/plugins/quickadd/`
4. Rename `(Your_Vault_Directory_Path)/.obsidian/plugins/quickadd/QuickAdd_data.json` to `data.json`

If you have existing Quick Add settings that you don't want to overwrite, you can also choose to add new commands to the existing code. If you open the data.json file, you should see that it looks something like this: 

```
{
  "choices": [
    {
      "id": "22fa99cd-2420-4a84-a505-562935fccdf0",
      "name": "NewNPC",
      "type": "Template",
```

You can copy and paste the code from each `QuickAdd_(TemplateName)-Snippet.json` file within this "choices" code block. Make sure that each `"{}"` block inside is delimited by a comma to avoid errors. 

### Templates

**TEMPLATE-NewNaturalDanger** This template is used to generate two types of notes - Hazards or Dangerous Terrain. <br>
**TEMPLATE-NewNPC** This template is used to generate NPC notes. <br>
**TEMPLATE-NewObstacle** This template is used to generate notes pertaining to Obstacles in the party's path. <br>
**TEMPLATE-NewTrap** This template is used to generate notes about Traps. <br>
