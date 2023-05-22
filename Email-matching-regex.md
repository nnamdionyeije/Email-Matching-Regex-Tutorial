# Email Matching Regex Tutorial

Introductory paragraph (replace this with your text)

This tutorial serves to explain how a email matching regular expression works.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

I will be explaining the regular expression: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This regex is used to validate email addresses.

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

### Anchors

The regex includes the anchors '^' and '\$' The ^ anchor signifies that the string must begin with the characters that follow it (which constitute the username), and the \$ signifies that the string must end with the characters which precede it (which constitute the extension).

### Quantifiers

The quantifier, '{2,6}' is used to make sure the preceding string has between 2 and 6 characters to match how email extentions work.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
