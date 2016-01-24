# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The language is called Inform. It has a wikipedia article at <https://en.wikipedia.org/wiki/Inform> and a webpage at <http://inform7.com/>.

# Domain
_Describe the language's domain in five words._

Interactive fiction stories and games.

# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a ContextFree program runs._

I assume this is supposed to be about the language I found, rather than ContextFree.

The process is described at <http://inform7.com/sources/>. It is described as a collection of small programs working in succession. The source code is passed into one of two interpreters depending on what format it's in, and then through a series of compilers, which I would imagine translate it into some kind of object-oriented representation for the objects in the interactive fiction. I'm unsure of the details because the process is not explained in detail. The end result is a single binary file with all of the details of the story. 

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

Inform is purely domain-specific. It very strongly meets all of Fowler's criteria:
* It has an obvious feel of being a language.
* It is very restricted in what it can do; all it can do is define elements of an interactive fiction and how they relate to each other.
* It is clearly focused on a specific domain, and its restrictiveness fits with that focus. 

This is truer of Inform 7 than prior versions, as it overhauled the syntax to be much more English-like. Prior versions resembled general programming languages in their syntax (but without typical general constructs like loops and conditionals).

Inform 7 is very clear-cut as a pure domain-specific language. Earlier versions are still fairly clearly domain-specific languages, but slightly less clearly cut.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

The language is external. It is not part of any greater system, and an Inform program can be understood on its own. It uses its own syntax. There are no obvious vestiges within the language that come from the system in which it was built - it appears to be a completely standalone language.

# Host language
_What language(s) was (were) used to implement the DSL?_

At least pieces of it (some compilers) were written in ANSI C. However, the entire language seems to be a complex system and I think it was written using a number of languages.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

The fact that the language's syntax reads like English is a major benefit to those who want to pick up the language quickly.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

No matter how a DSL for interactive fiction is implemented, it is ultimately going to lose some expressiveness. Because of this, designers using Inform are restricted to giving their interactive fictions' users a restricted kind of interface with commands that have to work with Inform's back-end. 

To that end if someone had a very nonstandard idea for an interactive fiction, it is possible that Inform would not have enough options to express that idea.
