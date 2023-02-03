---

kanban-plugin: basic
tags: kanbans

---

<%*
const hasTitle = !tp.file.title.startsWith("Kanban_Template");
let title;
if (!hasTitle) {
	title = await tp.system.prompt("Enter Kanban Name");
	await tp.file.rename(title);
} else {
	title = tp.file.title;
}
_%>

#kanbans 

## Backlog


## In Progress

## Finished

**Complete**


%% kanban:settings
```
{"kanban-plugin":"basic"}
```
%%
