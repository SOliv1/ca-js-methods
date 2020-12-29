# ca-js-methods

### Methods
When the data stored on an object is a function we call that a method. A property is what an object has, while a method is what an object does.

Do object methods seem familiar? That’s because you’ve been using them all along! For example console is a global javascript object and .log() is a method on that object. Math is also a global javascript object and .floor() is a method on it.

We can include methods in our object literals by creating ordinary, comma-separated key-value pairs. The key serves as our method’s name, while the value is an anonymous function expression.


### OBJECTS
Pass By Reference
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

### View code here
https://gist.github.com/040f0650966c9f349ee673cd8bf5c613
