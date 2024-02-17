---
limit: 100
mapWithTag: true
icon: file-signature
tagNames: session
excludes: 
extends: event
version: "2.0"
fields:
  - id: nPHP21
    name: players
    options:
      valuesList:
        "1": Faris
        "2": Kellie
        "3": David
        "4": Drew
        "5": Abhra
      sourceType: ValuesList
      valuesListNotePath: ""
      valuesFromDVQuery: ""
    type: Multi
    path: ""
  - id: 1z7Tkr
    name: date
    options:
      dateFormat: YYYY-MM-DD
      defaultInsertAsLink: "false"
    type: Date
    path: ""
  - id: UlsRbC
    name: synopsis
    options: {}
    style:
      italic: true
    type: Input
    path: ""
---
players:: {"type":"Multi","options":{"valuesList":{"1":"Faris","2":"Kellie","3":"David","4":"Drew","5":"Abhra"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""}}
date:: {"type":"Date","options":{"dateFormat":"YYYY-MM-DD","defaultInsertAsLink":"false"}}
synopsis:: {"type":"Input","options":{},"style":{"italic":true}}