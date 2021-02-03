# Custom Functions 

Welcome to the eighth lesson! In this lesson, you learn how to write your own functions. Functions are blocks of code that perform one or more tasks. They're critical for adding functionality to your webpages. You will study the syntax of how to write a function and learn how functions work. Then, you will see several examples of how you can use functions to enhance your projects.

The purpose of showing you examples of how you can use functions is because many different types of situations require you to use a function, and not in all situations are you going to use functions in the same way. For instance, you can use functions for its return a value or instead to simply perform certain tasks. Plus, while practicing writing functions, you can weave together what you learned in previous chapters. For instance, you can write functions containing conditional statements, operators, and expressions. In addition, in your functions, you can get elements by the `id`, tag type, and `class` and do other DOM manipulations. 

At the end of this lesson, you see a live coding example. The live coding session reinforces what you learn in the lesson. This lesson also helps prepare you for making your personal portfolio site. The code from this session is included in this repository. You can use it however you like, but as with any code you get from someone else, make sure you understand it well enough to explain it to someone before putting it in your own projects.  

In this lesson, you learn:  

- Hour 1: [How to Write a Function](#how-to-write-a-function)     
- Hour 2: [Examples of Functions](#examples-of-functions)   
- Hour 3: [Live Coding](#live-coding)   

The topics below outline what you learn in the live session. After the live session, you can use this material as a resource for guided self-learning. This document will serve you as a roadmap for gaining repetition with the material that you learned during the live session.   

## [How to Write a Function](#how-to-write-a-function)       

- Two keys concepts for understanding functions:
  -- You have to define your function  
  -- Once defined, to use your function, you have to invoke it  
  
### Function Definitions  

- Function definitions are blocks of code that contain instructions for what the function does when you invoke it; note that the function definition code isn't run unless and until you invoke it    
-- Once you define a function, you can reuse it  
- You can define functions in the global scope, inside other functional blocks of code, and inside objects; where you define your function impacts which other blocks of code in which you can invoke that function   
- The modern syntax for writing functions is the [arrow syntax](https://www.w3schools.com/js/js_arrow_function.asp)  
- You should know about the [older syntax](https://www.w3schools.com/js/js_function_definition.asp) too becuase you will see it online; although you will see it online, practice using the arrow syntax in your code, as its the more modern approach; this [StackOverflow post has some tips](https://stackoverflow.com/a/23045200) on when to use which type of syntax and why   
- Regardless of which syntax you use, functions can be saved as a named variable, define parameters required by the function, and/or have an explicit `return` statement; each of these are optional and can be used alone or in combination with one another    
  -- Function definitions that are not saved as a named variable are known as anonymous functions    
  -- You should get in the habit of saving your function definitions as named variables because this makes your functions re-usable throughout your code  
  -- Here is an example of an arrow function named `greetUser` saved to variable that console logs a welcome message with the `username`:  
  ```javascript
  const greetUser = (username) => {
    console.log("Welcome to ITC, " + username);
    }
  ```
  -- In the example, the `username` is a parameter  
  -- Your function definitions are not required to include parameters  
  -- By including parameters in your function definition, that means you need to give those parameters values when you invoke the function  
  -- You can give them default values in your function definition or you can pass arguments into the function when you invoke it  
  -- Here is an example definition with a default value for the `username` parameter:  
  ```javascript
  const greetUser = (username="Jack") => {
    console.log("Welcome to ITC, " + username);
    }
   ```
  -- To invoke a function, you use the name of the function followed by `()`, and you put inside the `()` values for any of the parameters required by the function definition   
  -- For instance, `greetUser("Jill")`  
  -- The value "Jill" is an argument for the `username` parameter   
  -- The difference between an argument and parameter is that a **parameter** appears in the **function definition** and is like a property of the function (typically because the function requires that parmeter to have a value for the function to work properly) and an **argument** is a **value** that you pass in for each parameter **when you invoke the function**  
  -- If the function definition has a default value for the parameter, calling the function without an argument results in the function using the default value  
  -- Invoking a function causes the code inside the function definition to run 
  -- All functions return a value    
  -- By default, a function returns the value `undefined`; therefore, you you don't explicitly include a `return` statement or if you `return` nothing, then the function's `return` value is `undefined`
  -- You can override that default value by explicitly returning a value, like so:  
  
  ```javascript
  const greetUser = (username) => {
    const message = "Welcome to ITC, " + username
    return message
    }
  ```
  -- A `return` statement makes the value that it's returning available outside the scope of the function definition  
  -- When you invoke a function, to capture the `return` value for use later in your code, you can save a function's `return` value to a variable  
  -- For instance, you can do this: `const userGreeting = greetUser("Jill")`  
  -- `userGreeteing` is equal to the value "Welcome to ITC, Jill"  
  -- Naming is important; you can use good naming to make your code tell a story to your reader and, therefore, easier to understand; notice the function returns a gretting message to a user; a message is a noun, so we named our message as the noun `userGreeting`
  -- The function definition performs an action, which is to greet the user; so the function definition has a verb name of `greetUser`  
  -- Oftentimes when you return a value, you **will** want to save that value to a variable 
  -- A `return` statement ends that block of code, which means that the browser does not read any code appearing inside of the function definition but after a `return` statement    
  
  
  


## [Examples of Functions](#examples-of-functions)    

## [Live Coding](#live-coding)   

The live coding session continues working on the live code from the previous lessons. Here are the tasks:  

1. 
