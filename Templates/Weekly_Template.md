Index:: [[⛩️Altar]]
Tags:: [[<%tp.date.now("YYYY-[M]MM")%>]] #Semanal | #rw
Links:: [[📆 Diario]]

-------------

# <%tp.file.title%>
[[<%moment(tp.file.title,'YYYY-[W]WW').format("YYYY")%>-W<%moment(tp.file.title,"YYYY-[W]WW").add(-2,'weeks').week()%>|Last Week]] | [[<%moment(tp.file.title,'YYYY-[W]WW').format("YYYY")%>-W<%moment(tp.file.title,"YYYY-[W]WW").week()%>|Next Week]]
# Planeación futura
## A la acción
```dataview
task
WHERE file.name = "<%tp.file.title%>"
```

### Proyectos
```
table deadline, area
FROM [[<%tp.file.title%>]] AND #proyectos 
WHERE file.name !="Project_Template"
SORT deadline asc
```
## Recapitulación

```dataview
table Rating as ⭐, Sentence as Summary, Story, headings as ✍️ and #daily from [[<%tp.file.title%>]]
sort file.name asc
```

### Métricas
#### Energia
```tracker
searchType: dvField
searchTarget: Fisicamente, Mentalmente, Emocionalmente, Espiritualmente, Socialmente
startDate: <%moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(1).format("YYYY-MM-DD")%>
endDate: <% moment(tp.file.title,'YYYY-[W]WW').day(0).format("YYYY-MM-DD")%>
line:
	title: Energia
	yMax: 5
	yAxisLabel: Fis(Ro) / Ment(Az) / Emoc(Am) / Espi(Ve) / Soci(Bl)
	lineColor: red, blue, yellow, green, white
```

**¿Te faltó energía para algo?¿Cómo lo podrías mejorar para la próxima semana?**
- 
### Proyectos
```dataview
table deadline as Deadline, area as Area
FROM [[<%tp.file.title%>]] AND #project 
WHERE file.name !="Project_Template"
SORT deadline asc
```

### Tasks
```dataview
TABLE WITHOUT ID
regexreplace(Tasks.text, "@\[.*$", "") as Task, meta(Tasks.section).subpath as "Status",
file.link as "Board"
FROM #kanbans
FLATTEN file.tasks As Tasks

WHERE contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(1).format("YYYY-MM-DD") %>") OR contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(2).format("YYYY-MM-DD") %>") OR contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(3).format("YYYY-MM-DD") %>") OR contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(4).format("YYYY-MM-DD") %>") OR contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(5).format("YYYY-MM-DD") %>") OR contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').add(-1,'weeks').day(6).format("YYYY-MM-DD") %>") OR contains(Tasks.text,"<% moment(tp.file.title,'YYYY-[W]WW').day(0).format("YYYY-MM-DD") %>")

SORT date(Tasks.due.file.name)
```

## Review
### Aprendizaje
##### Week Highlights
- **Lo mejor:**
- **Lo peor:** 
- **Lección:**
- **Mejora futura:**
- **¿Cumpliste lo que te prometiste?**
- **Pude pasar mas tiempo:**
- **Pude pasar menos tiempo:**

### Puntuación de vida
Salud fisica::
Productividad::
Salud mental::
Aprendizaje::
Relaciones::
Metas::
Experiencias::
Energia::
Finanzas::
Coraje/Espiritu::
Total:: /100

---------------
Created:: <%tp.date.now("YYYY-MM-DD HH:mm") %>