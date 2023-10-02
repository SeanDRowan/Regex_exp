# matching an email regex


## Summary
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The regex described above will check a password to see if it meets all the given requirements. it is divided into three subexpressions using parethesis in order to describe the different parts of an email adress. 
([a-z0-9_\.-]+) is the first, and can include any regular character or number plus period, underscore, and hyphen. ([\da-z\.-]+) is the second, and can include everything from the first except for the underscore. /d defines a character class of all digits 0-9. ([a-z\.]{2,6}) is the third and allows characters a-z and period (but no numbers), and must be between two and six characters in length.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
the anchors are the ^ and $ symbols, ^ indicates the beginning of the regex expression $ indicates the end.
### Quantifiers
quantifiers set the limits for a string. in this example the quantifiers are {2,6} as the top and bottom limits. They indicate that the final part of the email adress should be between 2 and 6 characters in length.
### Grouping Constructs
this regex is grouped by parenthesis into three separate subexpressions. ([a-z0-9_\.-]+), ([\da-z\.-]+),and ([a-z\.]{2,6}). they are connected by the @ and an period, which should be present in every email adress.
### Bracket Expressions
bracketed characters set a range of characters to match. [a-z0-9_\.-] can include any regular character or number plus period, underscore, and hyphen. 
### Character Classes
character classes are specific classes that define a set of characters. in this example ([\da-z\.-]+) \d is a character class that defines all arabic numerals (0-9). 
### Character Escapes
\ escapes a character so that it is not interpreted literally. in the example ([\da-z\.-]+) the period has an escape so that it is not rerad as a special character.
## Author

for additional questions, please reach out to me on github SeanDRowan or by email at sdrowan93@gmail.com
