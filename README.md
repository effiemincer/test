| Stack | Input | Action |
|-------|--------|---------|
| 0 | id1.id2**id3.id4+*(*id5).id6$ | shift-5 |
| 0id5 | .id2**id3.id4+*(*id5).id6$ | reduce-7 (B→id) |
| 0B4 | .id2**id3.id4+*(*id5).id6$ | shift-10 |
| 0B4.10 | id2**id3.id4+*(*id5).id6$ | shift-26 |
| 0B4.10id26 | **id3.id4+*(*id5).id6$ | reduce-8 (B→B.id) |
| 0B4 | **id3.id4+*(*id5).id6$ | reduce-6 (F→B) |
| 0F3 | **id3.id4+*(*id5).id6$ | reduce-4 (T→F) |
| 0T2 | **id3.id4+*(*id5).id6$ | shift-9 |
| 0T2*9 | *id3.id4+*(*id5).id6$ | shift-14 |
| 0T2*9*14 | id3.id4+*(*id5).id6$ | shift-13 |
| 0T2*9*14id13 | .id4+*(*id5).id6$ | reduce-7 (B→id) |
[... continuing with remaining steps ...]
