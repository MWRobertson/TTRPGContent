# TEMPLATE-NewNaturalDanger

This template is used to generate two types of notes - Hazards or Dangerous Terrain. The form for these two types of notes asks the same set of questions, and the distinction between them is purely subjective. I personally categorize a "hazard" as a specific natural danger to the party while "dangerous terrain" is a large, dangerous area that the party would travel through for an extended time. 

## Setup

### Installation

1. In Obsidian, open your Command Palette and choose **Modal Form: Manage Forms**
2. Click on the **Import Form** button
3. Copy and paste the contents of `ModalForm-NewNaturalDanger.json` and click Import
4. Download `ModalForm-NewNaturalDanger.md` and place it in your Global Templates folder. 
5. Choose to either replace your entire existing Quick Add data.json file with the contents of `QuickAdd_data.json` or add just the contents of `QuickAdd_NewNaturalDanger-Snippet.json` into your "Choices" field.  

### Files

[ModalForm-NewNaturalDanger.json](/TEMPLATE_NewNaturalDanger/ModalForm-NewNaturalDanger.json) This file contains the settings for the "New Natural Danger" Modal Form. This is the file that you would choose with the "Import" option in the "Manage Forms" page of Modal Forms. <br>
[ModalForm-NewNaturalDanger.md](/TEMPLATE_NewNaturalDanger/ModalForm-NewNaturalDanger.md) This is the template file for "New Natural Danger." This file is placed in your Global Templates folder. <br>
[QuickAdd_NewNaturalDanger-Snippet.json](/TEMPLATE_NewNaturalDanger/QuickAdd_NewNaturalDanger-Snippet.json) If you do not overwrite your entire `(Vault_Directory)/.obsidian/plugins/quickadd/data.json` file, you can copy and paste this portion of code within the "Choices" block to add a "NewNaturalDanger" quick add command. 

## Usage

1. Open your Command Palette and choose **Quick Add: NewNaturalDanger**

![Screenshot - Quick Add NewNaturalDanger](/images/screenshot_quickadd_newnaturaldanger.png "Screenshot - Quick Add NewNaturalDanger")

2. Fill in the details for this danger in the user input form

![Screenshot - NewNaturalDanger Modal Form](/images/screenshot_modalform_newnaturaldanger.png "Screenshot - NewNaturalDanger Modal Form")

3. The template converts this into a new note with the form values and places it in the appropriate folder

![Screenshot - NewNaturalDanger Example Note](/images/screenshot_newnaturaldanger_example.png "Screenshot - NewNaturalDanger Example Note")

### Form Fields

When the form is launched, you are prompted to fill in the following fields:

| Parameter | Label | Explanations | Input Type |
|---|---|---|---|
|name|Name of Danger|A unique name that will become the title of the note|Text|
|habitat|Habitat|The habitat(s) in which you might find this danger|Multi-Selection|
|description|Description|A detailed synopsis of the danger. The main text of your note|Text Area|
|level_nuisance|Level Nuisance|The party level range at which this danger is simply a nuisance|Single Selection|
|level_deadly|Level Deadly|The party level range at which this danger becomes deadly|Single Selection|
|level_lethal|Level Lethal|The party level range at which this danger will almost certainly result in death|Single Selection|
|notetype|Danger Type|Choose whether this is a "Hazard" or "Dangerous Terrain"|Single Selection|
|link|Source|The book name, URL, or other attribution for this danger|Text|