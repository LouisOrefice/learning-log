# 19-05-24 - Beginner/tutorial Course

I have started to create Github learning logs to document my learning journey and help reflect on what I learn each day. Im hoping to show my progression over the next few months.

Today was productive. I'm starting to gain a clearer understanding of JavaScript, though there's still much to learn. I built small projects like a weather app, color picker, and pig game last week, but I didn’t fully grasp how the data flowed at the time. Now, after learning about scopes and the call stack, the logic is starting to make much more sense.

## ✅ What I Did Today

Jonas Schmedtmann Complete JS Course - Zero to Expert! Progress = (102/342) - (113/342)

- Nearly completed section 8 - How JavaScript Works behind the Scenes

## 🔍 What I Learned

Scoping
Scoping determines where variables and functions are accessible — their "visible zone."
JavaScript has three types of scope:

Global Scope:
Variables declared outside of any function or block; accessible anywhere in the code.

Function Scope:
Variables declared with var inside a function are only accessible within that function.

Block Scope (introduced in ES6):
Variables declared with let or const inside {} blocks (like if, for, etc.) are only accessible within that block.
➤ This helps prevent errors where variables are accessed before being declared.

🔑 Within a block or function, code can "look up" the scope chain to find variables — but not down into inner scopes.

🔹 Call Stack
The call stack is like a stack of trays (LIFO - Last In, First Out) that tracks which function is currently running.
Each time a function is called, a new execution context (EC) is placed on the stack.
When a function finishes, its EC is popped off, and control returns to the previous one.
This helps JavaScript keep track of where it is in your code during execution.

🔹 this Keyword
The value of this depends on how a function is called, not where it's defined:

In the global scope, this refers to the global object (window in browsers).

In strict mode, this is undefined in regular functions.

In object methods, this refers to the calling object.

Arrow functions do not have their own this; they inherit it lexically from the surrounding scope.

To preserve this in older code (or in callbacks), developers often assign const self = this.

🔹 JavaScript Engine & JIT
The JavaScript engine (like V8 in Chrome) processes code in two phases:

Compilation: Code is parsed and compiled.

Execution: Code is executed, and the engine uses Just-In-Time (JIT) compilation to optimize performance by compiling code at runtime as it's needed.
Hoisting, TDZ (temporal dead zone) - further study is needed.

## 🚀 Next Steps

- Practice basic JS problems on CodeWars.
- Look into making an asteroid game. - decided after learning more about Js behind the scenes that I lack a concrete understanding of building functions and correct coding structures.
- Focus on understanding object references, use tutorials in Jonas JS Course to develop a deep understanding.
