# Regex Tutorial

A tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary
 In this tutorial I will break down a regular expression that matches hex values which are typically a # with 6 numbers or letters following it.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)


## Regex Components

A Hex value, the Regex would look similar to this  " /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ ". Heres the break down...

### Anchors

These Anchors in a regex string are the ^ and $, the ^ will represent the start of the string and the $ represents the end of the string

" ^#?([a-f0-9]{6}|[a-f0-9]{3})$ " everything in between the ^ and $ will be representing what the regex is looking for

### Quantifiers

Quantifiers will  be the *, ?, and {}. In this situation the ? is showing that the # will be followed by 0 or 1 characters

-  ?([a-f0-9]{6}|[a-f0-9]{3}) , quantifier is saying after the # it will be either 0 or 1 characters

### OR Operator

" [a-f0-9]{6}|[a-f0-9]{3} " the | in the middle is representing that it will either be 6 characters or 3
OR operator in our example: |  Its purpose: Allows the user to match either the expression/characters on the left or the right. The | is positioned in between two seperate expressions.

### Character Classes

" /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ " The character class here is a-f0-9. The character class is the set of characters that is enclosed within the brackets. The a-f symbolize the range the hex code requires, meaning the code can begin with any letter between 'a though f'. Also the hex code has 0-9 attached immediately after the f, which also allows the hex code to begin with any digit from '0 to 9'

### Grouping and Capturing

" ([a-f0-9]{6}|[a-f0-9]{3}) " The () groups the regular expression between them. The grouping treats multiple characters as a single unit. This can proof useful when extracting information using any programming language. This group of data will be exposed in the form of an array. Values can be accessed using an index on the result of the match.
The grouped expression is a bracket expression whose details are provided in the section below. Ultimately the end string anchor $ is applied to this grouping.

### Bracket Expressions

" [a-f0-9] " Bracket expression is a regex that will match a specific pattern of characters alphabetic, numeric, special characters, and symbols defined within the brackets. The bracket [] expression indicates matching a string that has any lower case character between a-f or any integer between 0-9


## Author

My name is Jessica and im currently enrolled in a full stack web development course. My goal is to become the best developer i can be for any future team i work with and making sure im constantly learning new things.

Github: [Jhlynn95](https://github.com/jhlynn95)

Email: lynnsmith951@yahoo.com
