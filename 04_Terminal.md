# Part 4: Terminal

## Terminology
* **Terminal** or **console**: the program we interact with
* **Command** ("array of strings named arguments; argument 0 is the command name; also called positional parameters)
* **Option** (e.g. "ls -a") -> a is the option (long options also exist; e.g. -v / --verbose)
* **Parameter** (extra info supplied to an option e.g. output -o filename.txt)

Excellent post on [StackOverflow](https://stackoverflow.com/a/36495940).

## Terminal basics
* Understanding the concept of a user
* What is a shell
* What a terminal gives us access to
* Understanding Windows vs Mac vs Linux terminals and limitations
* Understanding filesystem (may require [X01](/X01_Computers.md) knowledge)

## Basic commands
* **man**: Request manual for specific program
* **pwd**: Prints current working directory (Print Working Directory)
* **cd**: Changes the active directory (Change Directory)
* **cat**: Concatenate file to output (conCATenate)
* **ls**: List file directory contents (LiSt contents)
* **cp**: Copy file or directory
* **mv**: Move/rename file or directory

# Advanced commands
* ln: Link files
* ps: List processes that are active (usually `ps aux`)

# Combining commands
* mkdir hello && cd hello && git init

# Piping
* cat sample.txt | grep hello
* ps aux | grep user
* cat sample.txt | grep hello > out.txt