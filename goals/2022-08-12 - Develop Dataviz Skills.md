---
tags: goal
alias: Develop Dataviz Skills
Type: Professional
Progress: 5
Target: 10
Reason: Because I want to develop these skills and make myself more competitive for dataviz jobs
Timespan:  6 Months
---
%%
Bar:: `$= dv.view('progress-bar', {file: '2022-08-12 - Develop Dataviz Skills'})`
Projects:: `$= const projects = dv.page('2022-08-12 - Develop Dataviz Skills').file.inlinks.where(p => { const mp = dv.page(p.path); return mp.tags?.contains('project') && mp.status === 'In Progress'}); if (projects.length > 0) { dv.header(4, projects.length > 1 ? "Projects" : "Project"); dv.list(projects) }`
%%


## What does success look like? What are the key results?
- 


## Related core values
- 

## Projects to make this happen
### Ideas
- 

### Created projects
```dataviewjs
const pages = dv.current().file.inlinks.where(p => dv.page(p.path).tags?.contains('project'));

dv.table(["Project", "Status"], pages.map(p => {
	const page = dv.page(p.path); 
	return [page.file.link, page.status]
}));
```
