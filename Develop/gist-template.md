# Module 17: Javascript Regular Expressions(Regex)

As a web development student, I have developed this tutorial, where you will learn about the Regex abbreviation of Regular Expression and how you can use it to identify characters in a text.

## Summary

Regex or Regular Expressions are patterns used to identify combinations or characters in a string, they can be used to validate text based on complex criteria, and they can also be used to replace patterns of the character in a string.

In this tutorial we are going to use this Email:
         /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ 
as an example of how to breakdown some Regular Expression examples and how to use it.

## Table of Contents

- [Regex Components](#regex-components)
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

Anchors have special meaning in regular expressions. They do not match any character. Instead, they match a position before or after characters:

 ^ – The caret anchor matches the beginning of the text.
 $ – The dollar anchor matches the end of the text.

### Quantifiers

Quantifiers are used to communicate how many characters are expected. Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. By default, quantifiers are greedy, and will match as many characters as possible. If the ",+,?,{}" characters are found within regular expressions, they are considered quantifiers. The ? indicates the expression to match 0 or 1 time. As mentioned in the summary above because there are 2 types of formats we'll use the or operator to distinguish which format we are using. In our Hex Value regular expression we have {6} (Hex Triplet Format) and {3} (Shorthand Hex Format), this indicates that the length of the component preceding these quantifiers should be 6 for {6} and 3 for {3}.

Quantifiers summary

The following lists the quantifiers:

Quantifier	Description
*	Match zero or more times.
+	Match one or more times.
?	Match zero or one time.
{ n }	Match exactly n times.
{ n ,}	Match at least n times.
{ n , m }	Match from n to m times.

### OR Operator

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
The "or" operator within a regular expression is defined using the | element. The or operator indicates that it could either of the components that we are separating with the |. For our hex value regular expression we have ([a-f0-9]{6}``|``[a-f0-9]{3}). Note the or operator separating these 2 components. This means that our hex value could either be 6 characters [a-f0-9]{6} or 3 characters [a-f0-9]{3}.

### Character Classes

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Character classes are components within our regular expression that tells us what type of characters to expect. In our example our character classes are confined within brackets []. For our example we have 2 character classes: [a-f0-9] and [a-f0-9] which searches for the same values. We will be breaking down what the characters are searching within these character classes. a-f searches for letters a-f and 0-9 searches for digits 0-9.

### Flags

Regular expressions may have flags that affect the search.

There are only 6 of them in JavaScript:

i
With this flag the search is case-insensitive: no difference between A and a (see the example below).
g
With this flag the search looks for all matches, without it – only the first match is returned.
m
Multiline mode (covered in the chapter Multiline mode of anchors ^ $, flag "m").
s
Enables “dotall” mode, that allows a dot . to match newline character \n (covered in the chapter Character classes).
u
Enables full Unicode support. The flag enables correct processing of surrogate pairs. More about that in the chapter Unicode: flag "u" and class \p{...}.
y
“Sticky” mode: searching at the exact position in the text (covered in the chapter Sticky flag "y", searching at position)

### Grouping and Capturing

Regular expressions can be grouped by placing them inside parentheses () to apply quantifiers or restrict alternation to that part of the regex;

For example:
/^([a-z0-9_\.-]+)@([\da-z\.-]+).([a-z\.]{2,6})$/ 
There are three groups in the regex code above.

 Group 1: [a-z0-9_\.-] is used for the username of the email account.
 Group 2: [\da-z\.-] is used to capture the domain name/email service. 
 Group 3: [a-z\.] is used to capture the domain extension.

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

My name is Mohamed but I prefer being called by my nickname Mo Mo. I am a software engineering student currently enrolled in the University of Minnesota coding bootcamp. 

GITHUB LINK: https://github.com/mmohamed12452
