# Context Free

##  Who is this programming language for?
It seems to be intended for anyone who wants to create computer art with it. From looking at the gallery, I think there are quite a few math enthusiasts among the user base.


## What is easy to do in this language? Why is it easy?
It's relatively easy to create fractal patterns as I did, provided you know the geometry well enough. Context Free provides graphics primitives so it's really easy to draw squares, triangles, etc., plus you can combine them into "rules" which can be recursive. There are options that can be applied to the primitives that change size, position, orientation, color, and a number of other attributes. It's also possible to call rules with the same options and they will apply to all shapes the rules draw.

## What is hard to do in this language? Why is it hard?
Most complex patterns that are not recursive, repeating, or self-similar in some way would be difficult, or at least time-consuming, to create. I've also seen a few 3D-looking images in the gallery on Context Free's website, and their code is a _lot_ less elegant. Non-repeating patterns are difficult or time consuming simply because if you can't let recursion do the work you have to specify the primitives yourself, and for a complex image that will be quite a lot of primitives indeed.
The 3D images are inelegant because all the primitives are 2D, so quite a few of them are required with various brightness and color differences to create the illusion of depth.

## How did you learn how to program in this language?
I tried to look at the documentation, but it isn't very good and only got me so far. For the most part, I messed around with example code until it did what I wanted it to do, and also looked at code other people in the class wrote to see what was even valid in the first place.


## What is the underlying _computational model_ for this programming language?
_We don't yet have a great definition of the term "computational model".
For now, try to come up with the clearest, most concise explanation of what
happens when a ContextFree program runs._
The program evaluates the starting rule, immediately rendering any primitives it comes across, and then goes into recursive rules. My Koch snowflake seems to indicate that shapes are not drawn in the order one might expect, because some parts of the largest Sierpinski triangle in it apparently overwrite parts of the triangles over its corners.


## What do you think is interesting about the ContextFree program you wrote?
I think the most interesting thing about my program is how simple the code is despite the complexity of the resultant image. Plus, it draws a tree of Pythagoras made out of Koch snowflakes made out of Sierpinski triangles.
