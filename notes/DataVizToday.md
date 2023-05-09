# Notes from the Podcast 
### Episode 2
- the three different goals of dataviz can be grouped into **Attention & Beauty**, **Understanding**, and **Implication**
- These are not mutually exclusive goals, but more stepwise
	- **Attention and Beauty**: grab their attention and encourage them to continue looking at the visualization, engage multiple senses if possible to attract people with different learning types. Essentially the first impression.
	- **Understanding**: After they decide to stick around, this is where they start to explore and understand the information, and we have a chance to explain cool bits/key takeways. 
	- **Implication**: Convince the reader that what you've said is true, try to convince them to believe you and your information over what they may want to believe, and evoke feelings. Put the takeaways in context, connect it to the reader personally 
- Titles and text in dataviz are key elements to help people understand the recall the viz - what do you want them to remember? Make that the title
- People prefer images with curved edges rather than sharp edges, and this was determined through looking at MRI brain scans as people where shown images. 
- If you have data over time, it's always worth checking for seasonality
### Episode 3
- When trying to find a story in data about [[movement]]: 
	- define the characters
	- Define the attributes of the characters
	- how are the characters grouped/categorized
	- Now visually represent your characters and attributes and notice how they move from different categories as time passes and events happen
### Episode 4
- when dealing with survey results, is there a way to break the participants into groups based on their answer to one question
	- e.g. with Shirley Wu's analysis looking at dataviz, she split the responses into those that responded they were frustrated with something in dataviz and those that said they weren't. And she used this grouping as a lens through which to look at the rest of their responses 

### Episode 5
- draw inspiration from art

### Episode 7 
- annotations are extra layer of information on top of a visualization the provides context and directs readers to points of interest
- there's a visual hierarchy to annotations that dictates what the reader will notice first
	- Headers
	- lead-in-text below the header that describes more details about the data
	- subheader and explanatory text within the chart that can use circles/arrows/lines to call attention to the points of interest
