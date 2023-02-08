---
layout: post
title:  "Debugging Code"
author: Sydney Neslen
description: "Writing code is hard enough, but getting it to actually run? Sometimes it can feel like an insurmountable task. Working for hours on a script just for it to generate a supply of error messages is enough to wear down even the most hardened of programmers. Fortunately, there are a few methods and tricks that can help with identifying and preventing problems in your code."
image: /assets/images/debug.png
---

# Prevention 
The best way to create code with no errors is to avoid creating them in the first place. By using strategies to actively prevent bugs, you will save yourself a substantial amount of time. Taking the few extra minutes to implement these principles is well worth the effort down the road. 

### 1. Walk through the problem
When approaching a problem, you may find yourself immediately jumping into writing the code. This can lead to a lot of wasted work and going in circles. Before you start typing anything, walk through the problem step by step and conceptually describe each piece of necessary code. This allows you to see the desired task as a whole instead of becoming too preoccupied with small sections. The last thing you want is to spend thirty minutes fine-tuning a loop, only to discover that it wasn't actually relevant to your ultimate goal. 

### 2. Run small sections at a time
Sometimes the worst part of fixing code is pinpointing the actual issue. It can be difficult to locate the line that is causing havoc, especially if no error code appears. Instead of waiting until you have finished the whole problem to run your code, run it frequently and regularly throughout the whole process. After each step, check that your code was successful and fulfills its intended purpose. This narrows down the source of a bug to only a few possible lines. The less time you spend searching for the error, the more time you can spend solving it. 

### 3. Write tests for functions
Before writing a function, preparing tests for the desired result can be very beneficial. It also allows you to have prepared code to run once you have completed a function. Python provides a helpful procedure that facilitates testing functions called doctests. Doctests often provide a description of the function, input and output information, and examples of the function with the expected outcome. 

```
def add(x, y):
   """
   Return the sum of x and y
   >>> add(1, 2)
   3
   """
   return x + y
```

Use `doctest.testmod()` to run the tests. 

### 4. Comment and label your code
When revisiting code after a while, it can become pretty difficult to remember the purpose or reasoning behind each line. Make sure to routinely leave a description of each function or even individual lines, especially if they are particularly complex. Writing notes in your code can help you regain your train of thought or understand important details. Commenting is extremely useful when sharing code or collaborating with others. 

### 5. Keep things simple


---
# Solutions
### 1. What do you expect vs what happened (rubber ducking)
### 2. Check for typos
### 3. Use debugging tools
### 4. Use print statements
### 5. Look up the problem/error message
### 6. Ask for help
### 7. Take a break
