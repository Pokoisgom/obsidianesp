Index:: [[⛩️Altar]] | [[🤺 Diarios activos]]

Tags:: #J/PD | #rd

Rating::

Deadline:: 

----------------------
# <% tp.file.title %>

# Preguntas dificiles que debes hacerte cada tanto:
### Puede que nunca tengas las respuestas...
- ¿Qué sentimientos oscuros tienes respecto al tema que quieres meditar?
R. 
- ¿Por qué lo tengo?
R. 
- ¿Qué es lo que me interesa?
R. 
- ¿Por qué estoy interesado en alcanzarlo tan pronto como pueda?
R.
- ¿Por qué procrastino y cómo?
R.
- ¿Qué no estoy dispuesto a hacer?
R.
- ¿Qué me parece bien?
R.
- ¿Cómo me felicito y me castigo por acertar o fallar?
R.
- ¿Qué no estan bueno de mi que podría mejorar? ¿Qué debería mejorar basado en mis estandares? 
R.
-  ¿Es dificil admitir que necesitas pasos de novato para realizar las cosas al principio? No tengas miedo de decir si... piensa en una razón por la cual te molestas.
R.
- ¿Qué te hace sentir pasado a llevar? 
R.
- ¿Qué te hace actuar como arrogante? ¿Qué haces?
R.


----------------

Created:: <% tp.date.now("YYYY-MM-DD HH:mm") %>

<%*
const hasTitle = !tp.file.title.startsWith("Hard_Questions_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Estoy pensando en mejorar: ");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>