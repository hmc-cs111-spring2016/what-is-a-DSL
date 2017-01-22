# Context Free

##  Who is this programming language for?

The programming language is for people that want to be able to create digital art without learning how to render it in a different programming language. In ContextFree, the only code that the user needs to write involves the image that they produce. The user does not need to learn about graphics libraries or additional features of a more complex language. In general, ContextFree is optimal for someone who wants to create graphical images who has a basic understanding of computer science.

## What is easy to do in this language? Why is it easy?

It is easy to produce simple shapes in the language because it includes `CIRCLE` and `SQUARE` instructions. In order to produce a simple unit circle, the user only needs to write one rule and does not need to specify any adjustments to the shape. Similarly, it is easy to color the background and size the canvas because of the supported methods in ContextFree. The language makes it intuitive to reposition elements with use of `x` and `y` transformations.

## What is hard to do in this language? Why is it hard?

Without a background in computer science, this language would make it difficult to repeat objects. It is simple to implement recursion (call a rule within itself), but more difficult to understand how to use it. The language includes virtually no debugging and limited error messages. Given its simplicity, this is understandable. As mentioned above, the language seems to be optimized for someone with a basic understanding of computer science who wants to create complex graphics. 

It is also hard to make functions that accept arguments. The documentation includes sections about this but does not include extensive examples. The process of creating a function to rotate and transform a shape (passed to the function as a parameter) is not intuitive or simple in ContextFree.

## How did you learn how to program in this language?

I learned to program in the language through a combination of experimentation and reading the documentation. I began by skimming the documentation for the basic language commands and the specifications for the version I downloaded. I then opened the program and looked at the provided example in order to get a basic understanding of what the various commands were doing. Since the sample program was very easy to compile, I experimented with different values to determine what would affect the visual output. 

Once I had a basic understanding of this process, I chose a simple object (in my case, a tree) and tried to create it from scratch. Through a combination of the documentation, looking through the example code, and lots of trial and error, I was able to complete my task. Fortunately, the language is very easy to compile and it was easy to render my image after each new instruction.

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._

When a ContextFree program runs, all of the code is parsed in the context of the grammar. From my limited knowledge of DSLs, it seems as though the implementation code would specify the rendering for `CIRCLE` and `SQUARE` objects. ContextFree is written in C++, so it seems as though this rendering would use the graphics libraries of that language. Since the two aforementioned shapes are the only terminals in ContextFree, running a program would involve parsing all of the rules in the DSL in terms of these terminals. The program would then be run through the rendering specifications of the DSL and produce the visual output. 

## What do you think is interesting about the ContextFree program you wrote?

In the ContextFree program that I wrote, I tried to experiment with some capabilities of the language, such as rules, loops, and recursion. I also wanted to learn how to control color, especially in the context of loops. The resulting program uses many of these features and ended up looking a bit like the [Cascadia flag](https://en.wikipedia.org/wiki/Doug_flag), which was amusing despite not being my original intention. 
