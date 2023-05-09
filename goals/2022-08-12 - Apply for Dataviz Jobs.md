---
tags: goal
alias: Apply for Dataviz Jobs
Type: Professional
Progress: 0
Target: 5
Reason: I need to apply for jobs, and 5 seems like a good starting number. 
Timespan:  1 Month
---
%%
Bar:: `$= dv.view('progress-bar', {file: '2022-08-12 - Apply for Dataviz Jobs'})`
Projects:: `$= const projects = dv.page('2022-08-12 - Apply for Dataviz Jobs').file.inlinks.where(p => { const mp = dv.page(p.path); return mp.tags?.contains('project') && mp.status === 'In Progress'}); if (projects.length > 0) { dv.header(4, projects.length > 1 ? "Projects" : "Project"); dv.list(projects) }`
%%


## What does success look like? What are the key results?
- the preliminary key result is having just applied to the target number of jobs. 
- ultimatley success looks like having found a job

## Meeting Notes 
```dataview
TABLE Summary AS Summaries
from #job
SORT file.name desc
```
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


