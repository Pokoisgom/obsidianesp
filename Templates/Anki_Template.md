Index:: [[⛩️Altar]] | [[💎 Anki]]
Area::

---


```
TARGET DECK: <%tp.file.title%>

START
Basic

Back:
Tags: #SRAnki 
END
```

<%*
const hasTitle = !tp.file.title.startsWith("Anki_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Ingresar nombre del mazo");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>
