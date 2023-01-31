<%* 
let qcFileName = await tp.system.prompt("Beast")
text = qcFileName.replace(":", " -")
titleName = text
await tp.file.rename(titleName) 
await tp.file.move("Beasts/"+ titleName);
-%>
---
tags:
- beast
---

<% tp.file.cursor(1) %>