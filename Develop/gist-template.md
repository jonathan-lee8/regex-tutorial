# A Simple, Easy Regex Tutorial

For those getting into programming or even for those who want to expand their computer science related knowledge, this is a Regex or 'Regular Expression' tutorial created to help anyone understand the sequence of Regex. What is Regex? Regex is a sequence of special characters to confirm a search pattern in text, included in some kind of code or search algorithm. Regex can be used to find or find and replace opreations on strings. Regex is also commonly used for input validation.

## Summary

This tutorial is cover the components of Regex and dissect examples of code utilizing Regex. For this tutorial, we will be matching a URL as it is one of the most common things we interact with on a daily basis.

Example: /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

Please navigate through the table of contents to find specific parts the tutorial will cover. 

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

Regex Anchors match a position before, after, or between characters and match a certain position.

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

Using the example above, we can see the anchors defined in the beginning and end. See highlighted portion for the anchors.
Caret anchors(^) are positioned in the beginning of a string.
Dollar anchors($) are positioned at the end of a string. 

### Quantifiers

Regex quantifiers tell the engine to match qualities of characters in a string to its left position. The below characters are examples and they will match dependent on when called.

+ = once or more;
* = zero times or more;
? = zero times or once;
{x, y} = x times at least, y times at most; 
The HTTP will be called on zero or once.

### OR Operator

### Character Classes

Character classes help distinguish between alphabetic and numeric variables. These classes can be defined by square brackets or even just a backdash.
"\d" matches a single digit or character from 0 to 9. (digit)
"\w" stands for word character which matches ASCII characters. (word)

### Flags

### Grouping and Capturing

### Bracket Expressions

Bracket expressions in Regex basically indicate a set of characters that we want to match to. The content within each bracket is usually defined by the alphabet or numerals. Don't forget that the content within each bracket is case sensitive!

[\da-z\.-]
[a-z\.]
[\/\w \.-]

### Greedy and Lazy Match

Greedy: type of algorithm that will try to match the longest possible string or group as many variables as possible
Lazy: opposite of greedy and will try to repeat itself as minimally as possible usually enabled by "?". Will usually match the smallest group.

### Boundaries

Boundaries are used when searching or trying to match whole words. This is usually characterized by "\b" or "\B" for the inverse. In our example, boundaries are not used in URL regex, but good to know for other examples.

### Back-references

### Look-ahead and Look-behind

## Author

This Regex tutorial was created by Jonathan Lee. I was previously a financial analyst, now pursing to become a full stack developer. Please when you have a chance, check out my Github profile linked down below. Thanks for checking this out. Feel free to connect with me. Cheers!

Profile: https://github.com/jonathan-lee8
