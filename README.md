# node_summary

## sprint 1:

### prototype

Protypes are the mechanisms by which Javascript objects inherit features from one another.
Every object has a built in property called prototype. 
The property is itself an object. 
The property chain ends when we reach a property that has null for its own property.

Object.prototype

Date.prototype

Array.prototype

### callback
A function that is passed into another function (known as higher function) as an argument.
The callback function can then be invoked inside the higher order function.
In JS all functions are objects. 

setTimeout(() =>  { console.log("Hello World"); }, 300); 

### promises

Promises are objects that can have three states: pending, resolved and rejected. 
It is used to manage asynchronous operations (non blocking).
They can be chained with .then() and error handled with .catch


### async/ await

An async function ALWAYS returns a promise. 
await only works inside an async function.
JavaScript waits till the promise has resolved.
If it throws an exception, the promise is rejected.

async function main() {
  try {
    var quote = await getQuote();
    console.log(quote);
  } catch (error) {
    console.error(error);
  }
}

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
increase flexibility and reuse of existing code

#### Singleton
ensure that a class has only one instance, while providing a global access point to this instance.

### Structural patterns.
assembles objects and classes into larger structures, while keeping these flexible and efficient.

#### Decorator
lets you attach new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.

### Behavioral patterns
effective communication and the assignment of responsibilities between objects.

#### Observer 
lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.

## Middleware
provides a method of communication and data management between applications that would otherwise not have any way to exchange data -- such as with software tools and databases.

