# ca-js-methods and objects

### Methods
When the data stored on an object is a function we call that a method. A property is what an object has, while a method is what an object does.

Do object methods seem familiar? That’s because you’ve been using them all along! For example console is a global javascript object and .log() is a method on that object. Math is also a global javascript object and .floor() is a method on it.

We can include methods in our object literals by creating ordinary, comma-separated key-value pairs. The key serves as our method’s name, while the value is an anonymous function expression.


### OBJECTS
#### Pass By Reference
Objects are passed by reference. This means when we pass a variable assigned to an object into a function as an argument, the computer interprets the parameter name as pointing to the space in memory holding that object. As a result, functions which change object properties actually mutate the object permanently (even when the object is assigned to a const variable).

>const spaceship = {
>  homePlanet : 'Earth',
>  color : 'silver'
>};
 
>let paintIt = obj => {
>  obj.color = 'glorious gold'
>};
 
>paintIt(spaceship);
 
>spaceship.color // Returns 'glorious gold'
 
Our function paintIt() permanently changed the color of our spaceship object. However, reassignment of the spaceship variable wouldn’t work in the same way:

### View code here:
https://gist.github.com/040f0650966c9f349ee673cd8bf5c613


### OBJECTS
#### Looping Through Objects
Loops are programming tools that repeat a block of code until a condition is met. We learned how to iterate through arrays using their numerical indexing, but the key-value pairs in objects aren’t ordered! JavaScript has given us alternative solution for iterating through objects with the for...in syntax .

for...in will execute a given block of code for each property in an object.

### View code here:
https://gist.github.com/be034b3a8697d5c56c3ab3f864ad98a4

### review

#### Objects store collections of key-value pairs.
Each key-value pair is a property—when a property is a function it is known as a method.
An object literal is composed of comma-separated key-value pairs surrounded by curly braces.
You can access, add or edit a property within an object by using dot notation or bracket notation.
We can add methods to our object literals using key-value syntax with anonymous function expressions as values or by using the new ES6 method syntax.
We can navigate complex, nested objects by chaining operators.
Objects are mutable—we can change their properties even when they’re declared with const.
Objects are passed by reference— when we make changes to an object passed into a function, those changes are permanent.
We can iterate through objects using the For...in syntax.

## objects in JavaScript are containers that store data and functionality. In this lesson, we will build upon the fundamentals of creating objects and explore some advanced concepts.


