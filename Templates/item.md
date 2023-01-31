<%* 
let qcFileName = await tp.system.prompt("Item")
text = qcFileName.replace(":", " -")
titleName = text
await tp.file.rename(titleName) 
await tp.file.move("Items/"+ titleName);
-%>
---
tags:
- item
---

<% tp.file.cursor(1) %>
