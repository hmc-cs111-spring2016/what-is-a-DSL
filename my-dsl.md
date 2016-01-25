# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._
Bootstrap, http://getbootstrap.com/


# Domain
_Describe the language's domain in five words._
Front-end web development beautification


# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a ContextFree program runs._
I'm going to assume this question intends to ask what happens when a 
Bootstrapped program runs. Bootstrap is a JS/HTML/CSS framework that 
contributes to both the functionality and aesthetic during web development.
It provides consistent formatting for elements like tables, headers, etc and 
implements basic interactive tools like radio buttons, dropdown menus, etc.
(Note that it does not do any work to connect client to server.) 



# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 
Bootstrap is more on the domain-specific side of the spectrum. It does not nearly
have the expressivity to implement things like loops or advance logic. It mearly
has the ability to implement predefined web interactions and appearance.


# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._
I claim that Bootstrap is an internal DSL. It is created using common web dev 
languages (HTML, CSS, etc) to be use in conjunction with those very languages.
Furthermore, it displays the characteristic of being built with particular
components of its base languages in order to deal specifically with user interface
features, which Fowler lists as a key attribute of an internal DSL. Note that 
at least JS and HTML can do much more than just UI work. 

# Host language
_What language(s) was (were) used to implement the DSL?_
JavaScript, HTML, CSS, LESS, and Sass


# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_
This tool allows for easy, straightforward beautification during web dev.
Given that people tend to take better formatting more seriously, it is useful
when quickly prototyping an idea in a larger corporation. For a smaller developer,
it can help them save time by easily making a clean web page without having
to put in the effort to learn design principles and the intricacies of languages
like CSS (a not-especially difficult but surprisingly finicky language).


# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_
The use of bootstrap means loss of control over the design of the webpage. If a 
developer chooses to use this, they will be unable to make specific modifications
in terms of spacing, coloring, etc as easily because Bootstrap takes over those
features. Additionally, the website has less personality and is more generic,
which is not as good a strategy when trying to stand out. 
