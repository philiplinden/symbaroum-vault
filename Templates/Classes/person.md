---
aliases: 
class: person
limit: 100
mapWithTag: true
icon: user
tagNames: 
excludes: 
extends: 
version: "2.0"
fields:
  - id: AvNjoW
    name: origin
    options:
      valuesList:
        "1": human
        "2": abducted-human
        "3": goblin
        "4": changeling
        "5": dwarf
        "7": elf
        "8": ogre
      sourceType: ValuesList
      valuesListNotePath: ""
      valuesFromDVQuery: ""
    type: Select
    path: ""
  - id: hwzV3d
    name: faction
    options: {}
    type: MultiFile
    path: ""
  - id: m5fw11
    name: player-character
    options: {}
    style:
      bold: true
    type: Boolean
    path: ""
  - id: URbfQa
    name: occupation
    options: {}
    type: Input
    path: ""
  - id: Ss9aS8
    name: demeanor
    options: {}
    style:
      italic: true
    type: Input
    path: ""
---

origin:: {"type":"Select","options":{"valuesList":{"1":"human","2":"abducted-human","3":"goblin","4":"changeling","5":"dwarf","7":"elf","8":"ogre"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""}}
faction:: {"type":"MultiFile","options":{}}
player-character:: {"type":"Boolean","options":{},"style":{"bold":true}}
occupation:: {"type":"Input","options":{}}
demeanor:: {"type":"Input","options":{},"style":{"italic":true}}