<%* 
let qcFileName = await tp.system.prompt("Quest")
let qcReward = await tp.system.prompt("Reward (in thaler)", 0)
text = qcFileName.replace(":", " -")
titleName = "📜 " + text
await tp.file.rename(titleName) 
await tp.file.move("_Bricks of Symbaroum/Quests/"+ titleName)
-%>
---
tags: quest
active: false
complete: false
reward: <% qcReward %>
---

## Info
**Objectives:** <% tp.file.cursor(1) %>
**Stakeholders:** 
**Reward:**  <% qcReward %> thaler
```math
reward = <% qcReward %> # thaler
boss_cut = 0.25 # percent
party_cut = reward * (1 - boss_cut)
per_person = party_cut / 5 # thaler per person
```

## Progress & Updates
