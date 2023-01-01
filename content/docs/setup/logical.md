---
title: Conditionals and Logicals
weight: 9
---

# Conditionals and Logicals

How do we be logical inside of R? For example, `x + y` does not imply any logic here, it just tells us to add things together. Conditional statements allow us to add logic into our functions, furthering making our functions better.

Let us continue with an example. Say we want to return the predicted weather based on the current temperature in a function. We first provide the function below before going over it.

    weatherPredict <- function(temp) {
        if (temp >= 10 && temp <= 35) {
            return("snow")
        } else if (temp > 35 && temp <= 65) {
            return("rain")
        } else {
            return("sun")
        }
    }

Here, we declare the same function declaration above where we make a function names `weatherPredict` which takes in one argument `temp`. Then, we use conditionals `if` in order to check conditionals. Generally, an `if-else` statement has the following syntax:

    if (condition) {
        code executed when condition is TRUE
    } else {
        code executed when condition is FALSE
    }
