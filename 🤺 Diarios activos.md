Index:: [[⛩️Altar]]
Tags:: #J/Listening | #J/HQ | #J/TOT | #J/BH

---------------------------

### Si quieres entrenar tu escucha activa con unos ejercicios, utiliza el siguiente input:

```button
name 👂Entrenar escucha activa:
type command
action QuickAdd: Quiero analizar la conversación con el topico llamado:
```

### Si quieres cuestionar algo que te esté drenando energía en este momento, utiliza el siguiente input:

```button
name 🧛‍♂️Entrenar:
type command
action QuickAdd: Lo que me está drenando energía en este momento es:
```

### Si quieres meditar en malos hábitos:

```button
name Insertar ☠️Malos hábitos:
type command
action QuickAdd: Estoy pensando en eliminar de mi vida el habito de:
```


### Si te proyectas a 5 años con un objetivo, utiliza este template:

```button
name 🎯Insertar "The One Thing" Ejercicio
type command
action QuickAdd: Quiero proyectar lo aprendido en el libro TOT en:
```


------------

# 👂Listening Training #J/E

```dataview
table Rating as Rating, deadline as Deadline
FROM #J/Listening and !"Templates" 
WHERE file.name !="🤺 Diarios activos"
sort file.mtime desc
```

# 🧛‍♂️Hard Questions #J/PD
```dataview
table Rating as Rating, deadline as Deadline
FROM #J/HQ and !"Templates" 
WHERE file.name !="🤺 Diarios activos"
sort file.mtime desc
```

# ☠️Bad Habits Analysis #J/MH
```dataview
table Rating as Rating, deadline as Deadline
FROM #J/BH and !"Templates" 
WHERE file.name !="🤺 Diarios activos"
sort file.mtime desc
```

# 🎯The One Thing Exercise #J/TOT 
```dataview
table Rating as Rating, deadline as Deadline
FROM #J/TOT and !"Templates" 
WHERE file.name !="🤺 Diarios activos"
sort file.mtime desc
```


-----------
Completado:: 2022-12-20 21:00