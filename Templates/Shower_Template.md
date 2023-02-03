index:: [[⛩️Altar]] | [[🚿Shower Ideas]]
Tags:: #showeridea | #i/thought| #rd
Deadline:: 

---------------

# <%tp.file.title%>
<%*
const hasTitle = !tp.file.title.startsWith("Shower_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Ingresa un pensamiento random");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>
# What happened?

# Resolution

------------------

Created:: <%tp.date.now("YYYY-MM-DD HH:mm") %>
