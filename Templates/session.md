<%* 
let qcFileName = await tp.system.prompt("Title")
let qcText = await tp.system.prompt("Synopsis")
text = qcFileName.replace(":", " -")
titleName = "📓 " + text
await tp.file.rename(titleName) 
await tp.file.move("_Bricks of Symbaroum/Campaign Notes/"+ titleName)
-%>
---
tags: session
date: <% tp.date.now() %>
players: David, Drew, Abhra, Faris, Kellie
synopsis: <% qcText %>
year: 22
month: 1
---
```ad-done
title: Previous
collapse: open
```dataview
LIST
WHERE 
	contains(file.tags, "session")
	AND
	contains(this.file.inlinks, file.link)
```

> [!NOTE] Next
> 

> [!example] Quests
> 
<% tp.file.cursor(1) %>

