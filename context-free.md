# Context Free

## Who is this programming language for?
This programming language appears to be aimed at those interested in math
and computer science and want to use those concepts in an artistic manner.
To create anything interesting, basic knowledge of what a program/rule is, 
recursion, etc is necessary. Also, commenting mimics that use in C/Javascript, 
further suggested this is aimed at those with some programming experience.
However, knowledge of more advanced concepts, like class structure or 
control flow, is not necessary to create beautiful pictures, making this
more accessible. It seems like a good way to either build confidence with 
programming or to program just for aesthetic pleasure.


## What is easy to do in this language? Why is it easy?
Recursion and randomization is very straight-forward in this language. This 
becomes quickly evident when looking through the first lesson provided. To
randomize, all one has to do is create multiple rules of with the same name. 
Then, after the name, one puts a number that indicates its weighting relative
to the other same-named rule. This controls how likely one of them is to show up.
To use recursion, all one has to do is put the rule inside of itself and size it 
smaller than the starting rule. The renderer determines when it will be too small
to be seen and stops the recursion there. This is especially convenient, as it 
means the user can implement a limited form of recursion without having to consider
base cases, weird edge cases, etc.


## What is hard to do in this language? Why is it hard?
For me, the hardest part of this language is understanding how the positioning,
sizing, etc will render. The scale and positioning system is very unintuitive to
me, and I found myself surprised by how my changes appeared when rendered. I 
think that adding some sort of reference/grid option that shows how the positioning
works would be useful for gaining intuition. This probably is not necessary for 
more advanced users, but for beginners it could prove helpful. Another concept
I found confusing was how layering works in this program. For example, in 
Photoshop, one can create layers for different objects to specify their
respective z-positioning. However, it was unclear how to control this Context
Free and also what the standard seemed to be.


## How did you learn how to program in this language?
To first acquaint myself with Context Free, I looked through the code for the
welcome image. I took parts of it and copy-pasted it into an example image
to play around with the code and get a general sense of how it worked. This is
how I figured out to use startshape and which rules were built-in. However,
I did not have a good sense of what the specifications were for shapes and how
to use them. To learn these, I turned to the two lessons listed under the help 
menu. This was highly useful. I additionally discovered the recursive 
properties of Context Free and how other rules could be included in a program.
When I was confused about other things I wanted to make happen, I refered to the
examle images to find the code for the properties of interest. In general,
I found that learning by example was effective for this language.


## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._
When a ContextFree program runs, it appears that it compiles all of the 
different rules. It then refers to these rules as necessary. It starts by
going to the rule associated with the startshape command, and then follows
the rest of the as necessary.


## What do you think is interesting about the ContextFree program you wrote?
From an exploring the language perspective, I was able to take advantage of
both recursion and randomization in creating my image. I also played with
formatting features, like positioning and lightening the black. Furthermore,
I used a library to add text. From a artistic standpoint, I tried to have the arrows
lead into the spiral and used the black boxes to frame the edges. As for what it
means, I have no idea, but it is meant to be visually appealing in the way the 
eye follows the lines.

