by: Dan Abramov
Link: [Article](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)
Keywords: [[React]][[Hooks]]

# Notes
- Why Hooks? 
	- they apply explicit data flow and composition inside a component, just not between components
	- they don't require unnecessary nesting or suffer from drawbacks of mixins
	- hooks let you always use functions instead of having to switch between functions, classes, higher-order components, and render props
	- a good way to reuse code that doesn't need to render UI (which is what separates a component - something that must return a UI piece - from render props and HOCs)
		- functions don't need to render UI and can be reused, but you can have local React state inside them
- what are hooks exactly? 
	- they let you use react features (like state) from a function
	- they are not a way to share state, but a way to show stateful logic
	- you can pass data between hooks, because they are ultimately js functions and you can feed in info to the function
		- this makes them great options for animations, data subscriptions, form management, and other stateful abstractions
		- 
