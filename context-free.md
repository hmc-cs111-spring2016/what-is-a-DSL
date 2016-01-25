# Context Free

##  Who is this programming language for?
+ This language is for people who want to programatically create images. 

## What is easy to do in this language? Why is it easy?
+ It is easy to draw images that are made up of many much simpler shapes such as squares, circles etc. This is easy because the definitions for these shapes are already available in the language. 

## What is hard to do in this language? Why is it hard?
+ It is diffcult to draw images that are made up of more complicated shapes or images that might have a more random flow to them (look like they're drawn by hand). This is hard because if the image you are creating cannot be expressed by building off of smaller peices to crete larger pieces then you basically would have to program each pixel of the image by hand. This would take a very long time. 

## How did you learn how to program in this language?
+ I looked at the online documentation and also at the example welcome image shown when the program first started. I also experimented with different code to see what certain functions did. 

## What is the underlying _computational model_ for this programming language? 
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of what 
happens when a ContextFree program runs._
+ Most likely, the ContextFree program starts at the startshape and successively renders each subimage in that startshape. It then renders each sub-sub image and continues to do this until it gets to a base image, a square or a circle, which it draws on the canvas. 

## What do you think is interesting about the ContextFree program you wrote?
+ My program is intereting because it takes advantage of the subroutine model of ContextFree by repeating similar shapes but being able to make very slight changes such as color or orientation. 
