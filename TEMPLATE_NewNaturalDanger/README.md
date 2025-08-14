# TEMPLATE-NewNaturalDanger

This template is used to generate two types of notes - Hazards or Dangerous Terrain. The form for these two types of notes asks the same set of questions, and the distinction between them is purely subjective. I personally categorize a "hazard" as a specific natural danger to the party while "dangerous terrain" is a large, dangerous area that the party would travel through for an extended time. 

### Files

**ModalForm-NewNaturalDanger.json** This file contains the settings for the "New Natural Danger" Modal Form. This is the file that you would choose with the "Import" option in the "Manage Forms" page of Modal Forms. 

**ModalForm-NewNaturalDanger.md** This is the template file for "New Natural Danger." This file is placed in your Global Templates folder. 

**QuickAdd_NewNaturalDanger-Snippet.json** If you do not overwrite your entire *(Vault_Directory)*/.obsidian/plugins/quickadd/data.json file, you can copy and paste this portion of code into the "Choices" block to add a "NewNaturalDanger" quick add command. 

### Implementation

1. In Obsidian, open your Command Palette and choose **Modal Form: Manage Forms**
2. Click on the **Import Form** button
3. Copy and paste the contents of _ModalForm-NewNaturalDanger.json_ and click Import
4. Download _ModalForm-NewNaturalDanger.md_ and place it in your global templates folder. 
5. Choose to either replace your existing QuickAdd data.json file with the contents of *QuickAdd_data.json* or add just the contents of *QuickAdd_NewNaturalDanger-Snippet.json* into your "Choices" field.  

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