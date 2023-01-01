---
title: Functions
weight: 8
---

# Functions in R

We covered basics of R, how to create new variables, and other things. Now, we work on creating modular pieces of code, known as 'functions' to reuse over and over again.

## Introduction to Functions

We have already seen some functions in action. For example, `c()` creates a vector of elements inside. Other functions such as descriptive statistics methods (mean, median, mode, range) all have a method built in as well. For example:

    vec <- c(2, 3, 1, 6, 4, 3, 3, 7)

    mean(vec)
    [1] 3.625

    var(vec)
    [2] 3.98214

    sd(vec)
    [3] 1.995531

With the knowledge we accumulated earlier, if we wanted to use any of these values later, we can assign them to a value as well.

    meanvec <- mean(vec)
    meanvec
    [1] 3.625

However, what about creating your own functions. The general format of creating your own functions is

    nameOfFunction <- function(argument 1, arugment2, ...) {
        expression 1
        expression 2
        ...
    }

Once you run the above code, you are able to run your function regularly like `nameOfFunction(argument 1, argument 2)`. That may seem a bit confusing, so lets run through an example. Say that we wanted to count the number of total elements in two vectors. We first provide the following function:

    sum_elements <- function(x,y) {
        temp = length(x) + length(y)
        return(temp)
    }

We follow the original notation of declaring a function called `sum_elements` that takes in two arguments `x` and `y`. You may notice that there is a new function (or keyword) inside: `return()`. In fact, a return statement is not required for every function but it is in best practice to put one. Essentially, it tells you what to return. In the case of our function, it returns the value of temp.
