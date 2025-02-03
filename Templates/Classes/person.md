---
aliases: 
class: person
limit: 100
mapWithTag: true
icon: user
tagNames: 
excludes: 
extends: 
version: "2.2"
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
filesPaths: 
bookmarksGroups: 
savedViews:
  - name: Ordo Magica
    children: []
    sorters: []
    filters:
      - id: person____file
        name: file
        query: ""
      - id: person____demeanor
        name: demeanor
        query: ""
      - id: person____occupation
        name: occupation
        query: ""
      - id: person____player-character
        name: player-character
        query: ""
      - id: person____faction
        name: faction
        query: Ordo Magica
      - id: person____origin
        name: origin
        query: ""
    columns:
      - id: person____file
        name: file
        hidden: false
        position: 0
      - id: person____demeanor
        name: demeanor
        hidden: false
        position: 1
      - id: person____occupation
        name: occupation
        hidden: false
        position: 2
      - id: person____player-character
        name: player-character
        hidden: false
        position: 3
      - id: person____faction
        name: faction
        hidden: false
        position: 4
      - id: person____origin
        name: origin
        hidden: false
        position: 5
favoriteView: 
fieldsOrder:
  - Ss9aS8
  - URbfQa
  - m5fw11
  - hwzV3d
  - AvNjoW
---

origin:: {"type":"Select","options":{"valuesList":{"1":"human","2":"abducted-human","3":"goblin","4":"changeling","5":"dwarf","7":"elf","8":"ogre"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""}}
faction:: {"type":"MultiFile","options":{inFrontmatter: true}}
player-character:: {"type":"Boolean","options":{},"style":{"bold":true}}
occupation:: {"type":"Input","options":{}}
demeanor:: {"type":"Input","options":{},"style":{"italic":true}}