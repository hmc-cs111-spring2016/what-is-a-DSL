# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The language is [flask](http://flask.pocoo.org/). 

# Domain
_Describe the language's domain in five words._

Light weight framework for web development

# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a ContextFree program runs._

When a Flask program runs, it is interpreted as a Python program. 

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

Flask is closer to the domain-specific end of the spectrum, as it is specific to web development. 

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

Flask would be considered an internal DSL, as it uses a general purpose language (Python) in a particular way (web development). 

# Host language
_What language(s) was (were) used to implement the DSL?_

Flask is written in Python.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

By building a web application with Flask, developers take advantage of the lightweight framework, avoiding much of the overhead typically attributed to a more "full stack" web framework. Additionally, Flask provides more flexibility and granular control with its minimal framework, leaving design choices ultimately up to the developer. Flask also allows developers to take advantage of the Model-View-Controller model, which also contributes to more granular control. 

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

One disadvantage of Flask is the lack of many features normally included in a "full stack" web framework, such as a data abstraction layer, form validation, etc. As such, for larger projects, web applications built with Flask require several additional libraries to fulfill these features -- several describe Flask as a "build what you want and bolt on whatever you need" framework, whereas other frameworks are described as an already complete package. However, it is worthwhile to note that not including these features make most of the aforementioned benefits possible (lightweight framework, granular control, flexibility).
