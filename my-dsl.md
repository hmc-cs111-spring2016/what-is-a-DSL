# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

[Zillions of Games](http://www.zillions-of-games.com/) is a board game scripting language.

# Domain
_Describe the language's domain in five words._

Grid-Based Board Game Rules

# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a program in your DSL runs._

When a *Zillions of Games*  file is loaded, the game engine creates a board game on the specified grid with the specified rules, and plays the game automatically. 

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

I would say that this language is very much a pure DSL. It literally only has one use-case, the creation of a board game that's played on a grid. If that's not purely domain-specific, I don't know what is. 
I could see a similar kind of language, or an extension of this language being used to just draw things, but that's not the use case, and there are better tools for that anyway. 

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

This language is implemented as an external DSL. It's programs are created in their own separate files (.zrf files), and they run by themselves on top of the underlying engine.

# Host language
_What language(s) was (were) used to implement the DSL?_

Zillions of Games was impemented on top of the Windows .NET framework, so it requires a running Windows engine to work. The actual language itself uses S-expression syntax, so it basically works like Lisp, but with functions limited entirely to defining the rules of the game.  

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

I think the best way to answer this is with an example. Imagine you're a game company writing a game that involves smaller min-games as sub-content. Instead of having to write a new game engine entirely, come up with the graphics settings to make it look right, and write an AI for it, you could just write several tiny rule files that specify these games, and figure out a way to call them. Seems like a much simpler task. With that said, I'm not sure how customizable this is, so it might be the case that it won't fulfill your use case exactly. 

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

The main drawback of this DSL is probably just that its really specific in its domain. If it let you specify arbitrary games, not just board games on a fixed grid, then it might be better, but as it is, if a company decides to use this, and then needs something just slightly more complicated, they'll have to change systems completely. 
