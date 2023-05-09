# Process Book Template
# Overview
## Description
To visualize the first 100+ climbs Hans Florine has completed on the Nose in Yosemite Valley, as self-documented in the appendix of his book, On The Nose, I am going to try my hand at creating a bubble chart. 


## Detailed Project Plan
- Background and Motivation
	- Pure curiosity and interest in making a bubble chart. 
- Related Work or Inspiration
- Audience
	- What do they know? What are their interests? What visualization literacy do they have? etc.
		- This work is intended for a climbing audience that is familiar with the race for the nose record and Hans Florine. 
		- There will be little in the way of exposition in the visualization itself
- Questions
	- How many climbs of the 100+ recorded in the book were record-setting, and of what record? 
	- Is there a correlation between time and number of partners? 
- Data
	- Hand-collected from the appendix in On The Nose
- Data Cleanup 
	- Little atm. 
- What is the final product? 
	- A bubble chart that the viewer can step through 


# Map
- Table of variables (categorical, quantitative, ordinal)
- List of questions
 # Exploration 
## Key takeaways from data
# Sketch
Sketch ideal visualization for takeaways, standard and non-standard. 

# Journal
### 2/6/2021
I am using a combination of this source and that source to try to figure out how the bubble chart works and make my own without directly copying my own data into these frameworks. 

So far I can get graph the initial nodes but the application of the force simulation properties is tricky and I haven't figured it out yet. 
![[OnTheNose_chargefail.png]]

### 2/7/2021

Figured out how to update x/y positioning based on record statis
![[OnTheNose_code_force.png]]
![[OnTheNose_records.png]]
Now I need to figure out how to decentralize everything so that it's not one massive if statement. Maybe just one. 

## 2./9/2021

Yesterday I placed all the years according to my swiggly timeline pattern, but got stuck when trying to figure out the best way to approach the cubic bezier curves. 
![[OnTheNose_yearwinding.png]]
Tonight, I got my line plotting but try as I might I could NOT get the curves to work with me. 
![[OnTheNose_bezierfail.png]]
![[OnTheNose_bezierfail2.png]]

Even giving the curves the same x,y coordinates as the years was a headache because they didn't match up!

So I'm changing gears and am going to do a simple linear timeline across the middle of the svg. Should be a LOT easier to calculate. 

# Prototype
# Test 
# Publish
