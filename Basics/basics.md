# Variables
* Variable is used to store data temporarily in computer's memory. So we store data somewhere and give that memory location a name and with this name we can read the given location in the future.
* Declaring a variable using var keyword before ES6.
* Now will declare a variable using let keyword.
## Rules for naming Variables
1. It cannot be reserved keyword
2. Should be meaningful or descriptive name
3. Cannot start with number
4. Cannot contain space or hypen(-)
5. Use camel notation
6. Are Case sensitive  
Eg: 1. let firstName; // undefined  
    2. let firstName = "abc";

# Constants
1. If we use const keyword while initializing variable, value of the variable will not change through out the program.
Eg: ```
const PI = 3.14;
PI = 1.41;
console.log(PI);
//output: uncaught TypeError: Assignment to constant variable at line 3  
```
2. use let keyword if we want to change the value of the variable.

# Primitive Types
There are two types 
1. Primitive types are also called value types
2. Reference types
 ## Primitive types
1. String
2. Number
3. Boolean
4. Undefined
5. Null  
Eg:```
let name="abc"; //String literal
     let age = 30; // Number literal
     let isApproved = true; //Boolean literal
     let firstName = undefined; // variable not initialized
     let lastName = null // explicitly to clear the values of variables so we assing to null
```
### Dynamic Typing
* Javascript is a dynamic language
* There are two types of languages
1. Static Languages
2. Dynamic Languages
* Static languages whenever a value of variable declared it cannot be changed.
* In Dynamic, value can be change at runtime.
* typeof operator is used to check the type of a variable eg: typeof name //output: string
* In JS, floating point and integers are numbers(typeof)
* undefined is a type and also a value.  
eg: typeof lastName //output : object

## Reference Types
1. object
2. Array
3. Function
### 1. Object:
eg: ```
let person = { // object literal
 name : "abc",
age: 30
}
person.name = 'xyz'; // Dot notation
person['name'] = 'abcd'; // bracket notation
console.log(person.age);
```
### 2. Arrays
* Arrays is an object, it contains properties or bunch of key-value pairs that can access using the dot(.) notation
* typeof person //output: object, typeof array is an object.
* console.log(person.length); //returns number of items or elements in an array.
### 3. Functions
* Functions are one of the building blocks in JS, it is basically a set of statements that performs a task or calculates and returns a value.
eg 1: ```
function greet(name){
    console.log("hello world " + name);
}
greet('john');
2. 
function square(number){
    return number*number;
}
console.log(square(2));`
```
# Control Flow
### Loops:
1. For
2. while
3. Do while
4. For in
5. For of
* For, while and Do-while loops , with all these will repeat an action number of times.
* But, for-in and for-of loops, to iterate over properties of an object or elements in an array
### For-in loop
eg:1.  `const person1 = {
    name : 'john',
    age : 20
}
for(let key in person1){
    console.log(key, person1[key]);
}`

2. `const color = ['red','blue','black'];
for(let index in color){
    console.log(index,color[index]);
}`

### For-of loop
* iterate over the elements or items in an array
eg:`const color = ['red','blue','black'];
for(let colors of color){
    console.log(colors);
}`
* Break keyword, jump out of a loop
* Continue keyword, jump to the next iteration

# Objects
* Purpose of object is to group related variables and also function that should operate on these variables.
eg: ```
const circle = {
     radius : 1,
     location:{
        x:1,
        y:1
     },
     isVisible : true,
     draw: function(){
         console.log("dot notation");
     }

};

circle.draw();
// function draw();
```






