---
title: More on Vectors and Indexing
weight: 3
---

# More on Vectors and Indexing

After learning more about types and variables, lets talk more about vectors and indexing inside of R.

## **More** Vectors in R

Vectors are the most basic R data objects and there are six types of atomic vectors. They are logical, integer, double, complex, character and raw. When you write a single value in R, it becomes a vector of length 1 and belongs to one of the above types. Essentially, they are a list of items that are the same type.

To make a vector, you can use the `c()` function and seperate the items inside of the vector by a comma. For example, if we wanted to create a vector of restaurants in the UC area, we can do the following:

    > food <- c("Cravings", "Jerusalem", "Sticky Rice")
    > food
    [1] "Cravings" "Jerusalem" "Sticky Rice"

If we wanted to create a vector with numerical values in a sequence, we can use the `:` operator. For example, if I wanted a vector with the numbers 1-10 in a vector, I can do the following:

    > coolNumbers <- 1:10
    > coolNumbers
    [1] 1 2 3 4 5 6 7 8 9 10

## Useful Vector Functions

If we wanted to see the amount of elements inside of the vector, we can use the `length()` function

    > food <- c("Cravings", "Jerusalem", "Sticky Rice")
    > length(food)
    [1] 3

Also, we can also sort a vector as well. Using strings, it goes alphabetically while numeric values are sorted ascending.

    > food <- c("Cravings",  "Sticky Rice", "Jerusalem")
    > sort(food)
    [1] "Cravings" "Jerusalem" "Sticky Rice"

    > numbers <- c(1,4,5,2,3,8)
    > sort(numbers)
    [1] 1 2 3 4 5 8

## Accessing Elements of Vectors

To access elements of vectors, you use this technique known as indexing which is utilizing `[]`. For example, if I wanted to access the first element of vector, I would use `[1]`. Keep in mind that R uses 1-based indexing (arrays start at 1) while a majority of programming languages use 0-based indexing (arrays start at 0).

    > food <- c("Cravings",  "Sticky Rice", "Jerusalem")
    > food[2]
    [1] "Sticky Rice"

## Repeating Vectors

Say if you wanted to repeat a sequence of vectors, you can use the `rep()` function. There are two variants of it. These are `each` and `times`. If we wanted to repeat each element a number of times consecutively, we would use `each` as the following:

    > numbers <- rep(c(1,2,3), each = 3)
    > numbers
    [1] 1 1 1 2 2 2 3 3 3

However, if wanted to string a sequence together an amount of times, we use `times` as following:

    > numbers <- rep(c(1,2,3), times = 3)
    > numbers
    [1] 1 2 3 1 2 3 1 2 3
