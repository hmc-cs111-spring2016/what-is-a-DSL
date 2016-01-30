# Context Free

##  Who is this programming language for?
Context Free seems to target programmers who are also interested in creating art (computer-generated art is a pretty interesting, though unfortunately small, field).


## What is easy to do in this language? Why is it easy?
Context Free specializes in drawing images through recursion. It is really easy to spawn more instances of the shape you're drawing through recursion, and mutual recursion allows for even more diversity in the kinds of images generated.


## What is hard to do in this language? Why is it hard?
Since the output of this program is drawings, this language would not be good for any non-visual task and is limited in the visual tasks it can accomplish. Even drawing stuff other than repetitive / recursive drawings can be difficult, at least before the significant changes in the v3 release.


## How did you learn how to program in this language?
Personally, I like to learn by example. When learning a new programming language, I find it best to start with something that works and modify it until I get a better understanding for how the language works.

I started by looking at the welcome code that shows up when Context Free starts up as well as examples in the documentation in the language. To actually create my program, I started with a version of the flower code from the documentation that I fixed so it would actually compile. I then played with the options in the flower code and studied the documentation more to see how different terms and values affected the resulting output. After iterating over many revisions and trying out a lot of modifications, I finally arrived at my final program with a much better understanding for how the language worked. Interestingly enough 


## What is the underlying _computational model_ for this programming language? 
Judging from the way the output is generated, it looks like Context Free interprets the code and draws shapes as it goes. However, it seems to recurse on the rules in more of a breadth-first than a depth-first approach. So, if a rule spawns 3 more rules, Context Free will first draw the shapes in each of the three sub-rules before moving on to processing any sub-sub-rules specified in each of the three sub-rules.


## What do you think is interesting about the ContextFree program you wrote?
Instead of using one rule to generate the patterns in my image or using multiple independent rules, I used mutual recursion to get a pretty cool-looking pattern. What's especially interesting is both rules weren't very interesting on their own. The first one, with the proper settings, will generate something akin to a Sierpinski triangle. While it looked nice, it wasn't very complex. The second rule on its own generated a lot of circles, but there were too many and I couldn't find some nice parameters to use just that rule to make something interesting. However, when the rules were combined, I got a much better pattern.