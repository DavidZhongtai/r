---
title: Loops
weight: 7
---

# Loops

R is perfect at performing repetitive tasks. Like wonderful. If you want an operation to be performed an amount of times, you use something we know as loops. By creating a loop, R will execute the commands inside the loop the amount of times specified.

Loops are found in all programming languages, not only in R. They are a fundamental component of computers.

## For Loop

The for loop is one of the most commonly used loop structures if you want to predefine the amount of times a block of code is run. The most basic example is

    for (i in 1:4) {
        print(i)
    }
    [1] 1
    [1] 2
    [1] 3
    [1] 4

Lets break this down. First we declare the for loop. Then, we declare the inner variable `i`. This is actually dynamic variable that changes upon each iteration of the loop. The statement `i in 1:4` tells us to loop `i` through a sequence `1 to 4`. If we were to do this manually, it would look like the following:

    i <- 1
    print(i)

    i <- 2
    print(i)

    i <- 3
    print(i)

    i <- 4
    print(i)

We are not limited to just basic print operations however, we can also do more complex things. For example, if we wanted to loop through the elements of a vector and change an element, we can also do so:

    vec <- c(1,3,5,7,9)
    for(i in 1:length(vec)) {
        vec[i] <- vec[i] + 1
        print(vec[i])
    }

This is a loop that goes through the elements of `vec` and adds 1 to them and prints it.

## While Loop

Another loop that you will use and encounter (not as much) is the while loop. It is used when you want to keep looping until a specific condition is reached. Plainly speaking, the loop follows English conventions as you have "while this condition is true, keep doing what I want you to do." A simple example of the while loop can be found below:

    i <- 0
    while (i <= 4) {
        i <- i + 1
        print(i)
    }

    [1] 1
    [1] 2
    [1] 3
    [1] 4

Here, the loop will continue to execute the body (code inside the loop) when `i` is less than or equal to 4. Once `i` is greater than 4, the loop will stop. In most cases, the `for` and `while` loops are sufficient for your every day purposes.
