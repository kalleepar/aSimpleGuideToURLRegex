# A Simple Guide to URL Regex

Introductory paragraph (replace this with your text)

## Summary

The regular expression uses sequences to define search patterns. Today I will be reviewing regular expressions (or regex) for finding a URL. With this, the regex will search for a URL in pages text.

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
```

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

Anchors match the starting and ending points of thr string.

`^`     is used at the beginning of the string to position anchor.      
`$`     is used at the end of the string to position anchor.

### Quantifiers

Quantifiers specify how many of a character or character class should be matched.

`+`  matches one or more occurences of the preceding character.
`*`  matches zero or more occurences of the preceding character.
`?`  matches zero or one occurence of thr preceding character.

URL EXAMPLE: `(https?:\/\/)?`

### OR Operator

`[]` matches anything included in brackets.

URL EXAMPLE: `[\da-z\.-]`

### Character Classes

Character classes allow you to describe specfic sets of characters that can be used in a search pattern.

`\w`  looks for any alphanumeric character.
`\d`  looks for any digit.

URL EXAMPLE: `[\/\w \.-]`

### Flags

Flags allow you to change how the regex behaves. (making it case sensetive, allowing matches on multiple lines.)

### Grouping and Capturing

`()`  is used to organize and create seperate groups. within each of the groups there is a regex that can be evaluated seperately.

URL EXAMPLE: `([\/\w \.-]*)`

### Bracket Expressions

`[]`  matches any character within brackets to form a string.

### Greedy and Lazy Match

`+`  Greedy allows as many matches as possible.

URL EXAMPLE: `([\da-z\.-]+)`

### Boundaries

`\b`  asserts the engines current position in the string.

### Back-references

Back-references are used to match the same text as previously matched by a capturing group.

### Look-ahead and Look-behind

zero-length assertions?

## Author

Kal Parker
[text](https://github.com/kalleepar)

