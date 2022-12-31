---
title: Types and Variables
weight: 1
---

# Types and Variables

We cover how types work in R and how you should be cognizant of them.

## What are Variables and Types?

In its essence, a type is something that defines what the data can be. Without further ado, lets dive into what a type is. Before we do that, let us cover what a variable is. A variable is something that stores a value of different types. For example, the different types are

- **Numeric**: a number such as 1,2,3,4
- **String**: These are words surrounded by quotation marks such as "hello", "world", "32"
- **Logical**: These are boolean variables which can be either `TRUE` or `FALSE`
- **Vector**: A vector is a sequence of something that is the same type. Think of it as like a list or array. For example: these can be `1 2 3 4` or `"hi" "this" "is" "stats"`
- **Matrix**: A matrix is a rectangle of elements of the same type. You can think of it as a vector of vectors. For example:

        [xx] [,1] [,2]           [xx] [,1] [,2]
        [1,]   1    3      or    [1,] "hi" "hi"
        [2,]   2    4            [2,] "hi" "hi"

- **List**: A list is a vector but it allows different types. For example, a list can be `1, TRUE, "hello"`

## Assigning and Using Variables

Now you know what a variable is, how can you actually use them and manipulate them. The most basic thing to know is that you assign variables with `<-`. Technically, you can also use `=` but only noobs do that. For example, if we want to assign `x` to the value of `7`, we can do the following: `x <- 7`. If you want to see what is stored inside of `x`, you can type it into the command prompt and it should return `7`.

Creating variables is useful because it allows you to reuse those values over and over again inside the current session. You should also see the variable appear on your right-hand side variables' menu. In addition to that, you can also apply arithmatic operations to variables as you would do with numbers. For example, `x + y`, `x * y` are all valid operations. The same story can be said with strings and logicals such as `z <- "I AM STRING"` or `x <- TRUE`

In addition to that, variables are also case sensitive. The variables a `thisVariable`, `ThisVariable` and `THISVariable` are all different.
