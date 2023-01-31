---
tags: reference, quest
---
```dataview
TABLE reward
FROM #quest and !#reference
WHERE complete
SORT active DESC, reward DESC
```
