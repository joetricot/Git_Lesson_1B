# Command Line Interface!

## First, things first!

1. [Creddle Resume Creator](http://creddle.io/)
2. LinkedIn Review
3. GitHub Account Review

### Learning Objectives

- Understand the GUI vs. Command Line
- Analyze the benefits of using the CLI over the GUI
- Navigate file structure using the command line
- Create new files and directories without using the GUI

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

## 🚀 Lab time!

Use your new command line skills to create this structure on the command line!! (If you're stuck, ask a neighbor!)
