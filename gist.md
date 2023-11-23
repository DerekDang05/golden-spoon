# Regex (Regular Expression) Tutorial

To put it simply, Regex, otherwise known as a regular expression, is a sequence of characters that look like a bunch of random letters and symbols. This sequence of what appears to be gibberish, is actually being used to define a specific search pattern. They can be used to find certain patterns of characters in a text, which is why they are used. No matter how big the file is, it is able to find for example, all phone numbers, in a matter of milliseconds hence, increasing efficiency, and creating a more streamlined code.

## Summary

In this tutorial, I will be explaining a Regex that is used to find emails. <br>
<code>/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/</code>

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
There are two anchors being used in this regex. <code>^</code> amd <code>$</code>. The <code>^</code> essentially is indicating where the string is starting and the <code?$</code> is indicating where the string ends.
### Quantifiers
There are two quantifiers in this regex. <code>+</code> and <code>{2,6}</code>. The <code>+</code> is connecting the email name, for example(DerekDang), the email service (@gmail), and the .com together. The <code>{2,6}</code> is specifying a certain range, that is matching between 2 and 6 occurences of the preceding element.
### OR Operator
N/A
### Character Classes
The email sequence regex uses many character classes. <code>d</code> is being used to match any digit (0-9). <code>[a-z]</code> is being used to match any lowercase letters. The first block or section in the sequence <code>[a-z0-9_\.-]</code> is being used to represent a set of characters including lowercase letters, numbers, underscores, dots, or hyphens. After that, the <code>[\da-z\.-]</code> is being used to represent a set of numbers, lowercase letters, dots, or hyphens. After that, the <code>[a-z\.]</code> is used to represent a set of characters that include just lowercase letters and dots.
### Flags
N/A
### Grouping and Capturing
In Character Classes, those blocks or sections that I was referring to are actually called Groups. For example, in this specific regex, group #1 would be <code>([a-z0-9_\.-]+)</code> which is capturing a username. Group #2 would be <code>([\da-z\.-]+)</code> which is capturing the email provider/domain. That would make <code>([a-z\.]{2,6})</code> group #3, which is capturing the .com.
### Bracket Expressions
Bracket expressions, similarly like the group are, like the name says, everything in the bracket. For example, the bracket expression <code>[a-z0-9_\.-]</code> is mathcing any lowercase letter, number, underscore, dot or hypen. The bracket expression <code>[\da-z\.-]</code> is matching any lowercase letter, number dot or hypen. The bracket expression <code>[a-z\.]</code> is matching any lowercase letter or dot.
### Greedy and Lazy Match
This specific regex only utilizes the greedy match. This is because of the <code>+</code> and <code>{}</code> quantifiers. The <code>+</code> is greedy because it tries to match as much as possible. The <code>{2,6}</code> is greedy because it will try to match the max number of characters in the 2,6 range.
### Boundaries
The anchors that were shown in the first regex componenet, are serving as boundaries for this regex because they are basically creating the start and end point.
### Back-references
N/A
### Look-ahead and Look-behind
N/A
## Author
Derek Dang: 
https://github.com/DerekDang05
