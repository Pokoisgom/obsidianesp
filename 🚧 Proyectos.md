Index:: [[⛩️Altar]]
tags:: #proyectos/🟩 | #proyectos/🟨 | #proyectos/⬛ | #proyectos/🟥 | #proyectos  |  

-------------------------------------

```button
name Insertar Proyecto
type command
action QuickAdd: Este proyecto se llama:
```

-------------------------------------

# Activos #proyectos/🟩
```dataview
table Deadline
FROM #proyectos/🟩 
WHERE file.name != "Project_Template" AND file.name != "🚧 Proyectos"
SORT Deadline asc
```

# Descanso #proyectos/🟨 
```dataview
table Deadline
FROM #proyectos/🟨 
WHERE file.name != "Project_Template" AND file.name != "🚧 Proyectos"
SORT Deadline asc
```

# Detenido #proyectos/🟥 
```dataview
table Deadline
FROM #proyectos/🟥 
WHERE file.name != "Project_Template" AND file.name != "🚧 Proyectos"
SORT Deadline asc
```

# Backlog #proyectos/⬛ 
```dataview
table Deadline
FROM #proyectos/⬛ 
WHERE file.name != "Project_Template" AND file.name != "🚧 Proyectos"
SORT Deadline asc
```

------------------------------------

Completado:: 2022-12-03 09:00