# `JavaScript Lecture 2`
![](/img/logo.jpg)

 # **Table of Contents**

 <br>

-  [ **Scope**](#scope)
-  [ **Hoisting**](#hoisting)
-  [**Recursion**](#recursion)
-  [**Closure**](#closure)

<br>

# **Scope**

![](/img/javascript-scope-cover-2.png)

<br>
<br>

- ## **What is `Scope` in JavaScript**
`In JavaScript, scope refers to the accessibility of variables and functions in a particular part of your code during runtime. It determines which parts of the code can access a particular variable or function.`

<br>

## **JavaScript has the following kinds of scopes:**
***
<br>

- [ **Global Scope**](#global-scope)
- [ **Function Scope**](#function-scope)
- [ **Block Scope**](#block-scope)
- [ **Module Scope**](#module-scope)

<br>

- ## **Global Scope**
***
`Global scope in JavaScript refers to the outermost scope of a program, where variables and functions are declared without being enclosed in another function or block. In web browsers, the global scope is associated with the window object, which serves as the top-level object in the browser's JavaScript environment.`

`Variables and functions declared in the global scope are accessible from anywhere within the program, including within functions or blocks that are nested within other functions or blocks. However, care should be taken when using global variables, as they can be modified by any part of the program and can lead to naming conflicts or unintended changes.`

<br>

- ## **Function Scope**
***
`Function scope in JavaScript refers to variables that are only accessible within the function in which they are declared. In other words, variables declared inside a function have local scope and are not visible outside of the function.`

<br>

- ## **Block Scope**
***
`Block scope in JavaScript refers to the idea that variables declared with `let`  and  `const`  are only accessible within the block of code where they are defined, as well as any nested blocks. A block of code is typically defined by a pair of curly braces  `{ }`, such as an  `if`  statement, a  `for` loop, or a function.`

<br>

- ## **Module Scope**
***
`Module scope in JavaScript refers to the idea that variables declared within a module are only accessible within that module.`

`A module is typically defined using the `export` keyword to declare which variables and functions will be accessible outside of the module. Variables and functions that are not explicitly exported are considered to be private to the module and are not accessible from outside the module.`

<br>
<br>
<br>


# **Hoisting**
![](/img/hosting.png)
<br>
<br>

- ## **What is `Hoisting` in JavaScript**
***
`Hoisting is a JavaScript mechanism where variable declarations and function declarations are moved to the top of their respective scopes before code execution. This means that even if a variable or function is declared after it has been used, the interpreter will move it to the top of the scope, allowing the code to execute without any errors. However, only the declaration is hoisted, not the initialization or assignment of the variable. It's important to note that hoisting only occurs within a single scope, and does not work across multiple nested scopes.`
 
<br>

## **In JavaScript, there are two types of hoisting:**
***
<br>

- [ **Hoisting - Function Declaration**](#hoisting-function-declaration)
- [ **Hoisting - Variable**](#hoisting-variable)
- [ **Temporal dead zone, let and const**](#temporal-dead-zone-let-and-const)

<br>

- ## **Hoisting - Function Declaration**
***
`Function Hoisting is a behavior in JavaScript where function declarations are moved to the top of their respective scopes during code execution, regardless of where the actual declaration appears in the code. This means that you can call a function before it has been declared, and the JavaScript engine will still be able to execute it without throwing an error.`

`Note that function expressions (functions assigned to variables) are not hoisted in the same way as function declarations.`

<br>

- ## **Hoisting - Variable**
***
`Variable hoisting is a behavior in JavaScript where variable declarations are moved to the top of their respective scopes during code execution. This means that you can use a variable before it has been declared, and the JavaScript engine will still be able to execute it without throwing an error.`

`However, it's important to note that only the declaration (the var keyword) is hoisted, not the initialization. So even though you can use a variable before it is declared, if you try to use it before it is assigned a value, you will get undefined:`

<br>

- ## **Temporal dead zone, let and const**
***
`The temporal dead zone is a behavior in JavaScript that affects the let and const keywords. When using these keywords to declare variables, the variables are not hoisted like they would be with the var keyword. Instead, there is a "temporal dead zone" (TDZ) between the start of the block scope and the point where the variable is declared.`

`During the TDZ, if you try to access the variable before it has been declared, you will get a ReferenceError.`

`This behavior is different from what happens with the var keyword, where uninitialized variables have the value undefined during the entire scope. With let and const, the variable does not exist until it is declared, and trying to access it before that point results in a ReferenceError.`

`It's worth noting that the temporal dead zone only affects let and const declarations, not var or function declarations.`



## **Recursion**
***
## **Closure**
***
