# Context Free

##  Who is this programming language for?

Context Free is for anyone artistically inclined who either has programming experience or is willing to learn some basic programming concepts.

## What is easy to do in this language? Why is it easy?

In Context Free it's very easy to draw images involving patterns of simple geometric shapes.  By combining and transforming squares, circles, and triangles, most shapes can be created in a relatively straightforward manner.  Once you've created your shapes, Context Free's looping syntax allows you to easily create patterns with those shapes.

## What is hard to do in this language? Why is it hard?

It is difficult to create images that have no discernible pattern or repetition.  Without patterns or repetition, one can't take advantage of Context Free's powerful looping mechanism, and instead must draw everything "by hand" (ie by manually entering the parameters for each line and shape in the image).  At this point, there would be little point in using Context Free over a program like AutoCAD.

## How did you learn how to program in this language?

I learned how to program in this language by tackling simple concepts first and then gradually tackling things that were more complex. I started off by drawing simple shapes, and then combined them to create compound shapes.  I then modified those shapes with basic parameters (size, x, y, etc), and finally moved on to using colors and loops.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a Context Free program runs._

According to the [website](http://www.contextfreeart.org/mediawiki/index.php/Context_Free_Art:About), Context Free is written mostly in C++.  Thus, I would guess that when a Context Free program runs, the grammar is parsed and converted into native C++ code.  Each shape, or "rule," might be converted into its own class.  The C++ code would ultimately draw the image and then use the [Anti-Grain graphics library](http://www.antigrain.com/) (as stated on the site) to render a PNG.

## What do you think is interesting about the Context Free program you wrote?

I think the most interesting thing about the program I wrote is its subject matter.  While most examples of Context Free programs I saw were of abstract patterns or vegetation, I tried to create a face. This lent itself well to the organizational layout of a Context Free program. Each facial feature was its own rule (sometimes with its own sub rules), and the "main" rule simply drew the features in their appropriate location.
