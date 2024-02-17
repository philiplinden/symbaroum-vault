---
limit: 100
mapWithTag: true
icon: book-open-check
tagNames: 
excludes: 
extends: 
version: "2.0"
fields:
  - id: Xhff4J
    name: complete
    options: []
    type: Input
    path: ""
  - id: 8G45PL
    command:
      id: insert__presetField__active
      icon: check
      label: Insert active field
    name: active
    options: {}
    type: Boolean
    path: ""
---
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
complete:: {"type":"Boolean","options":{},"command":{"id":"insert__presetField__complete","icon":"file-check","label":"Insert complete field"}}
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

active:: {"type":"Boolean","options":{},"command":{"id":"insert__presetField__active","icon":"check","label":"Insert active field"}}
complete:: {"type":"Boolean","options":{},"command":{"id":"insert__presetField__complete","icon":"file-check","label":"Insert complete field"}}