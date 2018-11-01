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

Public
```ecmascript 6
let defaultColor = '#FFF';
```
Private
```ecmascript 6
 _numberOfColors = 5;
```


## Classes

PascalCase

```js
class MyClassName extends React.Component {
    
}
```

Instance of a class

```ecmascript 6
myInstanceClassName = new MyClassName();
```

## Functions/Methods

camelCase

private methods in a class should proceed with an underscore _

```ecmascript 6
class MyClassName extends React.Component {
    
    _myPrivateFunction() {
        
    }
    
    myPublicFunction() {
        
    }
}
```

### Event functions

### Event Handling