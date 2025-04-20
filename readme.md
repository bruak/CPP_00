# CPP Module 00

This repository contains the exercises for CPP Module 00, an introduction to C++ programming.

## Overview

This module focuses on the basics of C++ including namespaces, classes, member functions, stdio streams, initialization lists, static, const, and other language fundamentals. The code is compiled with C++98 standards.

## Exercises

### Exercise 00: Megaphone

A simple program that takes command-line arguments and outputs them in uppercase.

#### Usage:
```bash
$ ./megaphone "shhhhh... I think the students are asleep..."
SHHHHH... I THINK THE STUDENTS ARE ASLEEP...
$ ./megaphone Damnit " ! " "Sorry students, I thought this thing was off."
DAMNIT ! SORRY STUDENTS, I THOUGHT THIS THING WAS OFF.
$ ./megaphone
* LOUD AND UNBEARABLE FEEDBACK NOISE *
```

### Exercise 01: My Awesome PhoneBook

A phonebook application that allows users to store and retrieve contact information. This program implements a simple contact management system using classes in C++.

#### Features:
- Add new contacts with first name, last name, nickname, phone number, and darkest secret
- Search for contacts by index
- Display all contacts in a formatted table
- Exit the program

#### Commands:
- `ADD`: Add a new contact
- `SEARCH`: Display saved contacts and search for a specific one
- `EXIT`: Close the program

#### Implementation Details:
- Contact information is stored in a class called `Contact`
- PhoneBook class manages up to 8 contacts in an array
- If the user tries to add a 9th contact, the oldest contact is replaced
- Table display formats text longer than 10 characters by truncating and adding a dot

## Compilation

Each exercise comes with a Makefile that supports the following commands:
- `make`: Compile the program
- `make clean`: Remove object files
- `make fclean`: Remove object files and executable
- `make re`: Recompile the entire program

## Requirements

- C++ compiler with C++98 standard support
- Linux/macOS environment recommended

## Notes

All code follows the C++98 standard and has been compiled with the following flags:
```
c++ -std=c++98 -pedantic
```