---
tags:
 - NPC
notetype: NPC
scope: global
<%*
  const modalForm = app.plugins.plugins.modalforms.api;
  const result = await modalForm.openForm("ModalForm-NewNPC");
  tR += result.asFrontmatterString();
-%>
---


<% await tp.file.move("/Mechanics/NPCs/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewNPC");
let title;
if (!hasTitle) {
    title = result.get("name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>


````col
```col-md
flexGrow=1
===
#### Appearance

![[z_Assets/Images/NPCs/NPCMissingPicture.jpg|200]]

<% result.get("Appearance") %>

```
```col-md
flexGrow=1
===
### <% result.get("name") %>

_<% result.get("size") %> <% result.get("creature_family") %> (<% result.get("species") %>), <% result.get("alignment") %>_
<% result.get("gender") %> <% result.get("class") %>


#### Personality

<% result.get("Personality") %>

```
````

#### Locations


#### Adventures


#### Stats

````col
```col-md
flexGrow=1
===

| STR                           | DEX                           | CON                           | INT                           | WIS                           | CHA                           |
| ----------------------------- | ----------------------------- | ----------------------------- | ----------------------------- | ----------------------------- | ----------------------------- |
| `= this.str`    | `= this.dex`    | `= this.con`    | `= this.int`    | `= this.wis`    | `= this.cha`    |
| `=floor((this.str - 10) / 2)` | `=floor((this.dex - 10) / 2)` | `=floor((this.con - 10) / 2)` | `=floor((this.int - 10) / 2)` | `=floor((this.wis - 10) / 2)` | `=floor((this.cha - 10) / 2)` |

```
```col-md
flexGrow=1
===

|                |                                  |
| -------------- | -------------------------------- |
| Hit Points     | `= this.hp`                |
| Base AC        | `= this.ac`                |
| Proficiency    | `= this.proficiency`              |
| (P) Perception | `= this.passiveperception` |

```
````
