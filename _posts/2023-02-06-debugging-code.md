---
layout: post
title:  "Bugs, Snakes, and Ducks Oh My! A Guide to Avoiding Pesky Errors"
author: Sydney Neslen
description: "Debugging python code can be tedious, but here are some helpful tips to make the process much easier!"
image: /assets/images/debug.png
---

Writing code is hard enough, but getting it to actually run? Sometimes it can feel like an insurmountable task. Working for hours on a script just for it to generate a supply of error messages is enough to wear down even the most hardened of programmers. Fortunately, there are a few methods and tricks that can help with identifying and preventing problems in your code.

# Prevention 
The best way to create code with no errors is to avoid creating them in the first place. By using strategies to actively prevent bugs, you will save yourself a substantial amount of time. Taking the few extra minutes to implement these principles is well worth the effort down the road. 

#### 1. Walk through the problem
When approaching a problem, you may find yourself immediately jumping into writing the code. This can lead to a lot of wasted work and going in circles. Before you start typing anything, walk through the problem step by step and conceptually describe each piece of necessary code. This allows you to see the desired task as a whole instead of becoming too preoccupied with small sections. The last thing you want is to spend thirty minutes fine-tuning a loop, only to discover that it wasn't actually relevant to your ultimate goal. 

#### 2. Run small sections at a time
Sometimes the worst part of fixing code is pinpointing the actual issue. It can be difficult to locate the line that is causing havoc, especially if no error code appears. Instead of waiting until you have finished the whole problem to run your code, run it frequently and regularly throughout the whole process. After each step, check that your code was successful and fulfills its intended purpose. This narrows down the source of a bug to only a few possible lines. The less time you spend searching for the error, the more time you can spend solving it. 

#### 3. Write tests for functions
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
DigitalOcean has a [helpful tutorial page](https://www.digitalocean.com/community/tutorials/how-to-write-doctests-in-python) that goes more in-depth on writing and using doctests. 

#### 4. Comment and label your code
When revisiting code after a while, it can become pretty difficult to remember the purpose or reasoning behind each line. Make sure to routinely leave a description of each function or even individual lines, especially if they are particularly complex. Writing notes in your code can help you regain your train of thought or understand important details. Commenting is extremely useful when sharing code or collaborating with others. 

#### 5. Keep things simple
Using one function to fulfill multiple tasks can appear efficient, but can prove to be frustrating in the long run. Creating complex code can make it difficult to fix or change later; editing one line can cause the entire function to fail. The best approach is to write functions with a singular purpose when possible. 

---

# Solutions
Even with an arsenal of skills to prevent mistakes, they are unfortunately inevitable. Debugging can be frustrating to say the least, but these tips can make it much less daunting. 

#### 1. The rubber duck method
<img src="https://raw.githubusercontent.com/sneslen/my386blog/main/assets/images/rubberduck.jpg" alt="" style="width:400px;"/>
Similar to the first prevention strategy, explaining the problem in your own words can be enlightening. This is dubbed "rubber duck debugging". To do this, just describe the problem to a rubber duck (or another inanimate object) in simple terms. Inform the duck of what you wish the code to do versus what it is currently doing. Talk about what you've tried as well as potential solutions.  Speaking out loud can shed light on a hidden bug or provide helpful insight. 

#### 2. Check for typos
Searching high and low for an error only to discover that it was a missing parenthesis all along can be slightly rage-inducing. Even though typos can be fairly common, they are often overlooked as the cause of a bug. These are especially difficult to locate because they are often one character hiding among hundreds or thousands. Looking at your code thoroughly instead of skimming through it can help you spot the issue. You can also try retyping pieces of code to see if there are any differences. Many code editors such as Visual Studio Code are useful for identifying typos. Different types of code turn various colors, and elements such as quotation marks, parentheses, and indents are automatically generated while you type. 

#### 3. Use debugging tools


#### 4. Use print statements


#### 5. Look for help


#### 6. Take a break
If all else fails, walk away from the problem. Hitting a wall is certainly frustrating, but attempting to get through it over and over again with no progress can often lead you away from the solution instead of towards. Sometimes your viewpoint is too narrow and you're just too close to the problem. Giving yourself a break can provide a fresh perspective and renewed energy when you return. 