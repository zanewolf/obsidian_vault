tags: 
[Link](https://overreacted.io/the-elements-of-ui-engineering/)

## Notes
- general article is about the most problematic areas of creating a UI and how he's created custom exercises to get better acquainted with solving them
- Most languages and whatever happens to be in vogue will have to deal with these issues
	- learn more about libraries and packages along the way 
- Problems
	- **Consistency** :
		-  i.e. not forgetting what the user has done on one way if they navigate away and come back
	- **Responsiveness** : 
		- things can take a while to load, and if they do, do you show a loading page while that is happening to indicate that something is happening, or not since that can make the time period seem longer than it actually is? 
	- **Latency**: 
		- related to responsiveness, anytime you load new data, it'll take time, so same issues
	- **Navigation**: 
		- related to consistency, things should change in the room just because you left it, or are looking out the window. Need to retain context amid random navigation
	- **Staleness**: 
		- But when retaining context, what do you remember (cache)? Is there a time period for how long you should remember something? What things should be remembered for longer/shorter/not at all? 
	- **Entropy**: 
		- for every N options given to the user, there are $N*(N-1)$ possible states for the code to handle. Will they all work in combination together? Will bugs happen? How do you account for every possible state in the code that will probably happen at some point? 
	- **Priority**: 
		- with various functions happening, various inputs from users, various code written from different coders - what gets to use the limited resources (network, processor, screen size) first? 
	- **Accessibility**: 
		- Some disability is eyesight focused (red-green colorblind, dyslexic, can't pick up on low contrast), but some is tactile (can't use a mouse, is the website navigable using a keyboard?)
	- **Internationalization**: 
		- How do we support not just different latin languages but right-to-left languages without sacrificing latency and responsiveness? 
	- **Delivery**: 
		- Do we load everything initialially (so large package size) or only load as the user needs (which might slow down use)? 
	- **Resiliency**: 
		- A failure to render/load one blog post, for example, shouldn't crash the entire side. There needs to be a certain amount of isolation so that if one brick cracks, the entire house doesn't come crashing down
	- **Abstraction**: 
		- If multiple people are working on well-defined and separate parts of the code, how do you prevent multiple solutions to deal with the same problem, and unnecessary/conflicting redundancy? 
		- That seems easy, talk to each other
- Try to solve these without libraries in order to really gain understanding and key experience first

## Meeting Notes
- Goal: 
- abstractions and generalizations
	- all abstractions are generals but not the other way around

- project: define programming language
- timeline for running an app, phases? dev mode? production mode: removal of node app server?
- lifecycle
- 