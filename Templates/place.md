<%* 
let qcType = await tp.system.suggester(["Point of interest", "City", "Region", "Terrain"], ["point-of-interest", "city", "region", "terrain"], false, "Type")
let qcFileName = await tp.system.prompt("Place")
text = qcFileName.replace(":", " -")
titleName = text
await tp.file.rename(titleName) 
await tp.file.move("Places/"+ titleName)
-%>
---
tags:
- place
- <% qcType %>
aliases: []
---

<% tp.file.cursor(1) %>