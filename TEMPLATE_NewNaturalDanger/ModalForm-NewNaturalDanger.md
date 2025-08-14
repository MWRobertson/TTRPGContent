---
<%*
  const modalForm = app.plugins.plugins.modalforms.api;
  const result = await modalForm.openForm("ModalForm-NewDangerNatural");
  tR += result.asFrontmatterString();
-%>
tags:
 - Dangers
 - <% result.get("notetype") %>
scope: global
---

<% await tp.file.move("/Mechanics/Strategy/Dangers/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewNaturalDanger");
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

```
```col-md
flexGrow=1
===
#### Level Balance

|          |                         |
| -------- | ----------------------- |
| Nuisance | `= this.level_nuisance` |
| Deadly   | `= this.level_deadly`   |
| Lethal   | `= this.level_lethal`   |

```
````

**Source:** `= this.link`