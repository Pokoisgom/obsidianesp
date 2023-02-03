Index:: [[⛩️Altar]]
Tags:: #📥/🟩 | #📥/🟨 | #📥/🟥 | #📥/⬛ | #i/code | #i/work | #i/music | #i/personal | #i/book | #i/games | #i/profile | #i/definition | #i/languages | #i/article 

------------------------------------------------

Aqui es donde las entradas principales serán almacenadas. El jardín de Ideas se alimentará de las entradas principales, pero las entradas principales no se alimentaran del jardín de ideas. Aquí es donde comienza todo, podría partir como un tipo indice.

```button
name Insertar Entrada
type command
action QuickAdd: Mi entrada principal se llama:
```

-----------------------------------


# Finalizados #📥/🟩
```dataview
table Deadline
FROM #📥/🟩 
WHERE file.name != "Input_Template" AND file.name != "📥 Entradas principales"
SORT Deadline asc
```

# Editando #📥/🟨 
```dataview
table Deadline
FROM #📥/🟨  
WHERE file.name != "Input_Template" AND file.name != "📥 Entradas principales"
SORT Deadline asc
```

# Detenido #📥/🟥 
```dataview
table Deadline
FROM #📥/🟥   
WHERE file.name != "Input_Template" AND file.name != "📥 Entradas principales"
SORT Deadline asc
```

# Incompletos #📥/⬛ 
```dataview
table Deadline
FROM #📥/⬛    
WHERE file.name != "Input_Template" AND file.name != "📥 Entradas principales"
SORT Deadline asc
```


------------------------------------

Completado:: 2022-12-04 15:06