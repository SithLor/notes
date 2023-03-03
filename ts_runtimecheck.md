# Suggestion

Add Runtime typecheck to Typescript as option in tscofig.json 
The 

## 🔍 Search Terms

<!--
  💡 Did you know? TypeScript has over 2,000 open suggestions!
  🔎 Please search thoroughly before logging new feature requests as most common ideas already have a proposal in progress.
  The "Common Feature Requests" section of the FAQ lists many popular requests: https://github.com/Microsoft/TypeScript/wiki/FAQ#common-feature-requests

  Replace the text below:
-->
runtime typechecking type functions
## ✅ Viability Checklist

<!--
   Suggestions that don't meet all these criteria are very, very unlikely to be accepted.
   We always recommend reviewing the TypeScript design goals before investing time writing
   a proposal for ideas outside the scope of the project.
-->
My suggestion meets these guidelines:

* [ ] This wouldn't be a breaking change in existing TypeScript/JavaScript code
* [ ] This wouldn't change the runtime behavior of existing JavaScript code
* [ ] This could be implemented without emitting different JS based on the types of the expressions
* [ ] This isn't a runtime feature (e.g. library functionality, non-ECMAScript syntax with JavaScript output, new syntax sugar for JS, etc.)
* [ ] This feature would agree with the rest of [TypeScript's Design Goals](https://github.com/Microsoft/TypeScript/wiki/TypeScript-Design-Goals).


## ⭐ Suggestion

<!-- A summary of what you'd like to see added or changed -->

## 📃 Motivating Example
It would improve the Typescript by closing closing the gap javascript and typescript 
by typecheck function,method, variables

lib.ts
```ts 
function add(base_num:number,mod_num:number){
   return base_num + mod_num
}
```
lib.js
```js 
function add(base_num,mod_num){
   if (typeof(base_num) === 'number'){
            new Thorw Error(`Arg 1 Must Be type of String`)
   }
   return base_num + mod_num
}
```
main.js
```js
import {add} from './dist/lib.js'
console.log(add("2"+2)//this fail for secound arg for being a string
console.log(add(2+"3")//this fail for secound arg for being a string
```
## 💻 Use Cases
Better Runtime check For node,web and npm package.It will type declation 

