# React

### What is React?

A javaScript library for building user Interfaces

- Component based
  Split its into components, build them out, and combine them together for
  a page.
- Stateful
  A component can maintain internal state


### React.Component
Takes a parameter called props
Returns view with render() method

What does the render method do?
It returns a description of what you want to see on the screen
Render returns a React element

Each React component is encapsulated and can operate independently

### React Element
Each react element is a javascript object you can store in a variable or pass
around your program

### What is JSX?
You can put any javascript expression within braces inside JSX.

### SUPER
Always call super(props) when using a constructor

### setState
React will automatically update any chil components once you call setState on
a component


### Controled components
A parent component has complete control over a child compoennt, when it's
passing the child props, and and functions etc. The child is only taking in the
props, and using them, not chanigng anytihng itself

### Parent Component (BIG DADDY MAKES THE CALLS)
So big daddy owns all the state, and allows children to change it if it passses
props and the like down. BUT you do not have children passing to Big Daddy, no
sir
Big Daddy keeps the children in sync this way

### What is encapsulation and how does it work in react

### what is immutability and why is it important?
Replace the data with a new copy of that data which has the desired changes
applied to it.
- Time travel
- Detecting changes
- Pure components

The main benefit is being able to build pure components

### Key prop for React
Keys tell React about the identity of each component which allows React to
maintain state between re-renders

IF DYNAMIC ASSIGN A PROPER KEY HOMIE!

Using the array index as a key is problematic when trying to re-order a list's
items or inserting/removing list items

Keys don't need to be globally unique; they only need to be unique between
components and their siblings

### What are JSX Fragments?

### What is a class Component?


Everysingle class has props

#### What is a prop?

### What is a functional Component (Function component)?
A component that only contains a render method. 
Normally a child, that is being passed props, it's a controlled component in
most cases
Does not have its own state

<></>
Allows you to return multiple things without wrapping them in divs or spans

## Creating a React app ways

### create-react-app

What is create-react-app?

`npx create-react-app name_of_app`

## Hooks

### useState()

#### Add to an array

To set the state of an array, by adding one element to it you would use the
prevState, spread operator
`setArrayExample(prevState => [...prevState, addedElement])`
The set state is called, then the function prevState gets the previous state,
you then spread it out to add all the old state in but then add a new element
to it

#### Remove from an array using ID

To remove from an array using ID it's similar to the setting, we get the
prevState, then use .filter, to filter out the element by its id
`setArrayExample(prevState => prevState.filter(element => element.id !== id))`

### useEffect()

Side effect hook
Good to use like a lifecycle method, have it run when a component is mounted,
unmounted, rerenderd, changed, etc

You can pass it values so that it only runs when those specific values are
changed
If you pass it an empty array it'll run only the first time that component is
run

### useContent()

#Frequent NPM used

### eslint

Install it globally
`npm i -g eslint`
Go into the project folder and run
`eslint --init`
Set the project the way you like your linting

### Prettier

[[https://prettier.io/docs/en/install.html|Prettier]]
Install it
`npm install --save-dev --save-exact prettier`

`import styled from 'styled-components'`

<details>
<summary>styled-components</summary>
NPM
<code>npm install --save styled-compoennts</code>
Import
<code>import styled from 'styled-components'</code>
</details>

#### uuid

[[https://www.npmjs.com/package/uuid|uuid]]
Used to get a unique id
`npm i uuid`

#### Normalize css

`npm install --save normalize.css`

### React.Context

[[https://reactjs.org/docs/context.html|Context API]]
Good for using to change the authenticated user, theme, language, "Global"
stuff.
Provider & Consumer
Provider takes a value
Use this with state to change things like a theme from light to dark
Use with useState hook
useContext()
