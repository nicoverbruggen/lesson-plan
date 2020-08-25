# Part 6: JavaScript

## Terminology
- JavaScript
- ECMAscript
- Console
- Stack
- Primitives: booleans, strings, numbers
- Variables
- Functions / methods
- Parameters
- Returning
- Arrays
- Objects
- Closures
- Loops
- If-statements

## Preparation
* Do we have a browser installed?
* Is the browser up-to-date?
* Do we have `nodejs` and `npm` installed? 
* Do we have `browser-sync` globally installed?
* Have we started the watcher process?
    * `browser-sync start --server --files "src/*/*.css" "src/*/*.js" "index.html"`
* Alternatively: is Live Server VSCode plugin installed?

## Understanding JS
* What _is_ JavaScript? 
    - It is a scripting language we can use to add interactivity to web pages.

## Understanding npm / nodejs
* Why do we need npm and nodejs?
    - We need it to download an run packages made by other developers.
    - That way, we don't need to write tons of code ourselves, and can reuse previously built functionality.

## Programming basics

## Statements
* Each line of code is a statement (usually)
* We terminate statements with a semicolon (;)

## Data types
* What are the available primitive types in JS?
    - https://developer.mozilla.org/en-US/docs/Glossary/Primitive 
    - string -> 'hello world' / "hello world"
    - number -> 5.5
    - bigint -> 5
    - boolean -> true
    - undefined
    - Symbol
    - null is a special case, see MDN
* Are primitives mutable?
    - No. All primitives are immutable.
* What are the available reference types in JS?
    - array []
    - object literal {}
    - Date
* Are e.g. arrays mutable?
    - Yes.
* How do I check if an element is of a specific type?
    - Use the `typeof` reserved keyword: `typeof myVar === "number"` 
* What is the difference between `=`, `==`  and `===`?
    - Single = is for assignment
    - Double = is for comparison (loose)
    - Triple = is for comparison (strict)

## Functions & Methods
* What is a function?
    - A function is a set of statements grouped together,
     with possible arguments that are sent to the function to alter the behaviour.
* What is the difference between a function and a method?
    - A method is executed on an object.
    - A function is more generic. Each method is a function, but not every function is a method.
* What is a parameter?
    - It is like a variable that you pass along with the function.
* What does it mean to return?
    - It means the function ends, and the returned variable is given back to the original caller.
* Can I choose not to return anything?
    - Yes, this means the return type is `void` (the default).
* Can you create a function with two parameters?
    - `function myFunction(param1, param2) {}` 

## Constants and variables
* What does it mean to assign a variable?
    - It's like putting a sign to point at a box that contains something.
* What keyword do we use to assign a variable?
    - `let` (in case we need to be able to reassign it)
    - `const` (in case we don't need to reassign it) 
* What's the difference between reassigning a variable and a property?
* Can you reassign a constant?
    - No. The point is that you cannot.
* Can you reassign a property of a constant object?
    - Yes. The actual pointer to the object does not change.

## Selecting elements on a page
* How do I select an element with a specific class on our page?
    - `document.querySelector(".class")` 
* How do I select ALL elements with a specific class on our page?
    - `document.querySelectorAll(".class")`  
* How do I select an element with an ID of "name"?
    -  `document.getElementById('name')` 

## Adding new elements
* How do I create a new paragraph and store it in a variable called `paragraphElement`?
    -  `let paragraphElement = document.addElement("p")`
* How do I set the text of said element to "hello"?
    - `element.innerHTML = 'hello'`
* How do I adjust styling of said element?
    - `element.style` can be used for this 