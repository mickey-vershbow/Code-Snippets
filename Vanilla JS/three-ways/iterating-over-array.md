```
const instruments = ["drums", "bass", "guitar"]
```

### Method #1
```
for (instrument of instruments) {
  console.log("I play the " + instrument)
}
```


### Method #2
```
for (let i = 0; i < 3; i++) {
  console.log("I play the " + instrument.i)
}
```


### Method #3
```
instruments.forEach((instrument) => {
  console.log("I play the " + instrument)
})
```
