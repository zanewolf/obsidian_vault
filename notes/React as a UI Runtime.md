by: Dan Abramov
Link: [React as UI Runtime](https://overreacted.io/react-as-a-ui-runtime/)
Keywords: [[React]] [[Hooks]][[UI]]

- a runtime system implements portions of the execution model, in other words, it is  executed while the program is running. In addition to any code, there could be higher-level support such as debugging, type checking, optimization, etc
	- a necessary for declarative coding (tell code what you want to do vs exactly how to do it)
	- browser runtime versus library runtime
	- 


# Notes
- Host Tree
	- react is based on two key principles:
		- stability
			- the bulk of the site stays unchanged while updating only the specific things that did
		- regularity
			- all the ui components can be broken down into the same basic building blocks
- Host instances
	- are the individual elements that appear on the screen, aka nodes, and these nodes have their own properties (like classnames) and functions/APIs to manipulate them (e.g. appendChild)
		- these APIs are how React interacts with nodes
- Renderers
	- a renderer teaches react how to interact with the host environment
	- two types/modes
		- mutating mode
			- APIs like appendChild to update notes in place
		- persistent mode
			- clone the parent tree and create new instance of child, rather than update old one
- React Elements
	- react elements, the smallest building blocks, are immutable - you can't change one building block into another. 
- Entry Point
	- spot where you tell react to add a particular react element to the host instance
	- ReactDOM.render(reactElement,domContainer) = dear react, make the dom container host tree match my react element
- Reconciliation
	- reconciliation is the process of figuring out what to do to the host instance tree in response to new information. 
		- could trash existing tree and recreate it from scratch (persistent?) or update (mutate?)
		- if the new element matches with an old element in the same place ('same identity'), react just updates the old one
- Conditions
	- get around the problem of moving/displaying new items above old ones with conditions
		- create it, but don't show it until some condition is met. Then the item that was first shown isn't moved/bumped down to be recreated, it's just that the item above it was updated, not created
- Lists
	- this is why keys are important in react lists - they give react a way to compare the identities in case the lists are reordered. If the key is the same, don't create a new one, just update position
- Components
	- functions that return react elements are components
	- take in one item: props
- Purity
	- local mutation is fine
	- but merely calling a component shouldn't by itself produce change on the screen. That should happen once the component has finished, and not during. Bad UI? 
- Idempotence??
- Recursion
	- react is continually calling on components to see what they render, and since components normally are stacked (A renders B, B renders C, etc), this calling tree is recursive
	- reconciliation is recursive
- Inversion of Control
	- we call components like <App/> because calling them directly (App()) means that you are bypassing React's API and calling them yourself. With the bracket notation, you are telling React there is a component here, and letting it take control of when/how it is called
	- because of this
		- components become more than functions, and have features tied to them that wouldn't be tied to normal functions (adding the react API to them?)
		- component types participate in the reconciliation. Otherwise you'd have to have the recursion calling manually coded, react wouldn't do it for you
		- react can delay the reconciliation
			- only update when the component is finished calling
		- debugging is better -> lazy evaulation
- Lazy Evaluation
	- or rather smart evaluation. React knows how/when to render components or not. If we called them manually, they would always render, whether or not we wanted them to
- State
	- react gives components/host instances their own version of local state, than can be used to update them. These instances of local state are called Hooks
- Consistency
	- so user doesn't seem some half-baked site during rerender, react has two phases
		- render phase
			- components are called and reconciliation happens
				- safe to interrupt, asynchronous
		- commit phase
			- react touches/updates the host tree
			- synchronous
- Memoization
	- with big trees, updating a local state can have large and deep rippled affects on nest components. If something will NOT update with local state changes, you can sequester those off with memoization - telling react that the state changes didn't affect this item and to not waste time checking it 
		- like if you update a table header but the individual rows are unchanged
		- there is a useMemo() hook
- Raw Models
	- any top-level state changes trigger a whole-tree reconciliation
	- even if everything stays the same except for one tiny little thing, the reconciliation process still has to run through the entire tree and compare
	- fine-grain updating loopholes exist, but React wouldn't be the best framework if you want something that updates consistently (like a graph charting live stock prices. Just the chart is changing, but every little change would trigger a whole-site reconciliation)
	- Two problems: 
		- making page transitions without blocking the browser
		- have to wait for data to reach server before we cans tart rendering the view
	- both are solved with concurrent rendering
- Batching
	- batch state updates for only one re-render procress
	- useReducer is a good way to batch state updates
- Call Tree
	- react keeps track of everything that was called during the making of the dom, because it needs to keep local state somewhere in order to reference any changes/updates
	- the call tree is updated/destroyed after reconciliation, replaced with a new one
	- Fibers are these different versions of the call trees
		- React marks the fibers whose state changed, and then just those components are rerendered
- Context
	- a wormhole to drop props into just components that need them, rather than passing them all along through the tree
- Effects
	- when you DO want side effects to appear to the user while a component is rerendering, you can use side (use)Effects
- Custom Hooks
	- let different components share reusable stateful logic
- Static Use Order
	- hooks can only be called at the top of the component tree 