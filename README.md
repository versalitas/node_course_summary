# node_summary

## sprint 1:

### prototype

Every object has a built in property called prototype. 
This property is itself an object. These are the mechanisms by which Javascript objects inherit features from one another.
The property chain ends when we reach a property that has null for its own property.

Object.prototype

Date.prototype

Array.prototype

### class

Classes are a template for creating objects.

Class declaration:
```
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}
```



### callback

A function that is passed into another function (known as higher order function) as an argument.
The callback function can then be invoked inside the higher order function.
In JS all functions are objects. 
```
setTimeout(() =>  { console.log("Hello World"); }, 300); 
```
### promises

Promises are objects that can have three states: pending, resolved and rejected. 
It is used to manage asynchronous operations (non blocking).
They can be chained with .then() and error handled with .catch().

The promise constructor takes a callback function known as the executor function which in its turn takes two functions as parametres... resolve() and reject().

```
//this returns the promise

const myPromise = () => {
  return new Promise((res, rej) => {
    let yay = true;
    if(yay){
      res(Yay');
    } else {
    rej('Nay!');
  }
}

//here come the results of the successhandler and the errorhandler

myPromise
.then(resValue => console.log(resValue))
.catch(rejValue => console.log(rejValue))


```

### async/ await

An async function ALWAYS returns a promise. 
await only works inside an async function.
JavaScript waits till the promise has resolved.
If it throws an exception, the promise is rejected.
```
async function main() {
  try {
    var quote = await getQuote();
    console.log(quote);
  } catch (error) {
    console.error(error);
  }
}
```
## sprint 2

### DB SQL

- relational (relationship through keys)
- structured query language and have a predefined schema.
- vertically scalable
- table based

### DB NoSQL

- non relational (embedded data, references)
- dynamic schemas for unstructured data 
- horizontally scalable
- documents (key:value)

## sprint 3

### Creational Patterns.
Flexibility and reuse of existing code.

#### Singleton
Ensures that a class has only one instance, while providing a global access point to this instance.

### Structural patterns.
Assembles objects and classes into larger structures, 
while keeping these flexible and efficient.

#### Decorator
Attaches new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.

### Behavioral patterns
Effective communication and the assignment of responsibilities between objects.

#### Observer 
lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.

### Middleware
The middleware pattern consists of code that runs (on the server) between getting a request and sending a response. The exit point of each unit is the entry point to the next.

## sprint 4


