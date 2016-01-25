# Language
_What is the name of the language? Link the name to its webpage 
(if appropriate)._

+ I chose the SumoLogic query language
+ https://service.us2.sumologic.com/help/Default.htm#Search_Example_Cheat_Sheets.htm


# Domain
_Describe the language's domain in five words._

+ Searching / Querying application log data

# DSL-ness
_Fowler writes about a spectrum of languages, from general-purpose languages to 
"purely" domain-specific. Where does the DSL you chose fall on this spectrum, 
and why?_ 

+ I would classify this language as purely domain-specific because it is not turing complete. It also lacks many features that Fowler points out are necessary for a general-purpose language such as, "conditions, looping constructs and variables."

# Internal or external?
_Is the language implemented as an internal or external DSL? 
Justify your answer._

+ This is an external DSL because programs in this language are not valid syntax for any other programming languages.

# Host language
_What language(s) was (were) used to implement the DSL?_

+ The language is based mostly on SQL queries and syntax and also include Regex for matching log messages. 

# Benefits
_Identify one potential benefit of the DSL: how is a programmer's life or a 
company's bottom line made easier by the existence of this language?_

+ One benefit of this language is that a company can search its application log messages through a language with a low learning curve. Because the language is based off of SQL syntax, it is easy to understand but at the same time provides funtionality specific for searching log messages. 

# Drawbacks
_Identify one potential drawback of the DSL: what does a programmer or company 
lose by using this DSL instead of a general-purpose language?_

+ One drawback of the language is that some aggregations and combinations of log messages are impossible to implement. For example, say for some reason you wanted to pick one out of every 5 messages that matches a certain regex it would not be possible. Or if you wanted to pick out a random log message, it also would not be possible. the language just does not allow for all possible manipulations of log data. Another example is that the language does not allow for things like 'if then' expressions. 
