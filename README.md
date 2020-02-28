# JSBasics

Github repo for notes / JS basics course exercises

[Wes Bos Courses](https://courses.wesbos.com/account)

[Beginner JS Github repository](https://github.com/wesbos/beginner-javascript)

adernley@gmail.com

1. Browser shortcuts
- cmd + shift + c - inspect element
- option + cmd + j - console

2. Cmdline shortcuts
- cd - change directory
- ls -l - list all directories
- pwd - print working directory
- cd .. - go up a level in directory
- cmd + k - clears out terminal

3. Running JavaScript
- via devtools console
- via script tags in html file (before closing body tag for example, after the DOM elements have loaded)
- via script tag but from an external file (using src= in the script tag)
- via node.js in the terminal - runs via the node server ('node node-example.js' in the cmdline runs the js file in the node server)

4. [Variables](https://github.com/aaron-dernley/JSBasics/blob/master/beginner-javascript-master/playground/variables.html) in JS
- let age = 300 - this can be changed if required in a block of code
- const age = 300 - this cannot be changed in a block of code
- var age = 300 - can be used when you don't want the above restrictions
- variables don't start with a capital letter, in convention best practice
- $ and _ can be used in variables - common in loadash and jQuery library

5. 7 Types in JavaScript
- Strings - ''
- Numbers - 666
- Objects - Everything in JS is an object
- Boolean - True or false
- Null - defines 0 - has a value of nothing
- Undefined - defines 0 - something not yet defined
- Symbol - always give a unique identifier

6. Functions
- Built in - thousands of built in functions in the browser
- Custom - first a function needs defining before it can be called (write code for function, then call if afterwards) e.g.:
```
// 1. Function Definition

function calculateBill() {

// This is the function body

    console.log('running calculate bill');
    const total = 100 * 1.13; // total * tip - block scoping means this isn't available outside of this function YET
    console.log(total);
    return total // addition - this is needed for the total to be available outside of this scope

}

// 2. Function Call or *Run*

const myTotal = calculateBill(); // needed in order to use the returned total in the block above ^

console.log(`Your Total is $${myTotal}`);

```

![Function breakdown](https://github.com/aaron-dernley/JSBasics/blob/master/functionimage.png)