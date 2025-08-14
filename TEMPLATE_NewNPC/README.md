# TEMPLATE-NewNPC

This template is used to generate new NPC notes

## Setup

### Installation

1. In Obsidian, open your Command Palette and choose **Modal Form: Manage Forms**
2. Click on the **Import Form** button
3. Copy and paste the contents of `ModalForm-NewNPC.json` and click Import
4. Download `ModalForm-NewNPC.md` and place it in your Global Templates folder. 
5. Choose to either replace your entire existing Quick Add data.json file with the contents of `QuickAdd_data.json` or add just the contents of `QuickAdd_NewNPC-Snippet.json` into your "Choices" field.  

### Files

[ModalForm-NewNPC.json](/TEMPLATE_NewNPC/ModalForm-NewNPC.json) This file contains the settings for the "New NPC" Modal Form. This is the file that you would choose with the "Import" option in the "Manage Forms" page of Modal Forms. <br>
[ModalForm-NewNPC.md](/TEMPLATE_NewNPC/ModalForm-NewNPC.md) This is the template file for "New NPC." This file is placed in your Global Templates folder. <br>
[QuickAdd_NewNPC-Snippet.json](/TEMPLATE_NewNPC/QuickAdd_NewNPC-Snippet.json) If you do not overwrite your entire `(Vault_Directory)/.obsidian/plugins/quickadd/data.json` file, you can copy and paste this portion of code within the "Choices" block to add a "NewNPC" quick add command. 
[NPCMissingPicture.jpg](/TEMPLATE_NewNPC/NPCMissingPicture.jpg) This is technically optional, but I like to stage a "missing picture" on new NPC notes. Then later if I find an image to use for an important NPC, I can replace it in the note. 

## Usage

1. Open your Command Palette and choose **Quick Add: NewNPC**

![Screenshot - Quick Add NewNPC](/images/screenshot_quickadd_newnpc.png "Screenshot - Quick Add NewNPC")

2. Fill in the details for this NPC in the user input form

![Screenshot - NewNPC Modal Form](/images/screenshot_modalform_newnpc.png "Screenshot - NewNPC Modal Form")

3. The template converts this into a new note with the form values and places it in the appropriate folder

![Screenshot - NewNPC Example Note](/images/screenshot_newnpc_example.png "Screenshot - NewNPC Example Note")

### Form Fields

When the form is launched, you are prompted to fill in the following fields:

| Parameter | Label | Explanations | Input Type |
|---|---|---|---|
|name|Character Name|A unique character name for your NPC|Text|
|alignment|Alignment|The moral alignment of the NPC|Single Selection|
|species|Species|The race/species of the NPC|Text|
|creature_family|Creature Family Type|General type of NPC creature (Humanoid, Construct, Dragon, etc.)|Text|
|gender|Gender|The NPC's gender or lack thereof|Single Selection|
|class|Class or Job|The NPC's class or primary career/job|Text|
|size|Creature Size|The NPC's size category|Single Selection|
|hp|HP|The NPC's current HP|Number|
|ac|AC|The NPC's armor class|Number|
|proficiency|Proficency Bonus|The NPC's proficiency bonus|Number|
|passiveperception|Passive Perception|The NPC's passive perception|Number|
|str|Strength|NPC Strength Score|Number|
|dex|Dexterity|NPC Dexterity Score|Number|
|con|Constitution|NPC Constitution Score|Number|
|int|Intelligence|NPC Intelligence Score|Number|
|wis|Wisdom|NPC Wisdom Score|Number|
|cha|Charisma|NPC Charisma Score|Number|
|Appearance|Appearance|The NPC's general appearance and physical traits|Text Area|
|Personality|Personality Traits|Notes about the NPC's personality, demeanor to PCs, or goals|Text Area|