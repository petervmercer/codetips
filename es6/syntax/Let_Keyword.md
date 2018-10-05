### ES6 Code Tips

## let Keyword

# When to use it?

Used to prevent scope errors. For example

```ecmascript 6
var x = 'global';

if(x === 'global') {
    let x = 'local';
}

console.log(x); // Result should = 'global'
```

Very useful in for loops to have local scope