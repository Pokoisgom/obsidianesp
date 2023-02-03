Index:: [[⛩️Altar]] | [[⛰️ Montaña]]
tags:: #montaña 

--------------------

# <%tp.file.title%>


```button
name Insertar Proyecto
type command
action QuickAdd: Este proyecto se llama:
```
```button
name Insertar Entrada
type command
action QuickAdd: Mi entrada principal se llama:
```
```button
name Insertar Nota
type command
action QuickAdd: Mi nota se llama:
```
```button
name Insertar Audio
type command
action QuickAdd: Este audio se llama:
```



# Queries
## Projects
```dataview
table Deadline
FROM #project AND [[<%tp.file.title%>]]
SORT Deadline asc
```

## Inputs
```dataview
table Status, Author
FROM #i AND [[<%tp.file.title%>]]
SORT file.mtime desc
```

## Notes
```dataview
table Created
FROM [[<%tp.file.title%>]] AND !#project AND !#i
SORT file.mtime desc
```


-------

Created:: <% tp.date.now("YYYY-MM-DD HH:mm") %>

<%*
const hasTitle = !tp.file.title.startsWith("Esta montaña se llama:");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Ingresa un nombre:");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>