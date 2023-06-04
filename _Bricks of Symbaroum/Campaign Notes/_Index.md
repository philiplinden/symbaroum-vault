---
tags: reference
---
# Campaign Session Notes
```dataviewjs
let pages = dv.pages('"_Bricks of Symbaroum/Campaign Notes"');

for (let group of pages.groupBy(b => b.file.folder)) {
	var arc = group.key.match(/([^\/]*)\/*$/)[1]
	dv.header(3, arc); 
	dv.table(["session", "synopsis", "players", "date"], 
		group.rows
			.sort(k => k.date, 'asc')
			.map(k => [
				k.file.link,
				k.synopsis,
				k.players,
				k.date
			]
		)
	);
}
```
***
# Quests
![[_Bricks of Symbaroum/Quests/_incomplete]]
![[_complete]]
