# Workshop JavaScript Deep Dive

## Program

* Motivation for deep diving in JavaScript 
* Theory based on two demo's: a functional - and an object-oriented one
* Practical applications in a SvelteKit Project

### Motivation for deep diving in JavaScript

* Making it more fun to write JavaScript
* Needed skills to land a job:  [10 Interview Questions Every JavaScript Developer Should Know in 2024] 
> closure, pure function, promise, typescript, webcomponent, react hook, etc.
* How to handle your Imposter Syndrome
* How to handle bro coding culture, how to survive the complexity of the web 
> poggen flexen met ingewikkelde code

// React heeft de code base verandert van oop naar functional

### Theory based on two demo's: a functional - and an object-oriented one

The main concepts derived from the code:
* Fundamentals of JavaScript (Constructor Functions, Context(this), Scope) 
> context = objecten, scope = functies en blocks
* Functions and Closures (Callbacks, Returning Functions, Binding Functions)
* Array Manipulation and Logical Operations (Array Methods, Short-Circuiting, Event Delegation)
* Async Programming in JavaScript (Promises, Async/Await)
* Code Flow and Control Structures (Defensive Programming, Return Early, object destructuring, spread operator)
* Advanced JavaScript Concepts (Chaining Methods, Concurrency Model, Event Loop (Call Stack, Event Queue, and Microtask Queue), Hoisting, Closure)


Topics we encounter when using the debugger from the **Sources** tab in DevTools:
* Application state
* Scope 
* Context (this)
* Call Stack (Concurrency Model / Single thread)
* Extra: modules (scoped, deferred, async)


### Practical applications in a SvelteKit Project

Opdracht Refactor your JavaScript:
* Object destructuring
* Short circuiting
* Spread operator
* One responsibility rule for functions
* Pseudo-Private Custom Properties (CSS) // een private property, gaat eigenlijk over scope. Scope in CSS

Bron: You Don't Know JS


<!-- references -->
[10 Interview Questions Every JavaScript Developer Should Know in 2024]: https://medium.com/javascript-scene/10-interview-questions-every-javascript-developer-should-know-in-2024-c1044bcb0dfb


## Eigen notities

```js
<script type="module">
```
> Je kan dan scripts inladen

Als je een module maakt doet eigenlijk al hetzelfde als defer, maar dan met extra's

defer = dan hoef je niet het script onderaan de body te laden

Zijn modules scoped bij default?
Modules zijn async bij default
En die kan je awaiten, je hoeft dan geen function te schrijfen

Wordt altijd uitgevoerd in strict mode = zelf uitzoeken


Scope = function/blocks
Context = objecten (this)

Local scope = de algemene scope

window = global scope

Hoe staat de code op dat moment voor( de state van de code)

Call stack = aan de hand van een concurrency model = wat kan er tegelijkertijd van code worden afgevoerd
In javascript kan er niet tegelijkertijd code uitgevoerd worden want js is eeen single threaded

Meer te leren van de source debugger = naar 'event loop'kijken

event loop = zorgt dan de code gewoon doorgaat ook als het word onderbroken

Als je `debugger` in de code schrijft dan maak je met code handmatig een breakpoint


Je kan ook een breakpoint maken bij een DOM element dan doe je rechter mui > Break on > subtree modifications

Je kan ook een atribute modifications doen, dan moet je een attribute hebben