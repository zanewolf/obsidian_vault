# Overview
## Description
This is a different version of the group project [[Space Monkeys]] we did for CS 171. I felt dissatisfied with our story, and how redundant our visualizations were (three of them showed cumulative launches over time in some way/shape/form). We compromised a lot on the story in order to not create more visualization-work for us, and that left me with the desire to do this again, without those compromises.


## Detailed Project Plan
- Same as V1
- Specific Changes
	- Incorporate a dashboard
		- switchable between company and country
	- Provide some higher-order visualizations, i.e. not just show the raw data, but an analysis
	- Make the network visualization update-able 
		- will need to move treedata.js into wrangledata and simplify using *d3.groups*, which transforms it into an array, not a map
		- transformable into tree? 
			- apply time axis??? 
	- Make satellite vis update-able by date?
- one of my issues with V1 is that for the network vis, the original tagline that Mike/Juan gave it was "this is how the industry has changed over time" and that's not what the vis showed at all - it was the cumulative shape of the industry with no time axis whatsoever. It wasn't a snapshot of the current industry or of any specific time at all. If anyone had launched whenever, it was included. The launch vis showed involvement over time, and the brush viz had the capacity to show it if it were stacked. Hence the create of the stacked area chart. 


# Map
- Table of variables (categorical, quantitative, ordinal)
- List of questions
 # Exploration 
## Key takeaways from data
# Sketch
Sketch ideal visualization for takeaways, standard and non-standard. 

# Storyboard
# Prototype
## Project Journal
### Jan 3rd
Currently working on stackedVis and the main issue I'm encountering is getting the data into the format necessary for the stacked area chart. 

This is what I want the data to look like: ![[lab7stackedData.png]]
And this is where I'm at right now: ![[spaceMonkeysStackedData.png]]

So the data looks like it's in the right format. S

The error was partly in how d3.area() was defined, the x value. Changed it from d.data.key to d.data.year and this was the result: 
![[StackedArea-Step1.png]]
Changed the svg area and bottom margin. 
![[Pasted image 20210103170310.png]]

Added the top margin: 
![[Pasted image 20210103164718.png]]

I think the problem right now is with how I'm coding year. So I have the raw date/time/timezone for every flight. d.Datum. 

Fiddling around with the different parameters involved (how year is formatted, mostly, and year vs datum): got it! 
![[Pasted image 20210103183731.png]]

Jan 7th
![[Pasted image 20210107142455.png]]
This is the tooltip from the network vis and thought I'd use it to keep it consistent. However, I dislike that it obscures part of the graph. I might place the name in the top left corner near the y axis instead. Not sure what the tooltip would be best for then. 

# Test 
# Publish