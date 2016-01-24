# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

The language is the [Fuzzy Control Language](http://ffll.sourceforge.net/fcl.htm).

# Domain
_Describe the language's domain in five words._

Fuzzy logic instead of booleans.

# Computational model
_We don't yet have a great definition of the term "computational model". 
For now, try to come up with the clearest, most concise explanation of 
what happens when a ContextFree program runs._

In simple terms, when a program written in a domain-specific language is run, its purpose is to generate specific code that can be integrated into the application that implements it. In the case of FCL, this would involve the generation of a set of rules and categories beyond the scope of booleans in its parent application. For ContextFree, a specific set of terms (eg. `CIRCLE`) are being transformed into code that the parent application is capable of parsing. In either case, the language generates a configuration file to be evaluated in the context of the general application. 

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

FCL is closer to the general-purpose end of the spectrum because some programming logic (if/else, variable declaration) can be expressed in the language. However, the domain-specific features of the language are how programs become organized into sets of rules (termed `RULES`) and how variables are categorized based on the user's category definitions. FCL has limited features in that it does not implement loops or other capabilities of languages that are not domain-specific.

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

The language is implemented as an external DSL, since it is intended to be a supplement to other programs. It can be used in other applications as a replacement for booleans. FCL has its own syntax separate from the application in which it is being used. Since the entire purpose of the language is to implement fuzzy logic, FCL is not a subset of features of a different language, which would be characteristic of an internal DSL. 

# Host language
_What language(s) was (were) used to implement the DSL?_

FCL is a set of standards defined in the IEC 61131-7 standard for programmable controllers. Compilers and parsers for FCL have been implemented in several different languages. The language itself is constrained by the aforementioned standards. One FCL library is jFuzzyLogic, which has been implemented in Java.

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

Using this DSL, programmers can easily make use of fuzzy logic. With FCL, the programmer can define a set of general rules to categorize unknown values in terms of the specific problem they are trying to solve. The language allows the user to add their own sets of objects and categories in order to solve fuzzy logic problems within their more specific domain. 

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

One potential drawback of the language is that it does not include many keywords. Though FCL is very user-friendly (statements begin to look more like sentences than code snippets), some inuitive modifiers do not exist in the language. For example, the language supports `IF` and `THEN` but does not include a variable modifier such as `VERY`, which would place the object being modified into a different category than if the modifier was not present.
