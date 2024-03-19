# Video: Programming Fundamental

Video transcript

- Hey there.
- Anytime you're learning a new skill from cooking to driving to dancing, you should always start with the fundamentals.
- Programming with R is no different.
- To build this foundation, you'll get familiar with the basic concepts of R, including functions, comments, variables, data types, vectors, and pipes.
- Some of these terms might sound familiar.
- For example, we've come across functions in spreadsheets and SQL.
- As a quick refresher, functions are a body of reusable code used to perform specific tasks in R.
- Functions begin with function names like print or paste, and are usually followed by one or more arguments in parentheses.
- An argument is information that a function in R needs in order to run.
- Here's a simple function in action.
- Feel free to join in and try it yourself in RStudio using your cloud account.
- Check out the reading for more details on how to get started.
- You can pause the video anytime you need to.
- We'll open RStudio Cloud to get started.
- We'll start our function in the console with the function name print.
- This function name will return whatever we include in the values in parentheses.
- We'll type an open parenthesis followed by a quotation mark.
- Both the close parenthesis and end quote automatically pop up because RStudio recognizes this syntax.
- Now we just have to add the text string.
- We'll type Coding in R.
- Then we'll press enter.
- Success! The code returns the words "Coding in R.
-" If you want to find out more about the print function or any function, all you have to do is type a question mark, the function name, and a set of parentheses.
- This returns a page in the Help window, which helps you learn more about the functions you're working with.
- Keep in mind that functions are case-sensitive, so typing Print with a Capital P brings back an error message.
- Functions are great, but it can be pretty time-consuming to type out lots of values.
- To save time, we can use variables to represent the values.
- This lets us call out the values any time we need to with just the variable.
- Earlier, we learned about variables in SQL.
- A variable is a representation of a value in R that can be stored for use later during programming.
- Variables can also be called objects.
- As a data analyst, you'll find variables are very useful when programming.
- For example, if you want to filter a dataset, just assign a variable to the function you used to filter the data.
- That way, all you have to do is use that variable to filter the data later.
- When naming a variable in R, you can use a short phrase.
- A variable name should start with a letter and can also contain numbers and underscores.
- So the variable 5penguin wouldn't work well because it starts with a number.
- Also just like functions, variable names are case-sensitive.
- Using all lower case letters is good practice whenever possible.
- Now, before we get to coding a variable, let's add a comment.
- Comments are helpful when you want to describe or explain what's going on in your code.
- Use them as much as possible so that you and everyone can understand the reasoning behind it.
- Comments should be used to make an R script more readable.
- A comment shouldn't be treated as code, so we'll put a # in front of it.
- Then we'll add our comment.
- Here's an example of a variable.
- Now let's go ahead with our example.
- It makes sense to use a variable name to connect to what the variable is representing.
- So we'll type the variable name first_variable.
- Then after the variable name, we'll type a < sign, followed by a -.
- This is the assignment operator.
- It assigns the value to the variable.
- It looks like an arrow, which makes sense, since it's pointing from the value to the variable.
- There are other assignment operators that work too, but it's always good to stick with just one type in your code.
- Next, we'll add the value that our variable will represent.
- We'll use the text, "This is my variable."
- If we type the variable and hit Run, it will return the value that the variable represents.
- This is a very basic way of using a variable.
- You'll learn more ways of using variables in your code soon.
- For now, let's assign a variable to a different data type, numeric.
- We'll name this second_variable, and type our assignment operator.
- We'll give it the numeric value 12.5.
- The Environment pane in the upper- right part of our work space now shows both of our variables and their values.
- There are other data types in R like logical, date, and date time.
- R has a few options for dealing with these data types.
- We'll explore them later.
- With functions, comments, variables, and data types, you've got a good foundation for working with R.
- We'll revisit these throughout this program, and show you how they're used in different ways during analysis.
- Let's finish up with two more fundamental concepts, vectors and pipes.
- Simply put, a vector is a group of data elements of the same type stored in a sequence in R.
- You can make a vector using the combined function.
- In R this function is just the letter c followed by the values you want in your vector inside parentheses.
- All right, let's create a vector.
- Imagine this vector is for a measurement data that we need to analyze.
- We'll start our code with the variable vec_1 to assign to the vector.
- Then we'll type c and the open parenthesis.
- Then we'll type our list of numbers separated by commas.
- We'll then close our parentheses and press enter.
- This time when we type our variable and press enter, it returns our vector.
- We can use this vector anywhere in our analysis with only its variable name vec_1.
- The values in the vector will automatically be applied to our analysis.
- That brings us to the last of our fundamentals, pipes.
- A pipe is a tool in R for expressing a sequence of multiple operations.
- A pipe is represented by a % sign, followed by a > sign, and another % sign.
- It's used to apply the output of one function into another function.
- Pipes can make your code easier to read and understand.
- For example, this pipe filters and sorts the data.
- Later, we'll learn how each part of the pipe works.
- So there they are, the super six fundamentals: functions, comments, variables, data types, vectors, and pipes.
- They all work together as a foundation for using R.
- It's a lot to take in, so feel free to watch any of these videos again if you need a refresher.
- When you're ready, there's so much more to know about R and RStudio.
- So let's get to it.
-

## Question & Notes

The basic concepts of R:

- **Functions**: a body of reusable code used to perform specific tasks in R
- **Argument**: an argument is information that a function in R needs in order to run
- **Comments**: Comments are helpful when you want to describe or explain what's going on in your code.
- **Variables**: is a representation of a value in R that can be stored for use later during programming.
  - A variable name should start with a letter and can also contain numbers and underscores.
- **Data types**
- **Vectors**: a group of data element of the same type stored in a sequence in R
- **Pipes**: a tool in R for expressing a sequence of multiple operations, represented with `%>%`

### Question 1: Fill in the blank: In R, the _____ is information that a function needs to run

- [x] `argument`
- [ ] operator
- [ ] variable
- [ ] comment

> In R, the argument is information that a function needs to run.

### Question 2: In R, a variable name should begin with a number or an underscore

- [ ] True
- [x] False

> Correct: A variable name can contain numbers and underscores, but it should begin with a letter.

## Keypoints

The video introduces the fundamental concepts of programming in R, including functions, comments, variables, data types, vectors, and pipes. Here's a breakdown of each concept:

1. **Functions**: Functions in R are reusable blocks of code used to perform specific tasks. They begin with a function name followed by one or more arguments in parentheses. An argument provides the necessary information for the function to execute.

2. **Comments**: Comments in R are used to describe or explain code. They start with a "#" symbol and are used to improve code readability and understanding.

3. **Variables**: Variables in R are representations of values that can be stored and manipulated in code. Variable names should start with a letter and can contain numbers and underscores.

4. **Data Types**: R supports various data types such as numeric, character, logical, date, and datetime. These data types determine how data is stored and processed in R.

5. **Vectors**: Vectors are sequences of data elements of the same type stored in R. They can be created using the `c()` function and are used to store and manipulate data efficiently.

6. **Pipes**: Pipes, represented by `%>%`, are used in R to express a sequence of multiple operations. They allow the output of one function to be passed as input to another function, making code more readable and concise.