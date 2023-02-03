Index:: [[⛩️Altar]] | [[🤺 Diarios activos]]

Tags:: #J/MH | #rd

Rating::

Deadline:: 

----------------------
# <% tp.file.title %>

# Meditación de malos hábitos

 - El hábito en el que estoy meditando es:
R.
-  ¿Qué ocurrirá si no cambio este mal habito ahora?
R.
- ¿Esto es lo más escencial?
R. 
- ¿Esto es representativo de mi caracter? ¿Es quien quiero ser?
R.
- ¿Por qué no soy mejor de lo que soy ahora?
R.
- ¿Por qué vuelvo siempre a la misma gente en lugar de otra? (recuerdos, experiencias, etc)
R.
- ¿Cuándo es probable que lo haga?
R. 
- ¿Qué me hará mas próximo a hacerlo?
R. 
-  ¿Estoy inseguro de algo?
R.
-  ¿Qué ocurrirá si fallo completamente?
R. 
-  ¿Estoy seguro de que lo puedo hacer?
R. 
-  ¿Al menos una versión?
R. 
-  ¿Estoy seguro de que puedo mejorar?
R.  
-  ¿Qué me preocupa?
R. 
-  Si fallo, ¿qué parte de mi se sentirá completamente devastado?
R. 

----------------

Created:: <% tp.date.now("YYYY-MM-DD HH:mm") %>

<%*
const hasTitle = !tp.file.title.startsWith("Bad_Habits_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("El habito que estoy analizando es: ");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>