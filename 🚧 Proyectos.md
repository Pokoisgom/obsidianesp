Index:: [[β©οΈAltar]]
tags:: #proyectos/π© | #proyectos/π¨ | #proyectos/β¬ | #proyectos/π₯ | #proyectos  |  

-------------------------------------

```button
name Insertar Proyecto
type command
action QuickAdd: Este proyecto se llama:
```

-------------------------------------

# Activos #proyectos/π©
```dataview
table Deadline
FROM #proyectos/π© 
WHERE file.name != "Project_Template" AND file.name != "π§ Proyectos"
SORT Deadline asc
```

# Descanso #proyectos/π¨ 
```dataview
table Deadline
FROM #proyectos/π¨ 
WHERE file.name != "Project_Template" AND file.name != "π§ Proyectos"
SORT Deadline asc
```

# Detenido #proyectos/π₯ 
```dataview
table Deadline
FROM #proyectos/π₯ 
WHERE file.name != "Project_Template" AND file.name != "π§ Proyectos"
SORT Deadline asc
```

# Backlog #proyectos/β¬ 
```dataview
table Deadline
FROM #proyectos/β¬ 
WHERE file.name != "Project_Template" AND file.name != "π§ Proyectos"
SORT Deadline asc
```

------------------------------------

Completado:: 2022-12-03 09:00