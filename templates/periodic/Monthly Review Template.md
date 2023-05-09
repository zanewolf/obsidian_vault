Status:
Tags: <% tp.file.cursor(3) %>
Links: [[<% tp.file.cursor(4) %>
___

# Monthly Review Template
<% tp.file.cursor(5) %>
___
References:

Created:: 2023-05-04 10:29---
deadline:
hibernating:
completed:
---
Tags: #projects/
Links: [[~ Projects]]
___
# Monthly Review Template
## Progress
%% include period and project name in select-tags field %%
### To Do
```tq
group: due
select-tags: tq/p/
sort: due
completed: false

```
### Finished
```tq
group: due
select-tags: tq/p/
sort: due
completed: true

```
## Details
> Refer to the [[HORNIERR Goals]] framework

**Helpful**
- 

**Objective**
- 

**Roadblocks**
- 

**Naivety**
- 

**Insights**
- 
## Execution
- [ ] Implement execution into tq and habitica
### To Do's
**Big:**
- 

**Medium::**
- 

**Small:**
- 
### Dailies
**Big:**
- 

**Medium::**
- 

**Small:**
- 
### Habits
- 
## Resources

___
Created:: 2023-05-04 10:29Status:
Tags: [[<%tp.date.now("YYYY-[Q]")%><% tp.file.cursor(0) %>]] #monthlyReview
Links: [[Monthly Reviews]]
___
# <% tp.file.title %>
[[<%tp.date.now("YYYY-[M]MM", -45)%>]] <== This Month ==> [[<%tp.date.now("YYYY-[M]MM", 45)%>]]
- [ ] Remind yourself about the plans in higher-view reviews

> “Your decisions about allocating your personal time, energy, and talent ultimately shape your life’s strategy.”
## Weeks
```dataview
table Sentence, Happiness, Productivity, Relationships, Focus
from #weeklyReview  AND [[<%tp.date.now("YYYY-[M]MM")%>]]
sort file.name asc
```
## Reflection
Sentence:: 
### Ratings (Out of 10)
Happiness::
Productivity::
Relationships::
Focus::
### Events
**Biggest Personal Milestone**:: 

**Biggest Career Milestone**:: 
### Projects
#### Book Implementation
**Did I commit to my weekly implementation?**
- 

**Is there anything I would like to continue doing?**
- 
#### Career
##### Project - 
**What did I accomplish?**
- 

**Am I satisfied with my progress?**
- 

**What setbacks did I face?**
- 

**What are some possible improvements and plans for next week?**
- 
#### Personal
##### Project - 
**What did I accomplish?**
- 

**Am I satisfied with my progress?**
- 

**What setbacks did I face?**
- 

**What are some possible improvements and plans for next week?**
- 
#### Misc
- 
## Overview
### Key Metrics
Week 1-
Week 2-
Week 3-
Week 4-
Total Hours:
Hours average: 
Thoughts?
### Prompts
**Did you complete what you set out to do in the previous weekly review? Are you content?**
- 

**Does your calendar (and commitments) match your priorities and values?**
- 

**What was the completion rate of my projects? How was the workload?**
- 

**Did I do something outside of my plans? How did it influence the week?**
- 

### What Went Good?
- 
### What Went Bad?
- 
### The Learned
**What is one valuable lesson?**
- 

**What can I improve on?**
- 

**What should I start/stop doing?**
- 

## Future Plan
> **Focus on**: 
### Book Implementation
**Choose a book and create:**
- One to do, daily, and habit for the week
	1. 
	1. 
	1. 
- Two reflection questions to ask myself every day
	1. 
	1. 
### Action
> ***Be throrough in planning!***
- [ ] Come up with projects for the week
	- Consider someday/maybe list
- [ ] Integrate the tasks into habitica and tq
#### Projects
**Career:**
- 

**Personal:**
- 
___
References:

Created:: <% tp.date.now("YYYY-MM-DD HH:mm") %>
