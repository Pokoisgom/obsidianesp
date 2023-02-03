index:: [[⛩️Altar]] | [[🚧 Projects]]
tags:: #proyectos/🟩 | #proyectos/🟨  | #proyectos/⬛  | #proyectos/🟥  | #proyectos | #rd
___
# <% tp.file.title %>
Deadline:: <% tp.file.cursor(2) %>
Area:: 

## Logs
### Puntos clave del día anterior:
- [ ] 

### Puntos clave del día de hoy
- [ ] 

### ¿Qué impedimentos tendré?
- [ ] 


<%*
const hasTitle = !tp.file.title.startsWith("Project_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Ingresar nombre de proyecto");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>

## Kanbans

```button
name Insertar Kanban
type note(Kanban_Template) template
action Kanban_Template
templater true
```


### Kanbans del poyecto

```dataview
LIST
FROM #kanbans
WHERE contains(file.name, "")
```

## Recursos Resilientes 
### Notes 
- [Insert Links]()


#### Query
```dataview
list
FROM [[<%tp.file.title%>]] and !outgoing([[<%tp.file.title%>]])
```

Links
- Add interesting material that you can rely on here


## Planeación
Goals:
- [ ] Meta de algún día:
- [ ] Meta próximos 5 años:
- [ ] Meta próximo 1 año:
- [ ] Meta próximos 6 meses:
- [ ] Meta próximo 1 mes: 
- [ ] Meta semana 1 (como si fuera hoy):
- [ ] Meta semana 2 (como si fuera hoy):
- [ ] Meta semana 3 (como si fuera hoy):
- [ ] Meta semana 4 (como si fuera hoy):
- [ ] Meta hoy:

**Puntos clave de hoy**
- [ ] 

**Obstaculos y soluciones**:
- [ ] My obstaculo de algún día:
	- [ ] La solución es:
- [ ] My obstaculo para los próximos 5 años:
	- [ ] La solución es:
- [ ] My obstaculo para el siguiente año:
	- [ ] La solución es:
- [ ] Mi obstaculo para los próximos 6 meses:
	- [ ] La solución es:
- [ ] My obstaculo para este mes:
	- [ ] La solución es:
- [ ] My obstaculo semanal es:
	- [ ] La solución es:
- [ ] Obstaculo de hoy:
	- [ ] La solución es:

**Timeframe**:
- [ ] Week: 

### Review
**¿Te encuentras satisfecho?**
- R:
**¿Te sentiste experimentado??**
- R: 
**¿Puedes nombrar alguna mejora?**:
- R:


___
Created:: <%tp.date.now("YYYY-MM-DD HH:mm") %>
