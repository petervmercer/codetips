# Nodejs naming conventions

## Use strict

```javascript
'use strict';
```

## Variables

camelCase

Public
```ecmascript 6
var defaultColor = '#FFF';
let defaultColor = '#FFF';
const defaultColor = '#FFF';
```

Private
```ecmascript 6
 _numberOfColors = 5;
```

###Difference between var, let and const

**Scope of var**

Scope essentially means where these variables are available for use. var declarations are globally scoped or function/locally scoped. It is globally scoped when a var variable is declared outside a function. This means that any variable that is declared with var outside a function block is available for use in the whole window. var is function scoped when it is declared within a function. This means that it is available and can be accessed only within that function.

**let** 

let is preferred for variable declaration now. It's no surprise as it comes as an improvement to the var declarations. It also solves this problem that was raised in the last subheading. Let's consider why this is so.

let is block scoped 

**const**

Variables declared with the const maintain constant values. const declarations share some similarities with let declarations.

const declarations are block scoped

Like let declarations, const declarations can only be accessed within the block it was declared.

const cannot be updated or re-declared 

## Classes

PascalCase

Node uses Ecma-262. Javascript uses prototype objects so it may wise to use prototype.
```js
function MyClassName(id) {
    this.id = id;    
}

MyClassName.prototype.isMethodName = {};

/* Another approach */

var MyClassName = /** @class */ (function() {
    function MyClassName(param1) {
        this.param1 = param1
    }
    
    MyClassName.prototype.isMethodName = {};
    return MyClassName;
    
});

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

onEventName

### Event Handling

onHandleEvent
