---
banner: "media/banners/mountains.png"
banner_x: 0.90697
cssclass: cards
---

## Inbox 

- Swimmer's Plot, add to visual vocabulary
 ```dataview 
 TABLE file.cday as Created, file.tasks 
 WHERE contains(tags,"🌱")
 SORT file.size 
 DESC limit 10 
 ```

## Boards

- [[Goal_Board]]
- [[Project_Board]]
- [[Adventure_Board]]

# Active Projects

```dataview
table status
FROM "projects"
WHERE status = "Active"
SORT deadline desc
```

## Topic Indices
- [[1_Dataviz_MOC]]
- [[React]]




# Obsidian Activity 


> [!multi-column]
>
>> [!note]+ Recently Edited
>> ```dataview 
LIST FROM "" 
SORT file.mtime 
DESC LIMIT 5
>
>> [!note]+ Recently Created
>> ```dataview
list FROM ""
sort file.ctime DESC
LIMIT 5

```start-multi-column  
ID: ExampleRegion1  
number of columns: 2  
largest column: left  
```

Text displayed in column 1.

--- end-column ---

Text displayed in column 2.

=== end-multi-column

## Resources
### Symbols
 Δ  Meeting Notes
 Ꝓ  Project Page
 §  Query/Search Page
 λ  Literature Note
 


```dataviewjs

let ftMd = dv.pages("").file.sort(t => t.cday)[0]
let total = parseInt([new Date() - ftMd.ctime] / (60*60*24*1000))
let totalDays = "You have been using *Obsidian* for "+total+" days,"
let nofold = '!"misc/templates"'
let allFile = dv.pages(nofold).file
let totalMd = " with "+
	allFile.length+" notes, "
let totalTag = allFile.etags.distinct().length+" tags, "
let totalTask = allFile.tasks.length+" tasks created. "
dv.paragraph(
	totalDays+totalMd+""+totalTag+""+totalTask
)

```
 
 