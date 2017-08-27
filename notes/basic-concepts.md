# react basic concept and features
## React.js Basic
### JSX
- `JSX`, it is a syntax extension to JavaScript
- `JSX` produces React "elements".
- JS _expression_. An _expression_ is any valid unit of code that resolves to a value.
- JSX is an Expression Too.
- After compilation, `JSX` expressions become **regular JavaScript objects**.
- `JSX` Represents Objects
- `Babel` compiles `JSX` down to `React.createElement()` calls.

### Rendering Elements
- `Elements` are the **smallest building blocks** of React apps.
- React elements are **immutable**.
- React Only Updates What's Necessary.

### Components and Props
- `Components` let you split the UI into independent, reusable pieces, and think about each piece in isolation.
- Conceptually, `components` are like `JavaScript functions`. They accept arbitrary inputs (called "`props`") and return `React elements` describing what should appear on the screen.
<br/>

Functional and Class Components
- The simplest way to define a component is to write a **JavaScript function**.
- You can also use an `ES6 class` to define a component.
<br/>

Rendering a Component
- When React sees an element representing a `user-defined component`, it passes `JSX attributes` to this component as a **single object**. We call this object "`props`".
<br/>

Composing Components
- Components can refer to other components in their output.
<br/>

Extracting Components
- A good rule of thumb is that if a part of your UI is used **several times** (Button, Panel, Avatar), or is **complex** enough on its own (App, FeedStory, Comment), it is a good candidate to be a reusable component.
<br/>

Props are Read-Only
- Whether you declare a component as a function or a class, it must never modify its own props. 
- React is pretty flexible but it has a single strict rule:
**All React components must act like pure functions with respect to their props.**

### State and Lifecycle
See `State` example in offical doc.
<br/>

- In applications with many components, it's very important to **free up resources** taken by the components when they are **destroyed**.
- `mounting` and `unmounting`
- Do Not Modify State Directly
- State Updates May Be Asynchronous
- State Updates are Merged
<br/>

The Data Flows Down
- A component may choose to pass its state down as **props** to its child components
- This is commonly called a **"top-down" or "unidirectional" data flow**. Any state is always owned by some specific component, and any data or UI derived from that state can only affect components "below" them in the tree.
- If you imagine a component tree as a **waterfall of props**, each component's state is like an additional water source that joins it at an arbitrary point but also **flows down**.


### Handling Events
### Conditional Rendering
### Lists and Keys
- Keys help React identify which items have changed, are added, or are removed. 
- Keys only make sense in the context of the surrounding array.
- A good rule of thumb is that elements inside the map() call need keys.
- Keys used within arrays should be unique among their siblings. However they don't need to be globally unique.

### Lifting State Up
- In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called "lifting state up". 

- There should be a single **"source of truth"** for any data that changes in a React application. Usually, the state is first added to the component that needs it for rendering. Then, if other components also need it, you can **lift it up** to their closest **common ancestor**.

### Composition vs Inheritance
