# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._
The program is called JAGS (Just another Gibbs Sampler). The relevant webpage is [here.](http://mcmc-jags.sourceforge.net/)

# Domain
_Describe the language's domain in five words._
Bayesian hierarchical models (statistical inference).

# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a program in your DSL runs._
The programmer specifies exactly what type of computation wants to be used be specifying a "model", which is essentially a function or method in the language. This can be something like a basic linear regression. Then, the program will compute the result using Bayesian inference techniques and return those results. These results can easily be displayed/graphed in certain cases using R.

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 
This language is fairly domain specific as it focuses on Bayesian statistical inference using Markov Chain Monte Carlo (MCMC), and doesn't have too much to offer outside of that. While there is plenty that can be (and has been) done using JAGS and in the world of statistical inference/analysis, it still seems domain specific because of the subset of statistical inference offered. 

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._
I think that JAGS is an external DSL. It has its own syntax and is separate from the language it works with (usually R and C++).

# Host language
_What language(s) was (were) used to implement the DSL?_
JAGs was written in C++.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_
JAGS is platform independent, unlike many of its competitors (like, for example, BUGs), and as such I could imagine that this would make it easier to work on larger group projects. Additionally, being written in C++ and easier to include than other Gibbs samplers, it gives a developer more flexibility in use.

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_
Online reviews seemed to indicate that the software was **very** buggy when used with external programs like R. I may have simply stumbled on some frustrated corners of the Internet, but it seemed that the benefits of using JAGS may have been outweighed by the headache.
