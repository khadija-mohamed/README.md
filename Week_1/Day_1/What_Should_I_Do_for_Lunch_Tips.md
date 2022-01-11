### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

``` javascript 

function whatToDoForLunch(hungry, availableTime) {
  if (hungry) { 
  if (availableTime <= 20){
    console.log("Pick something up and eat back in the lab/kitchen.")
  }
  if (availableTime > 20 && availableTime <= 30) {
    console.log("Take a break and try a place in Gastown!")
  }
  if (availableTime > 30 ){
    console.log("Go eat since you are hungry, but be efficient with your time!")
    }
 } else {
   console.log("Bootcamp is intensive and you aren't hungry right now, maybe you should eat in a bit when you are.")
 }
}

console.log("I'm hungry and I have 20 minutes for lunch.");
whatToDoForLunch(true, 20);
console.log("---");

console.log("I'm hungry and I have 50 minutes for lunch.");
whatToDoForLunch(true, 50);
console.log("---");

console.log("I'm not hungry and I have 30 minutes for lunch.");
whatToDoForLunch(false, 30);
console.log("---");

console.log("I'm hungry and I have 15 minutes for lunch.");
whatToDoForLunch(true, 15);

```