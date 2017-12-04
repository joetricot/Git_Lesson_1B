# Command Line Interface!

### Learning Objectives

1. [Creddle Resume Creator](http://creddle.io/)
2. LinkedIn Review
3. GitHub Account Review
4. Understand the GUI vs. Command Line
5. React Introduction

## Leaving the GUI behind

Now that we're all about to become super awesome developers, it's time to leave the GUI behind. GUI stands for **G**raphic **U**ser **I**nterface, and it refers to the visual layer over the computer's actual core. Instead, we'll be using the **C**ommand **L**ine **I**nterface and telling the computer exactly what to do. (_Commanding_ it, as it were... 🤔)

Some benefits of using the CLI:

- **Speed** -- it's much faster to type `touch hello.txt` than it is to make a new text file using the GUI.
- **Precision** -- We're able to look at the commands we're about to enter and see exactly what they're about to do.
- **Tools** -- There are a number of tools we can use in the command line to make our work easier to do.
    - `npm install *thing*`

## Common CLI commands

Commands fall largely into two categories: commands that have **output** and commands that have **side effects**.
- Commands with output generally just tell you about files, directories, or the computer in general.
    - `ls`
    - `pwd`
    - `[thing] -v` -- for example, `node -v`.
- Commands with side effects make changes to the environment.
    - `touch [filename]`
    - `mkdir [directory name]`.

Commands can often be modified using **flags**. For example, `ls` lists all the un-hidden files in a directory, while `ls -A` lists _every_ file, even the hidden ones.

Here are the commands you'll use most frequently:

- `ls` & `ls -A` -- lists all files in a directory
- `cd [somewhere]` -- changes directories to the specified location. The "somewhere" is usually either the name of a directory or `..`, which refers to the parent directory.
- `pwd` -- print working directory. Prints the current directory to the terminal.
- `mkdir [directory name]` -- creates a directory with the specified name
- `touch [file name]` -- creates a file with the specified name

And, of course, the git commands...

Some commands you'll also see frequently:

- `mv [path/to/source] [path/to/destination]` -- moves the material at the source path to the destination path
- `cp [path/to/source] [path/to/destination]` -- copies the material at the source path to the destination path

## ⛔️🙅 Unsafe Commands 🚫🚨

There are some commands that you should try to avoid using.

### `rm [-rf] [a file or folder]`

`rm [-rf] [a file or folder]`, or "remove [recursively by force] [a file or folder]", removes files without any kind of prompt or confirmation. **YOU SHOULD ALMOST NEVER USE THIS COMMAND**. There is **no way** to recover files that have been removed in this way. They do not go in the trash. They are _instantly obliterated from the face of the earth_. Think of `rm -rf` as the fastest way to totally fuck up your entire machine if you run it wrong, or in the wrong place. _Don't use `rm -rf`._
-------------------------

# Introduction to ReactJS

## Objectives

1. Explain some common React terminology
2. Create a React App

## The ubiquity of React

- Everybody uses React... it's being adopted by many companies including Facebook, Reddit, Twitter, Netflix, Walmart, etc. Even other frameworks are incorporating many of its concepts and ideas.
- It can be used everywhere. React Native allows you to transfer your web dev skills to Android and iOS app development.
- Developer happiness
  * Descriptive warnings and errors
  * Great Documentation
- Everyone is loving it right now so there is a _huge_ community. Even the big names are in on the love: Facebook (obviously), Netflix, Reddit, Twitter, Walmart, etc.
  * Even other new frameworks are starting to incorporate the concepts and ideas React is introducing
- It can be used anywhere
  * web & native
- Virtual DOM


## React - a user interface library

- At the core of React are Components, which you can think of as pieces of an user interface. There are lots of moving parts to components but they all have at least a render method that returns a React element.
- React elements are immutable JavaScript objects. React utilizes its "Virtual DOM" to update the browser DOM much faster than normal.
- React is a JavaScript library used to craft modern UI's for front end in web client and native applications (native = mobile / desktop)
  * Note: React is a LIBRARY and not a FRAMEWORK

- First used by Facebook in 2011 and Instagram in 2012. Was finally offered as open source in May of 2013.
- Was originally conceived out of Facebook's need for a solution to ease the process of continuously re-rendering parts of views
- React can be thought of as the view layer

## Thinking in React

### Components

[Components Diagram](http://maketea.co.uk/images/2014-03-05-robust-web-apps-with-react-part-1/wireframe_deconstructed.png)

- In React, you think of your frontend as a collections of *components*. One simple example is a blog. A blog might have a PostList component, a Post component, a CommentList component, a Comment component, and on.
- Each of these components are reusable, composable, and efficient. As we'll see as we move deeper into React, building user interfaces in this manner makes data fetching, handling, and mutating more straightforward.

## React Hello World
- Create a project with CRA called `react-hello-world`
- Go through the architecture of a React application.

### How?
We're going to use `create-react-app`

```
npm install -g create-react-app

```

`create-react-app` = Babel + Webpack

### What is Babel?
- Babel is a transpiler, it compiles Javascript (in our case React/JSX and ES6/7) to Javascript (ES5)
- We use babel to allow us to use ES6 features and JSX

### What is webpack?
- Webpack is a bundler that will run all of our React source code into code that the browser can understand
- Think of it as a function that takes a directory containing React source code as an input, and returns a browser ready version into a new directory as an output
- We **only** touch the source code, we don't ever touch the ouput code

## Lab

Build a basic React app using `create-react-app` and go through the architecture together.
