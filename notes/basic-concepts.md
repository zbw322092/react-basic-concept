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



