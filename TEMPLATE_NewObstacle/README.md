# TEMPLATE-NewObstacle

This template is used to generate Obstacle notes. In this case I'm sort of defining obstacles as decision points for players. They could be environmental dangers, social encounters, or potential combat encounters that characters have to decide whether to go through or around. 

## Setup

### Installation

1. In Obsidian, open your Command Palette and choose **Modal Form: Manage Forms**
2. Click on the **Import Form** button
3. Copy and paste the contents of `ModalForm-NewObstacle.json` and click Import
4. Download `ModalForm-NewObstacle.md` and place it in your Global Templates folder. 
5. Choose to either replace your entire existing Quick Add data.json file with the contents of `QuickAdd_data.json` or add just the contents of `QuickAdd_NewObstacle-Snippet.json` into your "Choices" field.  

### Files

[ModalForm-NewObstacle.json](/TEMPLATE_NewObstacle/ModalForm-NewObstacle.json) This file contains the settings for the "New Obstacle" Modal Form. This is the file that you would choose with the "Import" option in the "Manage Forms" page of Modal Forms. <br>
[ModalForm-NewObstacle.md](/TEMPLATE_NewObstacle/ModalForm-NewObstacle.md) This is the template file for "New Obstacle." This file is placed in your Global Templates folder. <br>
[QuickAdd_NewObstacle-Snippet.json](/TEMPLATE_NewObstacle/QuickAdd_NewObstacle-Snippet.json) If you do not overwrite your entire `(Vault_Directory)/.obsidian/plugins/quickadd/data.json` file, you can copy and paste this portion of code within the "Choices" block to add a "NewObstacle" quick add command. 

## Usage

1. Open your Command Palette and choose **Quick Add: NewObstacle**

![Screenshot - Quick Add NewObstacle](/images/screenshot_quickadd_newobstacle.png "Screenshot - Quick Add NewObstacle")

2. Fill in the details for this danger in the user input form

![Screenshot - NewObstacle Modal Form](/images/screenshot_modalform_newobstacle.png "Screenshot - NewObstacle Modal Form")

3. The template converts this into a new note with the form values and places it in the appropriate folder

![Screenshot - NewObstacle Example Note](/images/screenshot_newobstacle_example.png "Screenshot - NewObstacle Example Note")

### Form Fields

When the form is launched, you are prompted to fill in the following fields:

| Parameter | Label | Explanations | Input Type |
|---|---|---|---|
|name|Name of Obstacle|A unique name that will become the title of the note|Text|
|habitat|Habitat|The habitat(s) in which you might find this obstacle|Multi-Selection|
|description|Description|A detailed synopsis of the obstacle. The main text of your note|Text Area|
|mechanics|Mechanics|How to mechanically run the obstacle (saves, rolls, etc.)|Text Area|
|link|Source|The book name, URL, or other attribution for this danger|Text|