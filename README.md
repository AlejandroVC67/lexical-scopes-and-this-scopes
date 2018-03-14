# lexical-scopes-and-this-scopes

## Scope:
- Ability to store values in variables, an later retrieve or modify those values

## Program State:
- State of the variables

Where do those variables live and how the program find them

Well-defined set of rules for storing variables in some location, and for finding them later

## Compiler Theory:

- Javascript is an interpreted language (used to be)
  now its Just In Time (Compiled): Steps ->  Tokenizing / Lexing (word by word), Parsing (Sentences), Code-Generation (Generates machine code)

- Javascript engine is more complex than that

- Javascript code is copiled before executed.

- CODE

## Type of errors: 
-  ReferenceError: cant find the reference
-  Undefined the value exits but it's undefined
- TypeError: When you can't do w/e you're doing

## Lex time:
- The first traditional phase of a standard language compiler
- Examines a string of source code characters and assigns semantic meaning to the tokens as a result of some stateful parsing
- It's based on where the developer created variables 
- In hoisting the first run it's Lex time
- CODE(var  and let in a for)
- CODE (Set time out)

## Hiding in plane scope:
 - Function expression
 - Function declaration

## Look up:
- Think in terms of Tree
- Global variables are property of the global object

## Function & block Scope:
- If, for, () => {}, function, while.

## Cheating Lexical:
- Eval (Webpack uses it)
- With

## IIFE:
- It's used so that you can't create global variables so the function inside an IIFE are expresed not declared 

- CODE(IIFE)

## Hoisting:
- CODE (a = 2, var a, console.log(a))
- First read the file in lex time and saves it in memory(The definition)
- Each scope has it's own hoisting
- Function declaration > Variable declaration (functions go first)
- Variables just "move" the declaration, no the assignment

## Closure:
- When a function remembers its lexical scope even when the function is executed outside that lexical scope
- The action of save the reference or definition 
- CODE (const name =  'Andres', function sayHello (){...} )

##Closures in the wild:
 - CODE(for with setTimeOut)

## Lexical this:
- Only happens when its used inside arrow functions 
- CODE (Run in Browser)
- You can't hardbind an arrow function therefor the this value outside that arrow function is the same in the arrow function 

## This Scope:
- First is not or has nothing to do with:
 - Is not an author time binding but a runtime binding
 - Has nothing todo with where a function is declared
 - Is not the function itself
 - It does not refer to a function lexical scope

- What it is? How can i know the value?
 - Determing the this binding for and executing function
 - Four rules can be applied to the call-site, in this order of precedence:
  - 1. Called with new? use the newly constructred object
  - CODE
  - 2. Called with call, apply or bind use the specified object
  - CODE 
  - 3. Called with a context object owning the call? use the context object
  - CODE 
  - 4. Default: Undefined in strict mode, globacl object otherwise
   - If you put 'use strict' that block of code will be in strict mode 







