# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

I have found a language called [TikZ](sourceforge.net/projects/pgf/). It's a syntax layer for the PGF package for LaTeX, and makes using it easier.


# Domain
_Describe the language's domain in five words._

Make cool graphics in LaTeX.


# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a program in your DSL runs._

A TikZ "program" will generally be part of a larger LaTeX (or other TeX) document, and will compile along with it. A TikZ program within a LaTeX document is written inside a tikzpicture environment, and will create graphics such as a diagram of a finite-state machine in the document that LaTeX outputs.


# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

This DSL is very close to the purely domain-specific end of the spectrum, especially since in typical use LaTeX itself is arguably a DSL. TikZ is very approximately like a LaTeX version of Python's turtle graphics, only it's about three-quarters declarative, and has quite a few primitives. It isn't really possible to do anything with TikZ except add certain kinds of graphics to LaTeX documents, so it fits the "limited expressiveness" and "domain focus" criteria in Fowler quite well.


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Insofar as any plain text is potentially valid LaTeX, TikZ is valid LaTeX without any extra parsing necessary. I do have further reason to believe that TikZ is at least kind of an internal DSL: it is absolutely possible to, say, use a LaTeX math environment to label nodes in an FSM diagram with mathematical symbols. On the other hand, certain parts of TikZ, such as the format of a command that draws edges between vertices in a graph, would as far as I know be treated as plain text
in ordinary LaTeX. Here's an example of that command as I've used it before:
```latex
        \path[->]
        (s) edge node {$\varepsilon$} (0)
        (0) edge node {0} (-1)
            edge node {1} (1)
            edge node {$\varepsilon$} (e0)
        (-1) edge [bend left] node {1} (0)
            edge node {$\varepsilon$} (e-1)
        (1) edge [bend left] node {0} (0)
            edge node {$\varepsilon$} (e1);
```
Since it does use some actual LaTeX, I'll venture a guess that it is in fact an internal DSL, but it doesn't look much like any other LaTeX I've ever written.


# Host language
_What language(s) was (were) used to implement the DSL?_

As I've already mentioned above, TikZ is a syntax layer for a TeX package, PGF. PGF I'm sure is written in TeX or some variant thereof. TikZ is treated as a separate TeX package from PGF, so I assume that it is also written in TeX, despite not using typical TeX or LaTeX syntax.


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

It makes it quite easy to add various kinds of mathematical graphics (graphs, geometric constructions, and so on) and even graphics that just look kind of similar (like flowcharts) to LaTeX documents.



# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

It does require the user to already know how to use LaTeX or TeX (although considering what TikZ is good at a typical potential user might very well already be familiar).
