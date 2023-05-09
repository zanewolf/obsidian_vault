## What is it
This is a challenge undertaken voluntary by people wishing to evolve their coding skills at an accelerated rate. I'm choosing to do this for two purposes: to evolve my coding skills at an accelerated rate, and build up my portfolio so that when I apply to the Fathon Info internship, I can show that I have pursued dataviz at my own leisure, working to master skills and a variety of tools beyond what was taught in CS 171. 

**bold things**

## List of Softwares/Packages/Practices to Learn
- JQuery
- Sass
- Typscript
- Vue
- React
- Testing
- Next.js (react framework)

## Goals
- Revisit and hone d3 skills
- Learn to combine Vue.js and d3
- Create [[Data Art]] (i.e. something static)
- Learn text analysis 
- Learn web scraping
Bonus: 
- Create a react app

### Day 1
I read On the Nose by Hans Florine this morning and the first Appendix is a summary of all of his climbs: MM/YY (and then MM/DD/YY in more recent years), companions, and time. Only climbes less than four hours have HH:MM:SS data, all others range from HH:MM to HH+ to X Days. 

I decided to see if I could visualize this in a fun way. 

Inputting the data into an excel spreadsheet
- I had two columns for date, the full date if available and the shortened date for all, just in case I wanted to do something with the recent dates. 
- The time I inputted as HH:MM, and if the time was simply listed as 3 Days, then I inputted it as 72 hours even. 
- There was an individual column for each Partner's name (never exceeded 6) and a column for just the total number of partners. 
- There was also a column describing if it was a special event (e.g. birthday, fundraiser climb). 
- And finally, a column denoting if the climb set a new record and which one

First I need to decide what I want to make? A single visualization? A dashboard? An infographic? 

I'm thinking a single interactive visualization. Forced Layout bubble chart c. CS171 Marvels? Show grouping by record-setting, partners, duration (rounded to hour), event type

What I accomplished today: 
- collected data from the book and inputted into excel/csv
- set up project directory and repo
- formatted the time into a date object, extracted month/year
- rounded time on wall to hours

Do I want to show percentage of climbers by gender? I can easily add that? Maybe. 

Next steps for tomorrow: 
- set up pipeline for bubblechart
	- object, init/wrangle/updateVis
- update index.html styling 
- try to get at least one static version of the bubble chart going

## Day 2

Setting up the pipeline for the bubble chart. Looking at Marvel's, they inputted four different data structures, one for each phase. I am not sure if I need to do that or I can simply define the four phases in wrangleData. So I guess the first thing I need to do is figure out what format the data needs to be in for the bubble chart. 

It looks like they hardcoded the coordinates for each bubble for each stage. I'm not about that. 

Found a new example: https://bl.ocks.org/SpaceActuary/d6b5ca8e5fb17842d652d0de21e88a05

So what information do I want encoded in the clusters? 
size => hour (rounded)
color => year? roughly 30 years
color => # partners (only 5)
color => redundant with hour?  0-3, 4-6, 7-12, 13-24, 25-48, 48+ 
color => random? This feels like a waste, since we naturally want to perceive color as meaningful first. 

Redundant seems like the best option. 

Set up the pipeline for bubblechart and imported the spaceActuary example. Has errors, but at least it appears. Now to tinker and see if I can get it to work tomorrow. 

Today I accomplished: 
- updated the html styling from the boilerplate styling
- finding a good example of the visualization I'm shooting for
- downloading and integrating that example from observable into the project directory

Tomorrow I would like to accomplish: 
- debug the example code
- begin applying it to bubbleVis

## Day 3 - 8

React.js Bootcamp

Learning 
- Props
- Rendering Lists
- State
- Functional Components
- PropTypes
- Api integration
- Children
- Higher Order Components
- Render Props
- React Router
- Query
- Class Fields
- 