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

The language itself is a plain-text ASCII representation of musical notes and symbols.  Various programs exist that parse these text files and generate TeX commands to ultimately create a musical score. Other output types are also possible.  [ABCJ](http://abcj.ganderband.com/), for example, is an ABC notation editor written in Java that parses ABC notation and outputs MIDI. 

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

With its narrow domain and limited functionality, ABC notation is purely domain specific. 

ABC notation's intended use is to notate simple, single-voice tunes, though it is possible to (awkwardly) notate more complex pieces. In terms of functionality, an ABC notation "program" is simply a text file of ASCII characters, each character representing a musical symbol (eg. a note, tempo marking, accidental, measure line, etc). There are no loops or variables, and the language is not Turing complete, meaning that it cannot be classified as a general-purpose language.

An issue Fowler may have with the classification of ABC notation as a DSL, however, is that it is not purely a "computer language," which according to him is a criterion of being a DSL (top of page 32). The [Wikipedia article](https://en.wikipedia.org/wiki/ABC_notation) on ABC notation (first paragraph) suggests that an ABC notated score can be an end product in itself, fully readable and shareable, even when written on a piece of paper or a napkin.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

The language is an external DSL.  It has its own custom syntax and is written using any text-editor that supports ASCII characters, separate from any specific general purpose programming language.

# Host language
_What language(s) was (were) used to implement the DSL?_

As previously stated, ABC notation can be written in any text editor. Many programs exist to parse this notation and output either MIDI or musical scores, usually by using TeX typesetting. Such programs have been written in [Java](http://abcj.ganderband.com/), [Javascript](https://github.com/paulrosen/abcjs), [Lua](https://code.google.com/p/abclua/), and more.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Combined with a parsing program, ABC notation is likely the fastest method of transcribing simple musical scores.  Notating music directly with TeX is cumbersome, as each musical symbol requires the entering of multiple characters, and using traditional GUI-based notation programs such as Sibelius or Finale requires the combination of the mouse and various keyboard shortcuts.  ABC notation doesn't require you to move from the keyboard and each musical symbol, for the most part, is represented by a single ASCII character.  An experienced user of ABC notation can transcribe a simple score in the time it takes to type a paragraph.  [Example](http://abcnotation.com/getResource/downloads/text_/by-way-of-the-dow.abc?a=thesession.org/tunes/8649.no-ext/0001)

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

A major drawback of ABC notation stems from its simplicity.  There is no intuitive way of notating pieces with multiple voices, and attempting to do so can result in huge text files that are difficult to maintain ([Example - Beethoven's 7th notated in ABC](http://www.ucolick.org/~sla/abcmusic/s7m2p.abc)).  The solution to notating such pieces does not lie in general-purpose programming languages, but rather in the previously mentioend GUI-based notation programs, such as Sibelius.  Such programs allow users to draw notes directly on to scores, and directly support the transcription of multiple-voiced pieces by allowing each voice to be split up into a separate part, with its own score.