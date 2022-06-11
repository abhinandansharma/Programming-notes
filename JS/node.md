## Node.js

### What exactly is node:
### Let's break it down to basics

"Node.js® is a JavaScript *runtime* built on Chrome's V8 JavaScript engine." (We will revisit this definition)

So vague definition, right?
Notice the words "runtime" & "JavaScript engine",we will look into the details of these two.

Now, look at the code,

## var num = 10;

What does this code do?  

It stores 10 at a memory location and gives that a name 'num', right?
But, It's u who know what that code does. Computers don't, cause they don't recognize it. They only know 0's and 1's, the machine code.
So, When a language is created, we need to create software that can actually understand the syntax, translate it in 0 and 1 & execute it to perform the actual task.

This is what *JS Engine* does.
It takes the JS code & translates it into machine-readable code and executes it.
This is how JS code is executed and the desired task is performed.

Traditionally, we have been executing JS code inside browsers.
Every browser has a JS engine, For eg. Chrome has V8, Safari has Chakra, etc.
These engines r responsible for executing JS code inside browsers.

Now you understand the job of a JavaScript Engine. Great 🔥
Now, Let's focus on understanding what actually a *Runtime* is.
JavaScript is great, indeed, but just declaring objects, arrays, doing the addition of vars is not what we want from JS.
Think about why JS was created.

JavaScript was created to make the web interactive and dynamic. 
Therefore running JavaScript in isolation is not that useful. We need to run it in some *context*. 
What do I mean by context?

When JavaScript runs in a browser, there are many built-in things like Window object, the document(web page), LocalStorage, etc. are provided by the browser to work with.
We access and manipulate this built-in stuff using JS to make the web better, more interactive, & dynamic.

![image](https://user-images.githubusercontent.com/35263182/173177175-fa428784-3921-4555-b522-70d6e8254602.png)

For eg. When a user clicks a button on a web page, we can write JavaScript to access the web page and maybe change the color of the page or maybe, pop up a window.
This way we r actually able to do what JavaScript was originally intended to do.
So, JS + Browser's Context = 🔥

It is quite useful. Awesome, but here is another thing.
When you're running JavaScript in the context of a browser, you can only access things like DOM, BOM, LocalStorage, Timers, etc. but you can not access Operating System and stuff like File System, memory, CPU, etc.

Thus, we can say that the context is kind of limiting the usefulness of JavaScript.
Think about If we can access OS stuff somehow using JavaScript then we can do a lot more useful tasks like reading/writing files, creating servers, talking to databases, handling HTTP requests.

This is where Node.JS comes into the picture.

The creator of Node.JS, Ryan Dahl, came up with an idea to take a JS Engine (As we know It is required to run JS) and provide a richer context to it.
So he took Chrome's V8 engine and embedded it in a C++ program named it Node.JS.

So what he did differently was that he provided a different context, i.e. a different runtime, a different set of built-in stuff like FS module, HTTP module, OS module, and many more. 
This new runtime called Node.JS is installable on various machines like Windows, Macs, Linux.

So, now You can run JS code on whatever machine Node.JS can be installed cause Node has a V8 engine inside it. If you can install Node on a coffee machine you can run JS there too. 
you don't need a browser to run your JavaSript code anymore.

Because Node.JS comes with a richer and different context we can use JavaScript to access those built-in modules and create servers, read/write files, and can do all the stuff that can be done using a programming language like Python or Java.

This made JavaScript not limited to browser only but now we can run JS on a server. This made JavaScript powerful. 
Using this one language we can create Full-Stack applications.
Let's revisit the definition of Node.JS.

Node.js® is a JavaScript runtime built on Chrome's V8 JS engine.
Now you should be able to break this definition.
" Node.JS is JS runtime that let's execute JS code outside of a browser, that is on a server, a local machine. It uses Chrome's V8 engine to actually execute JS".

- src: https://twitter.com/faheem_khan_dev/status/1500093539761496065?s=12&t=f8sjfIoKKDPPbpkfcfw6Uw