- Use annotations to explain non-obvious things to the reader, like how to interpret specific graphical or statistical elements
- Can also annotate high-low values, outliers, averages, events in time, group items with similar attributes, totals/subtotals, notes with expert interpretations, axes interpretations, etc. 
- Susie Lu built her own library for customizing annotations [D3 Annotations](https://d3-annotation.susielu.com/)

### Episode 9 
- Readers don't care about full data, show them the key bits
- focus on the "near view" - a specific experience that people can relate to 

### Episode 10 
- document your design decisions, why you went with X and not Y 
- when deciding on a particular visualization, go through the pros and cons
	- a bar chart would show x but lose y, which is important to show because
	- a (blank) chart would show x and y, but not the relationship between the two is muddy
	- using this color scale versus that color scale
- being able to effectively communicate design decisions and why they were better than the alternatives would help [[clients]] trust your abilities

### Episode 11
- don't get psyched out about the learning curve of a specific technology or technique
- if trying to engage audience in something they might have zero interest in, like sports, focus on strategy and nuance, something small but specific to the sport

### Episode 12
- if your data doesn't make sense with a basic chart, then it won't make sense with a more complicated chart
- Exploratory Viz: 
	- Pros: you give the reader the power to ask their own questions and find their own answers, personalize their experience, and can help communicate the complexity of the data and mitigate some of the biases when you push your own narrative
	- Cons: for a static viz, there is a lot of restrictions about what you can show, and it requires time and attention from the reader. Will your effort be worth the amount of effort your audience is willing to expend? 
	- You can give the reader control of three things: 
		- View - the ways in which the data is shown to the reader
		- Focus - the subject of the story, the ability to subset the data
		- Sequence - the order in which the information in the story is viewed

### Episode 13
- spatial data is easy for audiences to relate to since they have a innate knowledge of where they are at any given point

### Episode 14
- a visual metaphor is the representation of a person, place, thing, or idea by means of a visual image that suggests a particular association or point of similarity 
- one way to find metaphors is to create two separate lists and then combine items from each list into different combinations. 
	- e.g. war and nature might combine into death = flowers
	- [Visual Metaphor](visualmetaphor.com) to help create combo
- Using metapho can help readers use their existing knowledge to explain the unfamiliar

### Episode 15
- Building a predictive model is both really complicated and really exciting.
- Conveying uncertainty is crucial both visually and when reporting results.
- Annotation and clean formatting go a long way in making visualizations that anyone can understand.

### Episode 16
- Can use simulatiions/what-if analyses 
	- pros: 
		- no risk
		- can assess the weaknesses and opportunities quickly
		- can make it easier ot make decisiona dns et goals
	- decide on the factors you want to vary, what you want to see affected, and the formula that combines these factors
	- examples
		- forecasting sales
		- home buying affordability
	- useful when big change is coming, or if you want to propose change, 

### Episode 17
- 3 ways to amp up scatter plot include 
	- add lines that help orient reader quickly, such as median for x and y axes 
	- and label the quadrants
	- use color, size, or small multiples to present a third variable. Fourth variables get super complicated. Use color and size to represent the same variable to build in understanding redundancy 
### Episode 18
- Passion Projects
	- write down what skills you want to improve
	- write another lis of unique experiences you're passionate about and things that bring out emotion 
	- combine things from this list, think about the experience youw ant to have when doing this project
	- write out what success looks like to you 
### Episode 19
- Ways to review your viz
	- read it out loud
	- print it out
	- change your scenery 
	- image what the best compliment could be 
	- pretend to start over and redo your decisions - would you make the same choice, why or why not? 
	- ask someone else
### Episode 20
- isochrone maps 
### Episode 21
- you can visually break a line chart up by color, weight, vertical lines to draw attention to specific intervals that are meaningful 
- e.g. unemployment rate over time by presidential term 
### Episode 22
### Episode 23
- if you have data over time, think about whether visualizing a hot streak could reveal any useful patterns or insight
- line up your data with the same start and end points and stack them up 

### Episode 24
- Before accepting free work, ask yourself three questions
	- where does this fall on the ladder to your ideal job? Would this free project help you get closer to your goal? 
	- Could you turn this into a passion project instead for similar or better exposure? 
		- rather than give product to a newspaper to display for free, for example, could you get similar exposure by disseminating it yourself
			- by posting it yourself, you retain creative control and get to view all the metrics of views and engagement
	- Can this person or company afford to pay you for this work? Are they making money off of your efforts? 
		- If they can afford to pay you AND they are making money (selling a product or issues, saving money through increased efficiency), then they should pay you, or maybe give you a trade (interview, access to data, etc)
		- If both are those are yes but you really care about the company, then it might still be worth it to you to do it for free
	
### Episode 25
- to make a viz more inviting 
	- recreate maps using your preferred color palette
	- use icons instead of labels
		- pros: save real restate, more quickly scanned
		- cons: need to be easily understandable and can be cluttered

### Episode 26
- when designing your viz, ask yourself three questions:
	- I: Impression
		- what feelings or emotions is it bringing out in me? 
	- R: Readability
		- what makes it easy (or hard) to read? 
	- A: Allure
		- what makes this viz stand out or unique? 
- dont be discouraged if your work doesn't match your aesthetic taste. Keep practicing and it will. 

### Episode 27
### Episode 28
- always consider making a unique visualization (not a standard/defined chart) for your data, especially if it is naturally visually appealing 
- can be done using illustrator, too

### Episode 29
- defining your own style can be tricky
- check out style guides 
- define your most common audience, who you tend to design for
- build inspiration boards of art, viz, even furniture 

### Episode 30
- if you are having trouble designing or remaking a vis, ask three things
	- what is the goal? What do you want to learn from the viz? 
	- What are you seeing? What is the context? What are things you can measure and display that would inform you about the goal? 
	- What is causing the problem? What could you measure that would inform you when things are not going as planned? 
	- 
### Episode 31
- problems with 3D include occlusion and perspective distortion (things farther away seem smaller)
- However, 3D is great for understanding shape

### Episode 32
- 3 specific interaction techniques, to engage the reader and teach them something they'll remember by giving them control over the narrative
	- allowing them to reveal or draw a chart themselves
	- give them a  choice of the example they explore
	- allow them to walk through and build up a complex viz at their own pace

### Episode 33
- to find the story in the dataviz
	- avoid the obvious. you want to focus on the drama, conflict, and tension, but what's the use of visualizing something that everyone already knows
	- make it timely. you either need a fresh angle on an old issue or a reason why now is the time to take notice
	- clarify your emotional arc
		- start with delight, end with wisdom
		- ![[datavizstory.png]]
		
### Episode 34
- boxplot are a way of visualizing distrubtion of points and a way to compare that distribution across many gorups. If you are using a more complex/academic viz, consider priming the audience with a little lesson in how to read the chart

### Episode 35
- three techniques to handle overplotting
	- try aggregating the data
	- convey where the denisty of your data is by adding a distribution chart to the margin of the scatterplot, or a contour plot
	- add jitter, or use [gatherplot](https://arxiv.org/pdf/1708.08033.pdf)
	
### Episode 36
- how to create a new type of visualization
	- identify the problem in data anlaysis
	- find an analytical tool that solves this problem
	- use a visual metaphor to explore and communicate the results
	
### Episode 37
- RJ has found that the essential components for a creative routine are:
	-  periods of gathering lots of information and then
	-  move into a period of light exercise or rest where you can kind of free your mind to free associate the ideas that you just collected and then 
	- carve out time periods in your day where you can enter a creative flow state.
	- Then when you do have a creative idea, try sketching it out. First, the benefits are that you can explore the form of your idea rather than the technical aspect of what you can and can't do in a certain tool and your idea doesn't get influenced by your tool knowledge. It has the benefit of also looking unfinished so you can more easily focus someone's attention like your client on your specific idea and when you're trying to maximize your creativity under a deadline. Know that this calls for heavy engagement from your client so that you can rapidly prototype and make sure to limit your scope, start working to train your clients to understand that data is as hard and they need to budget time for it.


### Episode 38
- three reasons writing can help you improve
	- it's a creative outlet over which you have complete control
	- when you write and share, you are inviting others to engage
	- you learn more about yourself and the topic by trying to write about it
	- career builder, creating a body of work
- three tips to making writing easier
	- announce a schedule (and keep it!)
		- e.g. publish a new blog every Tuesday
	- narrow down your audience, keep the topic tight to something that you love, and the audience will be there
	- create a template
		- e.g. four blogs a month: a new technique you learned, your process behind a new viz, your opinion on something in the news, and your favorite viz that month


### Episode 39
- three design tweaks that make a huge difference
	- align everything on the page with something else
	- think about text hierarchy
	- keep annotations simple


### Episode 40
- if the main story is the flow of animation, that doesn't mean you have to leave out contextual information. You can integrate small multiples into the structure and give your audience the benefit of seeing the overall flow and extra details

### Episode 41
- designing without color (or in monochrome) lets you really focus on the data first, see the individual elements and the spacing
- have a conversation about what color works for which elements, not a conversation about why you chose yellow
- think HOW not WHICH. How will color improve my reader's understanding? 
- you can get the most out of no color/monochrome palettes by also using techniques like glow/shadow/patterns
- think of monochrome palettes as a limited resource, to be used/allocated/partitioned wisely

### Episode 42
- duncan clarke portfolio tip??

### Episode 43
- try a storyline or narrative chart if you want to visualize events happening over time and how many people were involved in those events

### Episode 44
- use dataviz to help people feel more connected, make badges, help them find themselves and people they know
- 

### Episode 45


### Episode 46
- building a portofolio tips
	- before you start putting together your portfolio, do a little bit of research on people's portfolio in your desired field or position and see what's working for them.
	- Add your images and then whether you add one sentence or one page of text, make sure your text is about the value you brought to the client with your work.
	- Do not over optimize your portfolio. Make sure your portfolio is on par with others in your field and then use the rest of your time making connections with real-life people.
- Good artists copy, great artists steal

### Episode 47

### Episode 48

### Episode 49

### Episode 50