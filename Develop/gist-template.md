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

`/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

`(https?:\/\/)`
- `^` defined as an anchor
- `https?` must begin with either http or https // can be defined as either or because of the '?'
- `:` followed by forward slashes

`([\da-z\.-]+)\.`
- domain
- anything inside the parentheses must be followed by a period or dot

`([a-z\.]{2,6})`
- type of URL
- expression happens at least twice but a maximum of six times

`([\/\w \.-]*)`
- looking for ending URL of search like '.com' or '.org', etc.

`\/?$/`
- end of an expression denoted by the anchor $

### Anchors

Regex Anchors match a position before, after, or between characters and match a certain position.

Using the example above, we can see the anchors defined in the beginning and end. See highlighted portion for the anchors.
Caret anchors(`^`) are positioned in the beginning of a string.
Dollar anchors(`$`) are positioned at the end of a string. 

### Quantifiers

Regex quantifiers tell the engine to match qualities of characters in a string to its left position. The below characters are examples and they will match dependent on when called. Quantifiers usually include either the minimum or maximum number of characters the engine is looking for.

`+` = once or more;
`*` = zero times or more;
`?` = zero times or once;
`{x, y}` = x times at least, y times at most; 
The HTTP will be called on zero or once.

### OR Operator

OR operator is defined by the character (`|`) to require multiple results in the case the string doesn't meet the requirements of a pattern so it can look for an alphabetic pattern or special characters or numerials.

### Character Classes

Character classes help distinguish between alphabetic and numeric variables. These classes can be defined by square brackets or even just a backdash.
"`\d`" matches a single digit or character from 0 to 9. (digit)
"`\w`" stands for word character which matches ASCII characters. (word)

### Flags

A flag is an optional parameter that can modify the behavior of the search. Instead of the default search of a string and its characters, flags will allow the search to be different defined by a single lowercase character.

There are 6 flags to be aware of:
`i` = ignore casing;
`g` = global;
`s` = Dot All;
`m` = multiline;
`y` = sticky;
`u`= unicode;

Our example does not include any flags!

### Grouping and Capturing

Grouping has a self-explanatory purpose which is to unify a pattern so its matched as a complete block. We can group patterns by using parentheses and if there is a specific sequence we want to capture, we can use '()+' to capture one or more times. 

In our example, we can see that there are 4 examples of this grouping.
`(https?:\/\/)` = capture URL;
`([\da-z\.-]+)` = domain;
`([a-z\.]{2,6})` = top level domain;
`([\/\w \.-]*)` = endpoints;

### Bracket Expressions

Bracket expressions in Regex basically indicate a set of characters that we want to match to. The content within each bracket is usually defined by the alphabet or numerals. Don't forget that the content within each bracket is case sensitive!

`[\da-z\.-]` = accepts any digits and letters a-z, dash, or dash;
`[a-z\.]` = same as above without the digits and only dot;
`[\/\w \.-]` = accepts the slash, dot, dash

### Greedy and Lazy Match

Greedy: type of algorithm that will try to match the longest possible string or group as many variables as possible
Lazy: opposite of greedy and will try to repeat itself as minimally as possible usually enabled by "?". Will usually match the smallest group.

### Boundaries

Boundaries are used when searching or trying to match whole words. This is usually characterized by "\b" or "\B" for the inverse. In our example, boundaries are not used in URL regex, but good to know for other examples.

### Back-references

Whenever a capturing group is matched, they become storing matches in memory. Backreferencing is referencing a captured or stored match that is saved in memory by a capturing group. Please refer to the Grouping and Capturing to learn more!

Our example does not include any backreferencing!

### Look-ahead and Look-behind

Look ahead and lookbehind which are both collectively known as lookaround are no length assertions that match characters in a string but only return a result of whether there is a match or not. It is an assertion so there are designed to just assert a match or not.

Our example does not include lookaround.

## Author

This Regex tutorial was created by Jonathan Lee. Cheers!

Profile: https://github.com/jonathan-lee8
