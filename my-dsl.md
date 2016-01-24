# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The language's name is ABC notation. [Link](http://abcnotation.com/)

# Domain
_Describe the language's domain in five words._

Musical notation, especially folk, traditional

# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a ContextFree program runs._

The language itself is a plain-text ASCII representation of musical notes and symbols.  Various programs exist that parse these text files and output to various formats.  [ABCJ](http://abcj.ganderband.com/), for example, is an ABC notation editor written in Java that parses ABC notation and output MIDI.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

With its narrow domain and limited functionality, ABC notation is purely domain specific. 

ABC notation's intended use is to notate simple, single-voice tunes, though it is possible to (awkwardly) notate more complex pieces. In terms of functionality, an ABC notation "program" is simply a text file of ASCII characters, each character representing a musical symbol (eg. a note, tempo marking, accidental, measure line, etc). There are no loops or variables, and the language is not Turing complete, meaning that it cannot be classified as a general-purpose language.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._



# Host language
_What language(s) was (were) used to implement the DSL?_


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_