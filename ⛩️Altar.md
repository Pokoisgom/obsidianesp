---
Cssclass: dashboard
banner: "![[jose-luis-sanchez-pereyra-U6HOr6-CPSA-unsplash.jpg]]"
---

# Cuando te sientas perdido, regresa a este lugar.

# Foco
- ## [[⛰️ Montaña]]
	- Creados recientemente:
	```dataview
	table file.ctime as creado
	FROM #area and !outgoing([[⛰️ Montaña]]) and !"Templates" and !"⛰️ Montaña"
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```

- ## [[🚧 Proyectos]]
	- Proyectos creados recientemente:
	```dataview
	table file.ctime as creado
	FROM #proyectos  
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```
- ## [[📥 Entradas principales]]
	- Entradas creadas recientemente:
	```dataview
	table file.ctime as creado
	FROM #📥/🟩
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```
- ## [[🎵 Jardín de sonidos]] 
	- Entradas de audio creadas recientemente:
	```dataview
	table file.ctime as creado
	FROM #au OR #music OR #pronunciation 
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```
- ## [[🌞Jardín de Ideas]]
	- Notas creadas recientemente:
	```dataview
	table file.ctime as creado
	FROM #n OR #on 
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```
- ## [[🔄 Revision]]
	- Notas y entradas para hacer review recientes:
	```dataview
	table file.ctime as creado
	FROM #rw OR #rd
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```
- ## [[📁 Archivado]]
	- Archivados recientemente:
	```dataview
	table file.ctime as creado
	FROM #archived 
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```
- ## [[💎 Anki]]
	- Mazos creados recientemente:
	```dataview
	table file.ctime as creado
	FROM #s/deck OR #s/card  
	WHERE file.ctime > (date(now) - dur(6 days))
	sort file.mtime desc
	```

# Diario
- [[🚿 Ideas en la Ducha]]
- [[📆 Diario]]
- [[🏃‍♂️ Rutinario]]
- [[🤺 Diarios activos]]


