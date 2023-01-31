<%* 
let qcOrigin = await tp.system.suggester(["Human", "Dwarf", "Elf", "Goblin", "Changeling"], ["human", "dwarf", "elf", "goblin", "changeling"], false, "Origin")
let qcFileName = await tp.system.prompt("Name")
text = qcFileName.replace(":", " -")
titleName = text
await tp.file.rename(titleName) 
await tp.file.move("People/"+ titleName)
-%>
---
tags:
- person
- <% qcOrigin %>
aliases: []
---

<% tp.file.cursor(1) %>