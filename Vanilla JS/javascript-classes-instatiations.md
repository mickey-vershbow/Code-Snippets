## Define a new class

```
class Animal {
    //define the constructor function to define object properties
    constructor(sound, ears, legs){
        //assign the values passed to the constructor to the new object
        this.sound = sound
        this.ears = ears
        this.legs = legs
    }

    makeSound(){
        console.log(this.sound)
    }
}
```

## New Pig Class that inherits from Animal

```
class Pig extends Animal {
    constructor(name){
        //invoking the parent constructor with set values
        super("oink", 2, 4)
        this.name = name
    }
```

## New Method

```
    rollInMud(){
        console.log(`${this.name} rolls in mud and says ${this.sound}`)
    }
```
    makeSound(){
        console.log(`${this.name} says ${this.sound}`)
    }
}


## Instantiate Instance of our new Pig Class
```
const wilbur = new Pig("Wilbur")

console.log(wilbur)
wilbur.rollInMud()
wilbur.makeSound()

```
