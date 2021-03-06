# B4_Assig

Option A – Strings and functional programming in R
Complete 2 of the following 3 exercises using concepts and tools covered in class (i.e. stringr, purrr, regex, tidyverse, etc.)

Setup: Make a new repository if you’re going with this option, by clicking the link provided to you on canvas. Name the repository as you wish.

Exercise 1 (37.5 points)
Take a Jane Austen book contained in the janeaustenr package, or another book from some other source, such as one of the many freely available books from Project Gutenberg (be sure to indicate where you got the book from). Make a plot of the most common words in the book, removing “stop words” of your choosing (words like “the”, “a”, etc.) or stopwords from a pre-defined source, like the stopwords package or tidytext::stop_words.

If you use any resources for helping you remove stopwords, or some other resource besides the janeaustenr R package for accessing your book, please indicate the source. We aren’t requiring any formal citation styles, just make sure you name the source and link to it.


Exercise 3 (37.5 points)
For this exercise, you’ll be evaluating a model that’s fit separately for each group in some dataset. You should fit these models with some question in mind.

Examples (do not use these examples):

Maybe your model is a linear model (using lm()) for each country’s life expectancy over time in the gapminder::gapminder dataset, where you are interested in each country’s overall trend in life expectancy.
Maybe your model is a distribution of body mass (using the distplyr package) for each penguin species in the palmerpenguins::penguins dataset, so that you can produce parametric prediction intervals (such as from a Normal distribution instead of using the quantile() function) for each species.
Your tasks are as follows.

Make a column of model objects. Do this using the appropriate mapping function from the purrr package. Note: it’s possible you’ll have to make use of nesting, here.
Evaluate the model in a way that interests you. But, you should evaluate something other than a single number for each group. Hint: you’ll need to use another purrr mapping function again.
Print out this intermediate tibble for inspection (perhaps others as well, if it makes sense to do so).
Unnest the resulting calculations, and print your final tibble to screen. Make sure your tibble makes sense: column names are appropriate, and you’ve gotten rid of columns that no longer make sense.
Produce a plot communicating something about the result.
Walk a reader through this analysis by providing an explanation as to what’s going on (in terms of a data analysis question and results, not necessarily in terms of what’s happening in the code).
Grading is as follows:

5 points: the “story” behind your data analysis.
5 points: the plot.
15 points: the calculations.