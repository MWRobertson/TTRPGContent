---
tags:
 - Dangers
 - Obstacles
notetype: Obstacles
scope: global
<%*
  const modalForm = app.plugins.plugins.modalforms.api;
  const result = await modalForm.openForm("ModalForm-NewObstacle");
  tR += result.asFrontmatterString();
-%>
---

<% await tp.file.move("/Mechanics/Strategy/Dangers/Obstacles/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewObstacle");
let title;
if (!hasTitle) {
    title = result.get("name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

#### Description

`= this.description`

#### Mechanics

`= this.mechanics`

**Source:** `= this.link`