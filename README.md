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

##Lexical this:
- 







