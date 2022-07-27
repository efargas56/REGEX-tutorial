# Email validation REGEX Tutorial 

Welcome, this is a tutorial on what and how to use this Email REGEX (Regular Expression).

## Summary

This is a regular expression that checks to see if your email is valid. it uses a series of special characters to make sure the information you are entering is accepted by the username text box you are trying to input into.
this is the email REGEX we will be using in this tutorial.
([\da-z\.-]+)\.([a-z\.]{2,6})$/
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
([\da-z\.-]+)\.([a-z\.]{2,6})$/
this is the REGEX code for this tutorial which is used to validate an email string.
### Anchors
Anchors are the type of validator tool the regex uses.
this regex uses the ``` ^ ``` at the beginning of the code to signify the begnning of the string its looking for.
at the end of the code there is a ``` $ ``` at the end this is to tell the regex code that this is the end of the string and that all the inputs its looking for or not looking for have been identified.

### Quantifiers
Quantifiers are the part of your regex that tells it how many times to look for something  in the code or to make sure something is not in the code.
At the end of the first half ``` ([\da-z\.-]+)``` there is a ** + ** symbol that symbol is used to tell the code that you need to fulfill this requirement atleast one or more times in order for the regex to go through.
There is also quantifiers in the middle and end of the code surrounding the second half of the regix here ```([\da-z\.-]+)\.([a-z\.]{2,6})$/ ``` usually at the beginning there is a ** ? ** to tell the code that this part of the regex should appear once or not at all but for this email you need both parts of the regex. there is also a ** + ** at the end to signal the regex  this part meets the requirement atleast one or more times.
### OR Operator
This REGEX does not have an OR operator but like in a javascript function you can use the ``` | ```character in your REGEX to add conditions to your REGEX to look for one thing or another based on what you have put in on each side of the operator.
### Character Classes
Character classes are the brackets of characters strings, numbers, etc, that you you put in ``` [] ``` to tell your REGEX what to look for in this regex there is ``` [\da-z\.-] ``` and  ``` [a-z\.] ``` there is also a ``` . ``` character which is used to catch all characters not classified but this REGEX does not use it like that instead it uses it in a literal sense to tell the REGEX you need the ``` . ``` for the email string to work. this is used to identify wether what is inside the bracket is meant to be searched for or excluded.
### Flags
flags are characters you can put into your REGEX to add certain search cases. usually you add a flag if you want to include or exclude a whole character or symbol or if you want to search for something a certain way you add a flag to help narrow your search. this REGEX does not have any flags as it is looking for straightforward answer specified by the regex.
### Grouping and Capturing
Grouping is important because it is how you tell your code where and what it should be looking for.  capturing allows you to add a number to a group of REGEX and assign a number to it this number can be used to reference the group that you have identified with that number.
### Bracket Expressions
Bracket expressions are the brackets which create the grouping these hode the code inside and helps seperate your groups if you have multiple strings you are looking for or are trying to put together. in this email REGEX there are two sets of characters that they are looking for. these character sets are seperated and identified by the ``` [] ``` that surround each one.
### Greedy and Lazy Match
Greedy matches are when you put an operator in your code to make sure that the information is as exact and matches what you are looking for it looks for the response to match everything or it wil not accept it.
Lazy matches do the opposite and instead they look for the minimal amount of information usually looking for the least exact amount of code in the REGEX this one is not as strict as a greedy match.
### Boundaries
boundaries are like anchors except they have their own rules. the most commmon way to use a boundary is by using it after a character with a ``` /b ``` you would use this if you were trying to add a space or some other not common character.
### Back-references
a back reference is a type of REGEX that you can add to repeat a previously declared expression. you can add a word or phrase you had previously refrenced add it to a capturing groupe and then reuse that same group with a REGEX like ``` \k<char> ```
### Look-ahead and Look-behind
look aheads are useful as they can be used to look for stuff in a file specifically without taking in extra information. if you are looking for a letter like D and you are trying to find all the instances of D that also have a A after it but you dont want the A only the data for the D then you can do something like ``` D(?=A) ```. 
look-behind also works this way but rather then searching for things ahead of the document you can use it to look at the code or file starting from the end. 
you can use these commands to help find and edit all instances of something that all starts with the same letters.
## Author
Find me and my other work on GitHub at https://github.com/efargas56 or send me an email at efargas56@gmail.com