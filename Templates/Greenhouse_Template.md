Index:: [[⛩️Altar]] | [[🌞Jardín de Ideas]]
Tags:: #n/🌱 | #n/🌿 | #n/🌲 | #on/health | #on/music | #on/code | #on/study | #on/people | #on/goals | #on/games | #on/finances | #on/productivity | #rd

--------
# <% tp.file.title %>

<%*
const hasTitle = !tp.file.title.startsWith("Greenhouse_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Ingresar nombre de nota");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>
# Main Idea

## Interconnected


------------------------------
Created:: <% tp.date.now("YYYY-MM-DD HH:mm") %>