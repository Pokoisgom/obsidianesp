Index:: [[⛩️Altar]] | [[🎵 Jardín de sonidos]]
Tags:: #au/input | #au/processed | #au/finished | #au/incomplete | #music/C | #music/D | #music/E | #music/F | #music/G | #music/A | #music/B | #music/read | #pronunciation | #rd 

--------

# <%tp.file.title%>

## Archivos de Audio

## Acordes

## ¿A qué esta relacionado?


## ¿Qué sentimientos te evoca?


# ¿Qué proyecto o canción tienes relacionado a esta pista?


----------------
Created:: <%tp.date.now("YYYY-MM-DD HH:mm") %>

<%*
const hasTitle = !tp.file.title.startsWith("Audio_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Ingresar nombre del audio");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>
