---
title: React Tutorial
date: 2024-09-10 23:23 +0200
categories: [Blogging, React Tutorial , Java Programming]
tags: [react, blog, programming, interview,technical,frontend]
---

# What is react?
React is a popular **JavaScript** library to create **User Interface (UI/Frontend)** of
Web Applications. React allows developers to create **manageable and reusable components**
that can handle their own **state** that makes the development efficient and scalable.

* Javascript library to build dynamic and interactive user interface.
* Developed at facebook.com in 2011.
* currently most widely used js library for frontend development.
* used to create single page application.
* React is a js framework (NodeJS).
* A react application run on the web server.
* React is used to create UI(Frontend).
* Its based on a component architecture.

## Component-Based Architecture
React allows web applications to be built using **small, reusable** components. These components
can manage their own state and lifecycle; this makes the code **modular and maintainable**. There
are two types of component structures: **Functional and Class components**.

## JSX (JavaScript XML)
An extension syntax in react allows you to write **HTML-like** code within JavaScript. This allows
developers to write HTML elements directly within JavaScript.

## Creating a React App
Use **Create React App** to easily start new React projects. It handles setup and provides a
smooth development experience.
    1. **Install Node.js**: Ensure you have Node.js installed on your system.
    2. **Create a New React App**: Run the following command in your terminal:
    3. Go to specific project location , where you want to create and open terminal and hit **npx create-react-app my-app**.
    4. got to **cd my-app**
    5. Hit **npm start** and its will open browser with basic react welcome page.

This is how your project folder look.
![React](/assets/img/posts/react1.png)__React project folder structure__

# Everything as a Component in ReactJS.
A component in React is like a building block you use to build your User
Interface. An independent, reusable pieces of UI. It can be **functional or class-based.**
They represent different parts of a web page and contain both structure and behavior.

## Component Structures
### Functional Components – 
Initially used for stateless components, these are simpler components defined in JavaScript functions that takes props and returns **JSX (JavaScript XML)**.

```jsx
import React from "react";

export default function MyComponent(){
    return (
        <div>
            <h1>Hello, World!</h1>
            <p>This is a simple React component.</p>
        </div>
    );
}
```
### Class Components-
Provide all React features via an object-oriented approach, they have additional features like state and lifecycle

```jsx
import React from "react";

class Mycomponent extends React.Component {
    render() {
        return (
            <div>
                <h1>Hello, React!</h1>
                <p>This is a simple React component.</p>
            </div>
        );
    }
}

```
React favors functional components because they're easier to understand and manage. These
functions can handle data changes (state) and external interactions (side effects) using **Hooks**
like **useState and useEffect**. This approach not only improves code readability and
maintainability but also allows for better performance optimization.

### JSX (JavaScript XML)
An extension syntax in react allows you to write HTML-like code within JavaScript.

### 2.Props
Are used to pass data from **parent component** to **child components**

```jsx
import React from "react";

export default function MyComponent(props) {
    return (
    <h1>Hello {props.name}!</h1>
    );
}

<MyComponent name="Bob" />
```

### Fragment
Allows functional components to return multiple elements without a div.

```jsx
import React from "react";

export default function MyComponent(){
    return (
        <>
        <h1>Hello World!</h1>
        <h2>Hello Universe!</h2>
        </>
    )
}
```
### Conditional Rendering
Allows components to render different content based on certain conditions.

```jsx
import React from "react";

export default function MyComponent(props) {
  return (
    <div>{props.isLoggedIn ? <p>Welcome, user!</p> : <p>Please log in</p>}</div>
  );
}
```

### 3.Event Handling
Events like **‘onclick’ or ‘onChange’** can be handled by components that are called **event handlers.**

```jsx
import React from "react";

export default function MyComponent() {
  const handleClick = () => {
    console.log("Button clicked");
  };
  return <button onClick={handleClick}>Click me</button>;
}
```

will continue...



