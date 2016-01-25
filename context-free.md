# Context Free

##  Who is this programming language for?

This programming language appears to be for anyone interested in vector-based digital art that does not want to go through the hassle of learning a more complete graphics editor, like Photoshop. Although the language itself is not extremely complicated, it seems geared toward someone who has some programming experience.

## What is easy to do in this language? Why is it easy?

I found it simple to generate recurring simple shapes because most of the basic shapes are built in (SQUARE, TRIANGLE, CIRCLE) and the language seems to lend itself to recursion quite nicely.

## What is hard to do in this language? Why is it hard?

I felt that doing something akin to painting, sketching, or any other form of hand-drawn art would be extremely difficult in this language. The programming language must be constructed from a series of lines and shapes; without control over every pixel, it's hard to create something that is not vector-based. On a related note, it's difficult to create any image intentionally in the sense that the programmer has to figure out what shape to recurse on, how to do the recursion, among other things.

## How did you learn how to program in this language?

I learned how to program in this language primarily through examples, such as the Welcome message and user submitted code on the website. Although there was documentation, I found it difficult to follow without more in-depth examples or images. I found experimenting with different values for each rule and noting the visual output helped a lot more than reading through the documentation. Seeing examples and experimenting with them on my own really helped solidify my understanding of the language. After getting a basic understanding of the language, I started playing around with the recursion and shapes until I found an image that I liked.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

When a ContextFree program runs, it parses the code and creates an image on the canvas as it reaches terminals. Much like a context-free grammar, it starts with a root symbol (the startshape) and uses a series of user-defined rules to render an image.

## What do you think is interesting about the ContextFree program you wrote?

I found it interesting how significant small adjustments to the grammar can affect the final image. By changing the starting shape, the scaling factor, or the rotating factor, the final image can look completely different! I also found it interesting how complicated an image made from repeating circles can be. 
