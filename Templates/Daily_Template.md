Index:: [[⛩️Altar]]
Tags:: #diario
Date:: <%tp.date.now("YYYY-MM-DD")%>
Week:: [[<%moment(tp.file.title,'YYYY-MM-DD').format("YYYY")%>-W<%moment(tp.file.title,"YYYY-MM-DD").add(-1,'days').week()%>]]

----------------------------------

# <%tp.file.title%>
<< [[<% moment(tp.file.title,'YYYY-MM-DD').add(-1,'days').format("YYYY-MM-DD")%>]] | [[<%moment(tp.file.title,'YYYY-MM-DD').add(1,'days').format("YYYY-MM-DD") %>]] >>

## Recordatorio
- Ingresa un recordatorio

### ¿Qué ocurrió la última vez?
- [ ] 

### ¿Qué haré hoy y qué impedimientos tengo?
- [ ] 




### Entradas para el día de hoy
- Work notes
- Study notes
- Projects notes

### Tasks
```dataview
TABLE WITHOUT ID
regexreplace(Tasks.text, "@\[.*$","") as Task,
meta(Tasks.section).subpath as "Status",
file.link as " Board"
FROM #kanbans AND [[<%tp.file.title%>]]
FLATTEN file.tasks AS Tasks
WHERE !Tasks.completed
AND contains(Tasks.text, "<%tp.file.title%>")
SORT date(Tasks.due.file.name)
LIMIT 20
```


#### Actual
- ¿Qué tienes en mente ahora?
	- R.
- ¿Qué te hace sentir incómodo ahora? ¿Cómo lo podrías solucionar?
	- R.


### Gratitud
**Menciona lo que te hace sentir agradecido de la vida:**
- 
**¿Por qué estoy agradecido de esto?**
- 
  
**Menciona lo que te hace estar agradecido de tí mismo**:
-  
**¿Por qué estoy agradecido de esto?**
- 
  
### Mentalidad mañanera
- **¿Qué te hace sentir motivado hoy?**
	-  
- **¿Quién te gustaría ser hoy?:**
	-  
- **¿Quién necesita tu mejor versión hoy?:**
	-    
- **¿Qué te causa ansiedad?:**
	-  
- **¿Hay algo que te genere ambición hoy?:**
	-  
- **¿Con quién estás molesto? ¿Cómo puedes solucionarlo hoy?:**
	-  
	

## Reflección
**¿Que te gustaría repetir de hoy?**
- 
**¿Qué te gustaría repetir menos hoy?**
- 
**¿Qué  puedo mejorar para mañana?**
-  
**Qué me hizo sentir sobre mis estandares o bajo mis estandares hoy?**
- 
  
Rating::
Sentence::
Story::

## Energias
**¿Qué hiciste para sentirte renovado? ¿Cómo resultó?**
- 
Fisicamente::
- 
Mentalmente::
- 
Emocionalmente::
- 
Espiritualmente::
- 
Socialmente::
- 



---------------

Created:: <%tp.date.now("YYYY-MM-DD HH:mm") %>