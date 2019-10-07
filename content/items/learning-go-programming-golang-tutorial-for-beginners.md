---
title: "Learning Go Programming - Golang Tutorial for Beginners"
date: 2019-10-04T21:31:41+02:00
itemurl: "https://www.youtube.com/watch?v=YS4e4q9oBaU"
sites: "youtube.com"
tags: ["golang", "tutorial", "video"]
draft: false
---

## Variable declaration


- **`var foo int`** declare and initialise later; useful for 
- **`var foo int = 42`** useful when compiler might guess the variable type wrong
- **`foo := 42`** declare and initialise shorthand. let compiler decide type
- variables cannot be redeclared but can be assigned new values
- all variables must be used

## Visibility

- lowercase first letter for package scope; variable is available and is accessible to all source files that available in that package\
- uppercase first letter means variable will be globally scoped and will be exported
- there is no private scope, however you can blockscope

## Naming conventions

- use Pascal or camelCase for naming variables
- capitalise acronyms (HTTP, URL)
- variable names should be as short as reasonable. variables with longer life spans within the code should have longer and more meaningiful names

## Type conversions

- in Go the destination type we want to convert to is used somewhat like a function and we pass the variable to be converted as a parameter. **`destinationType(variable)`**
- for strings we use the **`strconv`** package