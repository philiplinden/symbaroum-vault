---
tags: reference, quest
---
```dataview
TABLE reward, active
FROM #quest and !#reference
WHERE !complete
SORT active DESC, reward DESC
```
