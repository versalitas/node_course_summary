# node_summary

##sprint 1:

### prototype

Protypes are the mechanisms by which Javascript objects inherit features from one another.
Every object has a built in property called prototype. 
The property is itself an object. 
The property chain ends when we reach a property that has null for its own property.

Object.prototype

Date.prototype

Array.prototype

###  callback
A function that is passed into another function (known as higher function) as an argument.
The callback function can then be invoked inside the higher order function.
In JS all functions are objects. 

setTimeout(() =>  { console.log("Hello World"); }, 300); 

###  promises

Promises are objects that can have three states: pending, resolved and rejected. 
It is used to manage asynchronous operations (non blocking).
They can be chained with .then() and error handled with .catch


###   async/ await

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


