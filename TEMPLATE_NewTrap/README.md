# TEMPLATE-NewTrap

This template is used to generate notes for everyone's favorite dungeon detail - traps. 

## Setup

### Installation

1. In Obsidian, open your Command Palette and choose **Modal Form: Manage Forms**
2. Click on the **Import Form** button
3. Copy and paste the contents of `ModalForm-NewTrap.json` and click Import
4. Download `ModalForm-NewTrap.md` and place it in your Global Templates folder. 
5. Choose to either replace your entire existing Quick Add data.json file with the contents of `QuickAdd_data.json` or add just the contents of `QuickAdd_NewTrap-Snippet.json` into your "Choices" field.  

### Files

[ModalForm-NewTrap.json](/TEMPLATE_NewNaturalDanger/ModalForm-NewTrap.json) This file contains the settings for the "New Trap" Modal Form. This is the file that you would choose with the "Import" option in the "Manage Forms" page of Modal Forms. <br>
[ModalForm-NewTrap.md](/TEMPLATE_NewNaturalDanger/ModalForm-NewTrap.md) This is the template file for "New Trap." This file is placed in your Global Templates folder. <br>
[QuickAdd_NewTrap-Snippet.json](/TEMPLATE_NewNaturalDanger/QuickAdd_NewTrap-Snippet.json) If you do not overwrite your entire `(Vault_Directory)/.obsidian/plugins/quickadd/data.json` file, you can copy and paste this portion of code within the "Choices" block to add a "NewTrap" quick add command. 

## Usage

1. Open your Command Palette and choose **Quick Add: NewTrap**

![Screenshot - Quick Add NewTrap](/images/screenshot_quickadd_newtrap.png "Screenshot - Quick Add NewTrap")

2. Fill in the details for this danger in the user input form

![Screenshot - NewTrap Modal Form](/images/screenshot_modalform_newtrap.png "Screenshot - NewTrap Modal Form")

3. The template converts this into a new note with the form values and places it in the appropriate folder

![Screenshot - NewTrap Example Note](/images/screenshot_newtrap_example.png "Screenshot - NewTrap Example Note")

### Form Fields

When the form is launched, you are prompted to fill in the following fields:

| Parameter | Label | Explanations | Input Type |
|---|---|---|---|
|name|Name of Trap|A unique name that will become the title of the note|Text|
|habitat|Habitat|The habitat(s) in which you might find this trap|Multi-Selection|
|description|Description|A detailed synopsis of the trap. The main text of your note|Text Area|
|detection_disarm|Detection/Disarming|Mechanical notes on how PCs may find and disable the trap|Text Area|
|level_nuisance|Level Nuisance|The party level range at which this trap is simply a nuisance|Single Selection|
|level_deadly|Level Deadly|The party level range at which this trap becomes deadly|Single Selection|
|level_lethal|Level Lethal|The party level range at which this trap will almost certainly result in death|Single Selection|
|savedc|Save DC|The save (if any) that PCs must roll to avoid the trap's consequences|Text|
|type|Trap Type|The category of trap (Magical, Mechanical, or Other)|Single Selection|
|reset|Reset|How (or if) the trap is reset to be triggered again|Text|
|trigger|Trigger|The mechanism that sets off the trap|Single Selection|
|effect|Effect|Damage type, target radius, or other quick info about the trap's impact|Text|
|duration|Duration|How long the effects of the trap last|Text|
|bypass|Bypass|How the trap may be avoided|Text|
|link|Source|The book name, URL, or other attribution for this trap|Text|