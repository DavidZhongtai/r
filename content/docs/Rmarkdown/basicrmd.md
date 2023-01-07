---
title: Intro to R Markdown
weight: 1
---

# Intro to R Markdown

You may be asking, why do we need to learn this. However, as important as it is to be able to create quality code, its equally as important to present that code in a readable format. Essentially, you want to develop the skills in order to deliver an effective presentation.

## Installing R Markdown

To use R Markdown, you want to install the `rmarkdown` package in R Studio. You also need to install any necessary dependencies. To do so, just make sure you have R Studio and R installed before this. What we can do is then run the following code statements:

    # Install from CRAN
    install.packages('rmarkdown', dep = TRUE)

    # Or if you want to test the development version,
    # install from GitHub
    if (!requireNamespace("devtools"))
        install.packages('devtools')
    devtools::install_github('rstudio/rmarkdown')

After installing R Markdown, you will have the whole suite open to you to use.
