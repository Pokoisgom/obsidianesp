Index:: [[⛩️Altar]]
Tags:: #au/input | #au/processed | #au/finished | #au/incomplete | #music/C | #music/D | #music/E | #music/F | #music/G | #music/A | #music/B | #music/read | #pronunciation

-----------------------------------------

Aqui es donde almacenaras tus ideas musicales. Conectalas con tu jardín de ideas o otras en esta misma sección, como te guste. Al insertar un audio, el template indicará 

```button
name Insertar Audio
type command
action QuickAdd: Este audio se llama:
```

-------------------------------

# First Input #au/input 
```dataview
table Deadline
FROM #au/input 
WHERE file.name != "Audio_Template" AND file.name != "🎵 Jardín de sonidos"
SORT Deadline asc
```


# Processed #au/processed  
```dataview
table Deadline
FROM #au/processed  
WHERE file.name != "Audio_Template" AND file.name != "🎵 Jardín de sonidos"
SORT Deadline asc
```


# Finished #au/finished  
```dataview
table Deadline
FROM #au/finished  
WHERE file.name != "Audio_Template" AND file.name != "🎵 Jardín de sonidos"
SORT Deadline asc
```


# Incomplete #au/incomplete  
```dataview
table Deadline
FROM #au/incomplete  
WHERE file.name != "Audio_Template" AND file.name != "🎵 Jardín de sonidos"
SORT Deadline asc
```


---------------------------------

Completado:: 2022-12-04 15:23