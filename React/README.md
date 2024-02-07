# React roadmap

## CLI Tools:

### Vite
Vite is a build tool that aims to provide a faster and leaner development experience for modern web projects.
- [Vite](https://vitejs.dev)
- [Documentation](https://vitejs.dev/guide/)
- [Course](https://www.youtube.com/watch?v=LQQ3CR2JTX8)
- [Course](https://www.youtube.com/watch?v=89NJdbYTgJ8)
### Create React App

## Components:

### Functional Components
Functional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function. These functions may or may not receive data as parameters. In the functional Components, the return value is the JSX code to render to the DOM tree. Functional components can also have state which is managed using React hooks.
- [Functional Components and Props](https://react.dev/reference/react/Component)
- [Your first component](https://react.dev/learn/your-first-component)
- [Passing props to a component](https://react.dev/learn/passing-props-to-a-component)
- [Functional Components in React](https://www.robinwieruch.de/react-function-component/)
### JSX
JSX stands for JavaScript XML. It allows writing HTML in JavaScript and converts the HTML tags into React elements.
- [Writing markup with JSX](https://react.dev/learn/writing-markup-with-jsx)
- [JavaScript in JSX with Curly Braces](https://react.dev/learn/javascript-in-jsx-with-curly-braces)
- [JSX in React – Explained with Examples](https://www.freecodecamp.org/news/jsx-in-react-introduction/)
- [JSX in React on w3school](https://www.w3schools.com/react/react_jsx.asp)
### Props vs State
Props (short for “properties”) and state are both plain JavaScript objects. While both hold information that influences the output of component render, they are different in one important way: props get passed to the component (similar to function parameters) whereas state is managed within the component (similar to variables declared within a function).
- [State: A Component’s Memory](https://react.dev/learn/state-a-components-memory)
- [How to use Props in React](https://www.robinwieruch.de/react-pass-props-to-component/)
- [What is the difference between state and props in React?](https://stackoverflow.com/questions/27991366/what-is-the-difference-between-state-and-props-in-react)
- [How to update state from props in React](https://www.robinwieruch.de/react-derive-state-props/)
### Conditional Rendering 
In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application. < /br>

Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like [if](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else) or the [conditional operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator) to create elements representing the current state, and let React update the UI to match them.
- [Conditional Rendering](https://react.dev/learn/conditional-rendering)
- [Different techniques for conditional rendering in React](https://www.robinwieruch.de/conditional-rendering-react/)
### Composition
React has a powerful composition model, and it is recommended to use composition instead of inheritance to reuse code between components.

- [Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
- [How to perform component composition in React](https://www.robinwieruch.de/react-component-composition/)
- [Achieving Reusability With React Composition](https://formidable.com/blog/2021/react-composition/)
- [Passing JSX as children](https://react.dev/learn/passing-props-to-a-component#passing-jsx-as-children)