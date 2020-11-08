---
layout: post
title: Postfix Lab
subtitle: 2.3
tags: [lab]
comments: true
---

### Findings
I found that the mean of the values 100 postfix expressions is 529.91.

### Methodolgy
This result was found by running code that evaluates each of the expressions with a method that relies on two stacks. In this write-up, I will call it the **first stack** and **second stack**. The method starts by putting the values of the expression (which exists in the form of a list) into the first stack. Then, one by one, it checks whether the value on the top of the first stack is a number or operator. If it is _not_ an operator, it pops the value off into the second stack. If it _is_ an operator, however, it takes the last two values from the second stack (if they exist) and does that operation on them. The last two are on top of the second stack due to the last-in first-out nature of stacks. Then, it pops every value off of the second stack and pushes it onto the first stack. The method repeats this method until the

As you can see, this procedure very efficient when stacks are used.

As for the cvs module, I go row by row (expression by expression) running the evaluate method and adding the result to a master sum that was finally divided by the number of rows (expressions).

### Process

I stared off by trying to use a queue to do this. However, I realized that the nature of postfix notation lended itself perfectly to stacks (as can be seen above).

I tried to find a way to convert the operator in the form of a string to a operator which can actually operate on numbers in Python. This would make it so that I could have only one line of code instead of a series of conditionals, which look like this:

~~~python
if current_val == "+":
    res = temp2 + temp1
elif current_val == "-":
    res = temp2 - temp1
elif current_val == "*":
    res = temp2 * temp1

# where temp1 is the first value popped
# off of the second stack and temp2 is
# the second value popped off of the second
# stack.
~~~

I couldn't find a way how to do this; notwithstanding, my code is able (if not in the most efficient way) to execute its task.

### Muffin Recipe

Here is, [the muffin recipe](https://www.kingarthurbaking.com/recipes/thanksgiving-muffins-recipe). Getting ready for Thanksgiving? These are to die for!