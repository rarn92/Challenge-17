# Regex Tutorial

gist url: https://gist.github.com/rarn92/39239feef06f65964e4b93bce33dbe0f

# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

A regex, or regular expression, is a sequence of characters that defines a search pattern. Regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string.

For example, the following regular expression can be used to verify that user input is a valid email address:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

The components of a regex expression are comprised of different elements that define the syntax we will use when creating regular expressions. They are characters that allow us to match values in different ways and specify what we want our expression to accomplish.

### Anchors

`$  `	Matches any string where the specified value occurs at the end of the string.  
`^  `	Matches any string where the specified value occurs at the beginning of the string.  

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

`*?`	Matches zero or more times.  
`+?`	Matches one or more times.  
`?	??`	Matches zero or one time.  
`{ n }	{ n }?`	Matches exactly n times.  
`{ n ,}	{ n ,}?`	Matches at least n times.  
`{ n , m }	{ n , m }?`	Matches from n to m times.  

### OR Operator

`|   `	Represents an OR operator.  

### Character Classes

`.  `	Matches any single character  
`\  ` Lets special characters be used. The following need to be preceded by a backslash: `\   .   $   *   ?   +  [ ]   (   )   |  `  
`[]`	Matches any single character in the range or set enclosed in the brackets.  

### Flags

Regular expressions have optional flags that allow for functionality like global searching and case-insensitive searching. These flags can be used separately or together in any order, and are included as part of the regular expression.

* d - Substring matches
+ g	- Global search
+ i	- Case-insensitive search
+ m	- Multi-line search
+ s	- Allows . to match newline characters
+ u	- unicode
+ y	- Sticky search that matches position

### Grouping and Capturing

* Grouping: You can use brackets or parentheses to group part of the expression together. This allows you to apply elements to specified parts of the expression.  
+ Capturing: If you use parentheses to group part of an expression it will also create a captured group. A captured group is a stored value that matched the quantifier inside the parenthesis.

### Bracket Expressions

Bracket expressions can be used to match a single character.

### Greedy and Lazy Match

* Greedy match will continue to search until the entire defined quantifer is searched. It is greedy in that it will continue to match through the entire defined contraints.
+ Lazy match will only go until it comes across the first matching instance and then stop.

### Boundaries

* Similar to anchors, boundaries define what we want to be matched within our expression. The main difference is that boundaries are used to only match to the left and right of the current position.

### Back-references

* Back references are simply a reference to a previously matched grouped value. You could say it references back to the previously matched data.

### Look-ahead and Look-behind

* These are both components of the 'lookaround' assertion. They are similar to booleans in that they only care if a match is made and will return either match (true) or no match (false) rather than the values matched.

## Author
Robo - I am a full-stack developer who is always striving to be the best. Please check out my github @ user rarn92
