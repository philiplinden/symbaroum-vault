<%* 
let qcFileName = await tp.system.prompt("Event")
text = qcFileName.replace(":", " -")
titleName = text
await tp.file.rename(titleName) 
await tp.file.move("Events/"+ titleName);
-%>
---
tags:
- event
year: null
month: null
---

<% tp.file.cursor(1) %>
