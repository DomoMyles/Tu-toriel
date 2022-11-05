# Title (replace with your title)

Regex Tutorial for an Email.

## Summary

This tutorial will thuroughly explain wwhat a regex code is and how it matches up with an email adress

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
([a-zA-Z0-9_.-]+) This section of code will check each character from a - z uppercase and lowercase including numbers and the special characters of `_`, `.` and `/`. The plus sign on the end indicates that it can be of any length of character from one to an 'inifnity'. This part of the code in our example will specifically be for the body of the email. 

@([\da-zA-Z.-]+) This section of code is similar to the first one but does not include numbers. This one has the @ symbol at the start indicating that it will look for a domain name for an email and check wether or not the email is a valid name.

([a-zA-Z.]{2,})

### Anchors

### Quantifiers
`/^([a-zA-Z0-9_.-]+)@([\da-zA-Z.-]+).([a-zA-Z.]{2,9})$/`
The quantifiers in this example include where the `+` and where the `{2.6}` are. They tell the amount of characters that the regex must match. The `+` will indicate the number of characters that the string will match. There are other quantifiers, such as a `?` which will match 0 or one characters, while a `*` will match 0 or more characters. The `{2,9}` in our example will match a character that is atleast '2' but no more that '9' characters long. 
The quantifiers will usually be placed after the end of the brackets that defign what it will be looking for for example:
`([a-zA-Z.]{2,9})` 
This will look for any lowercase or uppercase letters expression but must be between 2 and 9 characters long.

### OR Operator
An Or operation is as simple as a boolean operationn in the way that it can match the expression befor or after the `|`. This can be used within a single group and/or used in the entire sequence.
### Character Classes
`[\da-zA-Z.-]`
Character classes are used to define a single character or digit, they are used within a group befor the expressions are defined as shown above.
`\d` Will match one digit filliwing
`\s` Will match a blank space such as a space or a tab
`\w` will match a single alpganumeric character or underscore. 

### Flags

### Grouping and Capturing

### Bracket Expressions
`[a-zA-Z0-9_.-]` 
The Bracket Expressions will define which characters will be defined, anything within these bracked the sequence will look for try to match.
### Greedy and Lazy Match

### Boundaries
`@([\da-zA-Z.-]+)`
The Boundaries are not typically used for emails because the `@` symbol acts as its own boundary between the email body and the email domain.

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
