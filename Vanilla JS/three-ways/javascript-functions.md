# Classic Functions
## HOISTED, Generates a Prototype (Constructor, Arguments Objects)

```
function helloWorld(){
    console.log("Hello World")
}

helloWorld()
```

# Anonymous Function with Function Keyword
## Not Hoisted, Generates a Prototype

```
const helloWorld = function(){
    console.log("Hello World")
}

helloWorld()
```


# Arrow Functions
## Not Hoisted, No Prototype

```
const helloWorld = () => {
    console.log()
}

helloWorld()
```
