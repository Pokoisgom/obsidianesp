Index:: [[⛩️Altar]] | [[⛰️ Montaña]]
tags:: #montaña

--------------------

# Cuando se trate de lectura

```button
name Insert Project
type command
action QuickAdd: Template - Project
```
```button
name Insert Input
type command
action QuickAdd: Template - Input
```
```button
name Insert New Note
type command
action QuickAdd: Template - Greenhouse
```
```button
name Insert Audio
type command
action QuickAdd: Template - Audio
```



# Queries
## Projects
```dataview
table Deadline
FROM #project AND [[Cuando se trate de lectura]]
SORT Deadline asc
```

## Inputs
```dataview
table Status, Author
FROM #i AND [[Cuando se trate de lectura]]
SORT file.mtime desc
```

## Notes
```dataview
table Created
FROM [[Cuando se trate de lectura]] AND !#project AND !#i
SORT file.mtime desc
```


-------

Created:: 2023-01-10 17:35

