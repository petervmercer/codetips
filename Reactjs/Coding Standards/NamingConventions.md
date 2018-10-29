### Reactjs naming conventions

## Creating a Component

File name in Pascal case in a ./components directory

```jsx harmony
import MyReactComponent from './components/MyReactComponent';
```



Use .jsx extension

Or if you are using Flow use .js



## Import Component naming

Use PascalCase for Component file names and use PascalCase if the Component is a direct reference and not an instance

Direct reference to component using its PascalCase Name
```jsx harmony
import MyReactComponent from './components/MyReactComponent';
```

For an instance use camelCase
```jsx harmony
import myReactComponentInstance from './MyReactComponent';
```

## Variables

camelCase

## Classes

PascalCase

```js
class MyClassName extends React.Component {
    
}
```

## Functions

### Event functions

### Event Handling