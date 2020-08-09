# React

### What is React?

A javaScript library for building user Interfaces

- Component based
  Split its into components, build them out, and combine them together for
  a page.
- Stateful
  A component can maintain internal state

### What is JSX?

### What are JSX Fragments?

### What is a class Component?

:
Everysingle class has props

#### What is a prop?

### What is a functional Component?

<></>
Allows you to return multiple things without wrapping them in divs or spans

## Creating a React app ways

### create-react-app

What is create-react-app?

`npx create-react-app name_of_app`

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

## Hooks

- useState()
- useContent()
