---
started: <%tp.date.now("YYYY-MM-DD")%>
finished: 
rating:
---
Index:: [[β©οΈAltar]] | [[π₯ Entradas principales]]
Tags:: #π₯/π© | #π₯/π¨ | #π₯/π₯ | #π₯/β¬ | #i/code | #i/work | #i/music | #i/personal | #i/book | #i/games | #i/profile | #i/definition | #i/languages | #i/article | #rd

---------------------
# <%tp.file.title%>
<%*
const hasTitle = !tp.file.title.startsWith("Input_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Enter Input Name");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>


## Resumen
### Notas

### Pensamientos personales
#### Pre-Lectura
- 
#### Post Lectura
- 

------------------

Created:: <%tp.date.now("YYYY-MM-DD HH:mm") %>