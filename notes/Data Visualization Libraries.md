[Navigating the Wide World of Data Visualization Libraries](https://www.youtube.com/watch?v=_H8y6j42Q2w)
![[visualizationlibraries1.png]]
- API - how the code is written
	- Plain JS
		- framework-agnostic
		- flexible and ubiquitous
		- more imperative than declarative
	- JSON with callbacks
		- hybrid
		- use a single configuration js object is used, and can accept functions
		- more flexible
	- JSON
		- declared a configuration object, not instructions or functions
		- more declarative
		- serializable, can save as text files
		- more difficult to integrate with others		
	- Framework Specific
		- tied to a specific framework (e.g. react)
		- better integration with target codebase
		- need to learn framework
		- 
- Level of Abstraction 
	- Graphic Libraries
		- Processing, p5.js, Three.js, Two.js, Rought.js, etc
		- Graphics operations, draw, shading
		- very high expressivity
		- very high effort
		- does not know about data
		- you're job to intrepret the data graphically and make it, kind of like using a coding version of illustrator or affinity
	- Low-level Building Blocks
		- d3, d3-legend, d3-annotation, flubber, cola, dagre, visx, etc.
			- visx is similar to d3 but meshes well with react? 
		- Independent, with components and utilities that each provide a specific funciton (e.g. scale, axis, interpolation, shape)
		- combined flexibility to create a visualization
		- linked to data
		- can work with other libraries
	- Visualization Grammar
		- instead of referring to charts by shapes (bars, lines, circles), it providews a structure for defining each chart using the same language
		- ![[visgrammar.png]]
		- vega-lite, g2, muze, chart parts
		- a framework that provides a set of chart parts, a specific way to compose the parts together to describe a chart
		- no chart type
		- less likely to work with other libraries
		- can express a broad range of visualizations on it's own, and can fluidly switch between them for rapid exploration
	- High level building blocks
		- each comes with own components, often larger pieces compared to vis grammar
			- 'preassembled larger parts'
			- may include chart type
			- trade expressivity for convenience
			- a container + many series/layers
				- Line series, Bar series, Candlestick, beeswarm, etc
		- eCharts, highcharts, plotly, victory, react-vis, semiotic
	- Chart Templates
		- Chart.js, nivo
		- refer to component by chart types
		- often ready to use, straight out of the box
		- less customization or optimization
	- Not uncommon for libraries to have multiple levels of abstractions
		- dc.js has both chart templates and high-level building blocks
		- g2plot is chart templates on top of g2 grammar
		- react-vis has both high-level building blocks and chart templates
- Choosing a library depends on your visualization type (common, rare, custom) and extra requirements (performance, special effects), how much time you have (due tomorrow, due in a week or month), project lifespan, and target tech stack (maintained in long term, or only made once and done? ), and experience (do you have to learn coding first)

![[vislibraries2.png]]

**https://www.slideshare.net/kristw/navigating-the-wide-world-of-data-visualization-libraries**
**Figma is great for collaboration.**

