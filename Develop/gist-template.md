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

| This element is used to separeted groups. If the character on the left side is matched, then the right side's character is ignored. \ It is used to escape a special character after this sign in a string. ( ) Captures values in the group using parentheses. [ ] Matches anything within the brackets. [0-9] Matches any number values between 0 and 9. [0 9] Matches only zero or 9, or any other number that you put inside.

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

My name is Mohamed but I prefer being called by my nickname Mo Mo. I am a software engineering student currently enrolled in the University of Minnesota coding bootcamp. 

GITHUB LINK: https://github.com/mmohamed12452
