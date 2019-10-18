TOPIC: Loop
AUTHORS: Federico Culloca; federicoculloca@github.com; github:federicoculloca
         Heather; hbloomer@mozilla.net; mdn:hbloomer
         Maria Rubina; maria-rubina@mozilla.net; mdn:maria-rubina
         Kobe Davis; Llamaless@mozilla.net; mdn:Llamaless
         Diana Varnes; ezrinjaz@github.com; github:ezrinjaz

# Loop

A loop is a sequence of instructions that is continually repeated until a certain condition is met
in computer programming. An example would be the process of getting an item of data and changing it,
and then making sure some condition is checked such as, if a counter has reached a prescribed number.

## Examples

### For loop

**Syntax**:

```javascript
for (statement 1; statement 2; statement 3){
  execute code block
}
```

- Statement 1 is executed once before the code block is run.

- Statement 2 defines the condition needed to execute the code block.

- Statement 3 is executed every time the code block is run.

**Example**:

```javascript
for(var i = 0; i < 10; i++){
  console.log(i)
}
//This loop will print numbers 0-9, will stop when condition is met (i = 10)
```

For the above example, the syntax is as follows:

- Statement 1 sets the variable for the loop (var i = 0).

- Statement 2 sets the loop condition (i < 10).

- Statement 3 increases the value of i (i++) each time the code block is run.

### While loop

**Syntax**:

```javascript
while (condition){
  execute code block
}
```

- The code block will continue to loop as long as the condition is true.

**Example**:

```javascript
var i = 0;
while(i < 5){
  console.log(i)
  i++
}
//This loop  will print number 0-4, will stop when condition becomes false (i >=5)
```

For the above example, the syntax is as follows:

- The code block will continue to run as long as the variable (i) is less than 5.

## Learn More

### General Knowledge

- [Control flow](https://en.wikipedia.org/wiki/Control_flow#Loops) on Wikipedia