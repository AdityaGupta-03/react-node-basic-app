## What is React.JS ?

Open source Javascript library for building user interfaces

## Why to learn React ?

Creates and maintained by Facebook
Huge Community

## Component Based Development

Component based development means designing our software applications by
building loosely-coupled independent components

## What is Component ?

A component is a well-defined and independent piece of our app's user interface

A Compoennt could include, but not limited to

-   Button
-   Header
-   Footer
-   Navigation
-   Table
-   Pagination

## Why Do we need Components ?

Compoenents build off of the concept of Ajax Requests,
in which calls to the server made directly from client-side,
allowing for the DOM to be dynamically updated without the
need of `page refresh`

Because componets are independent, one component can refresh without
affecting other compoenents or the UI as a whole

## Types components

1. Function Components
2. Class Components

## React JS Basics

props - Shortcut for properties

props - We can use props to allow compoenenst to talk to each other

-> Get passed co component function parameters
-> props are immutable
-> props - function component
-> this.props - class component

state - React updates UI based on the application state. - This is actuallys stored as a property of react Class Compoement

-> State is managed with in the component
-> state can be changed
-> useSate() - Function Component
-> this.state - Class Component

## JSX - Javscript XML

Extension for javascript Language Syntax

XML-Like code for elements and components

JSX is not manadtory to write react compoenents

JSX makes our code simplified and elegant

JSX ultimately transpiles to pure javascript which is understood by the browsers

## Conditional Rendering

1. if/else
2. Element variables
3. Ternary Operator
4. Short Circuit Operator

## Basics of Styling in React Components

1. CSS StyleSheet
2. Inline Styling
3. CSS Modules
4. CSS in JSLibraries ( Using Boorstrap Already)

## Life Cycle Methods

When we create a React Component it goes through several stages
in its life Cycle

Note: Life Cycle Methods do not exist on function components
Only available on class components

## 4 Phases of lifecycle Methods

1. Mounting
2. Updating
3. Unmounting
4. Error Handling

## Mounting

When an instance of component is being created and inserted into the DOM

## LifeCycle Methods

-> constructor
-> static getDerivedStateFromProps
-> render
-> componentDidMount

constructor - A special function that will get called whenever
a new component is created

      When to use ?
      -------------
      1. Initialize the state
      2. Binding the event handler

      When not use ?
      ---------------
      When Making HTTP requests

      Two Imporant things
      --------------------
      1. We have to call special function 'super' , this will call the
         base class constructor
         In our component we have access to this.props only after
         we initially called super passing the props
      2. This is the only place where we change or set the state directly
         overwriting this.state fields

## static getDerivedStateFromProps

Method is called every time a component is re-rendered

-> we can set the state
-> Never use this method for Ajax / HTTP Calls

## render()

-> Only Required method in our Components (Class)

-   > We simply read props, state and return JSX
    > -> Do not make HTTP calls
    > -> Right after the parent render method child
    > component life Cycle methods are executed

## componentDidMount

-> Invoked immediately after a component and all its
child compoenents have been rendered to the DOM

-   > Place to make the Ajax Calls and load the data

## Updating

When a component is being re-rendered as a result of changes to either its
props or state

## LifeCycle Methods

-> static getDerivedStrateFromProps,
-> shouldComponentUpdate
-> render,
-> getSnapShotBeforeUpdate
-> componetDidUpdate

## Unmounting

When a compoenent is being removed from the DOM

## LifeCycle Method

-> componentWillUnMount

## Error Handling

When there is an error during the rendering in a life cycle method
or in the constructor of any child component

## LifeCycle Methods

-> static getDerivedFromError
-> componentDidCatch

## React Routing

navigating to other pages

we use react-router-dom

BrowserRouter - Used for doing client-side Routing with URL Segments

Routes - Returns only the first Matching Route rather than all matching routes

Route - "Conditionally Shown Component" based on matching a path to a URL

Link - Replacement for anchor tags

## React Hooks

Hooks are new feature addition in react version 16.8
Which allows us to use react features without having to write a class

e.g state of component

-> completely Optional
-> Hooks doesn't contain any breaking changes and backword compatiable
-> Classes won't be removed from React
-> Can't use hooks inside a class component

## Rules of the Hooks

-> Only call hooks at the top level

Means, Don't call hooks inside the loops, conditions or nested functions

-> Only Call hooks from React functions

## Redux

Redux will need three things

Actions - Descibes type of action
Reducers - implenets behaviour of the action - take the current state and action and return new state - never return undefined from reducers - We always want our state to be defined
Store - brings actions and reducers together and changes the state of app

---

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

https://github.com/dsznajder/vscode-react-javascript-snippets/blob/HEAD/docs/Snippets.md - react Snippets

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.
