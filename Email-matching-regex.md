# Email Matching Regex Tutorial

The purpose of this tutorial is to demonstrate understanding of regular expressions by explaining how an email matching regex works.

## Summary

The regular expression I will be describing is an email matching regex. The regex takes the form: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The regex creates a pattern in the format of "username@domain.extension" and can be used to search for any email in a text document.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

The regex includes the anchors '^' and '\$' The ^ anchor signifies that the string must begin with the characters that follow it (which constitute the username), and the \$ signifies that the string must end with the characters which precede it (which constitute the extension).

### Quantifiers

The quantifier, '{2,6}' is used to make sure the preceding string has between 2 and 6 characters to match how email extentions work. Similarly the quantifier '+' is used multiple times to indicate that what the characters that precede it match the pattern in the bracket expression one or more times.

### OR Operator

In this regex, the sections surrounded by square brackets have an implicit OR operator between the different characters used in the pattern. For example, the first section '[a-z0-9_\.-]' could alternatively be written as '[a-z|0-9|_|\.-].

### Character Classes

This regex uses the character class /d which is equivalent to the bracket expression [0-9]. It matches up to any arabic numeral digit.

### Grouping and Capturing

This regex uses multiple grouping constructs to split the expression into multiple subexpressions. Parenthesis are used to create subexpressions for the username '([a-z0-9_\.-]+)', domain '([\da-z\.-]+)', and email extension '([a-z\.]{2,6})'.

### Bracket Expressions

This regex contains three bracket expressions for the purpose of outlining the patterns for different parts of an email address.

[a-z0-9_\.-] - specifies that the email address can have a username containing any lowercase letter, any number, as well as the special characters '\_' and '.'.

[\da-z\.-] - specifies that the domain name can only contain lowercase letters, any number, as well as the special character '.'.

[a-z\.] - specifies that the email extension can only contain lowercase letters and the special character '.'.

## Author

Nnamdi Onyeije is a student in the Georgia Tech Full Stack Web Development Coding Boot Camp. His github profile can be found at https://github.com/nnamdionyeije.
