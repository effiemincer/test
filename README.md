| Stack | Input | Action |
|-------|--------|---------|
| 0 | foreach var1 ( var2 .. var3 , list ) $ | shift-2 |
| 0foreach2 | var1 ( var2 .. var3 , list ) $ | shift-3 |
| 0foreach2var3 | ( var2 .. var3 , list ) $ | shift-4 |
| 0foreach2var3(4 | var2 .. var3 , list ) $ | shift-8 |
| 0foreach2var3(4var8 | .. var3 , list ) $ | shift-11 |
| 0foreach2var3(4var8..11 | var3 , list ) $ | shift-12 |
| 0foreach2var3(4var8..11var12 | , list ) $ | reduce-7 (R→var..var) |
| 0foreach2var3(4R13 | , list ) $ | shift-14 |
| 0foreach2var3(4R13)14 | $ | reduce-2 (F→foreach var(R)) |
| 0F1 | $ | accept |
