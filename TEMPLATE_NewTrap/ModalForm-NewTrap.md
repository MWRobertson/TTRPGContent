---
tags:
 - Dangers
 - Trap
notetype: Trap
scope: global
<%*
  const modalForm = app.plugins.plugins.modalforms.api;
  const result = await modalForm.openForm("ModalForm-NewTrap");
  tR += result.asFrontmatterString();
-%>
---

<% await tp.file.move("/Mechanics/Strategy/Dangers/Traps/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewTrap");
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
flexGrow=2
===
#### Description

`= this.description`

#### Detection/Disarming

`= this.detection_disarm`
```
```col-md
flexGrow=1
===
#### Mechanics

|          |                   |
| -------- | ----------------- |
| Type     | `= this.type`     |
| Save DC  | `= this.savedc`   |
| Trigger  | `= this.trigger`  |
| Reset    | `= this.reset`    |
| Effect   | `= this.effect`   |
| Duration | `= this.duration` |
| Bypass   | `= this.bypass`   |

#### Level Balance

|          |                         |
| -------- | ----------------------- |
| Nuisance | `= this.level_nuisance` |
| Deadly   | `= this.level_deadly`   |
| Lethal   | `= this.level_lethal`   |

```
````

**Source:** `= this.link`