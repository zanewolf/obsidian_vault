![[VisualVocab.png]]

[Data Viz Project](https://datavizproject.com/)
[Visualization Zoo Tour](https://homes.cs.washington.edu/~jheer/files/zoo/)

## Bar vs Lollipop
Bar charts can easily be replaced with lollipop charts with no loss of understanding. Lollipop charts remove the Moire effect present between bars (a type of optical illusion) and remove chart clutter/maximize data-ink ratio since the stick of the lollipop has much less area than a bar. 

## Small Multiples
[How Pew Research Center uses small multiple charts](https://medium.com/pew-research-center-decoded/how-pew-research-center-uses-small-multiple-charts-2531bfc06419) 
- > Small multiples often require more time for a reader to fully absorb than single panel information graphics, and any information graphics that require close study are not the ideal format to use for audiences with very limited time or attention. But for those readers who do have time and attention, a carefully designed set of small multiples can communicate a lot of information.
- Think facet-wrap/facet-grid.
- It's a way of displaying the same information but repetitively to enhance comparison. This can also enhance readability, if lots of the information, if plotted together, would overlap. 
- Common guidelines: 
	- use a title to highlight key finding, since there will most likely be several small ones, too
	- Use the same scale and style across the multiples - otherwise comparison because hard if not worthless
	- a reference line can help
	- Choose the order intentionally - not random or alphabetical unless alphabetical is useful(?)
	- annotations can help point out the significance of differences

Information below from [19 Innovative Ways to Use Information Visualization Across a Variety of Fields](https://towardsdatascience.com/19-innovative-ways-to-use-information-visualization-across-a-variety-of-fields-edba0613136d), though this article does seem to mostly be about defining different chart types

## Stream Graph
- a variety of a stacked area graph, with no main axis
- work great for when you want to show one variable against time, grouped by category 

## Sankey Diagram
- used to visualize quantitative flows and their proportion to one another
- useful as a large diagram or in small multiples
- best if your data is about a process or flow of values. It doesn't have to be over time, but there is an aspect of "evolution"

## Chord Diagram
- used to visualize inter-relationships between different groups
- can be confusing if there are too many variables - use interactivity to sort things out rather than layering
- use only if you have the time to explain it to your audience, who might otherwise be unfamiliar with it

## Choropleth Map
- a single variable or piece of information as it pertains to a map
- use if geographic location is pertinent
- use normalized data instead of raw, since most data will simply scale with population centers. Normalize to population to plot meaningful data

## Hex Map 
- essentially the same as a choropleth but removes area from consideration by making all regions the same size hex

## Interactive Polygon Map
- just like a hex, but shows a three-sided cube that can display three pieces of information/variables instead of just one
- the values shown are categorical (e.g. top 3 categories per state, bottom 3 categories per state), not percentages or normalized values

## Ridgeline Plot
- aka joyplots
- a density chart that shows distributions over several groups
- when you want your data to be easily read and visually rich
- order needs to be chosen purposefully, so that important data remains visible rather than accidentally hidden by the layering


## Boxplot
- visualizes data distribution and variability
- good for comparing the values, especially if it is symmetrica or skewed, and is a great way of showing outliers

## Treemaps
- a type of hierarchical chart that shows the value of things in different categories

personally not a huge fan, as they can difficult to decipher. But a good way of packing a lot of data into a small area

## Isochrone Plot
Meaning "equal time", these types of plots are great when you want to visualize how far/much you could do in the same amount of time. E.g., how far you can travel from one city in an hour. How many 

	