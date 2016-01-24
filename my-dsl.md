# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

Although the reading says configuration files are not always DSLs, I believe
Vim's configuration language constitutes a DSL. Referred to by a number of
names, such as _.vimrc_, _Vim Configuration Files_, _Vimscript_, etc., the
Vim's configuration language enables a powerful way to customize nearly every
aspect of a Vim user's experience.

[Documentation](http://www.vim.org/docs.php)



# Domain
_Describe the language's domain in five words._

Vim users want customizable experiences.



# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a program in your DSL runs._

When a Vimscript runs, it modifies aspects of a Vim sessions environment.
This can include graphical options, syntax highlighting, and even addon
extensions.



# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

The Vimscript language is certainly closer to the "purely" domain-specific
side of the spectrum than the general-purpose languages side. This is because
the _vimrc_ commands only expose a very limited subset of commands with the
sole intention of customizing a Vim user's experience. 
[Here](http://vim.wikia.com/wiki/Example_vimrc) you can see an example of 
a _.vimrc_ file. Notice how there appears to be no functionality for a complex
non-domain specific task. Although constructs such as loops do exists, they are
a more advance feature frequently used with macros. Similarly the extensive
syntax highlighting scripts have a limited use beyond customizing text display.
An example of a syntax script can be seen
[here](http://vim.wikia.com/wiki/Creating_your_own_syntax_files).

Although some developers have done some really funny and clever things using
Vimscript and their Vim customization files, including some plugins that
replicate an entire IDE in text form, the scope of these commands is greatly
limited and focused to extending and customizing a text editor.

That being said, someone has made a stand alone game to teach Vim where the
controls and puzzles are all related to Vim's keys and commands. I guess that
means this language can be used beyond the scope of editor customization, but
that's the joke of the game, not a _real_ use case. Check it out
[here](http://vim-adventures.com/).



# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Vimscript appear to be an external DSL. This is because although it is
interpreted by Vim on startup or during execution, it is not an extension
of another language like jQuery is to JavaScript or Django is to Python.
Additionally, Vimscript will not run in another environment such as Java, C++,
or JavaScript. That being said, even though it is a stand-alone language, 
Vimscripts do not compile, even though they can sometimes be used to
call external compiled code.



# Host language
_What language(s) was (were) used to implement the DSL?_

Since Vimscript is interpreted by Vim, its features were written and
implemented within Vim. Since Vim was written in C, Vimscript is technically
implemented within C as well.

The GitHub repo for Vim can be found [here](https://github.com/vim/vim).



# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Vimscript enables a highly customizable environment within a text editor unlike
most other editors. Without an extensive Vimscript system, this degree of
customization would be challenging, if not impossible, without having to
manually edit source code. In the end, this allows developers to design a
customized editor that maximizes ease (after the learning curve) and workflow.



# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

Vimscript, especially in more advanced applications, can get very complicated.
Although this inherent, since it enables so much power, it makes there be a
significant learning curve that serves little purpose beyond the scope of Vim.
If a general purpose language was used, it would require less domain knowledge
about Vim to do simple customizations. That being said, having to implement
complex customizations within someone else's C code would be a much more
daunting nightmare.


