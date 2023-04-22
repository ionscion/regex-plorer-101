# Regex Email Verification 

## Summary

We will be explaining the regex used to verify an email address. This regex is valuable because it can be used to verify that an email address is valid before sending an email to it. This is important because it can prevent the user from entering an invalid email address and having the email bounce back.

The regex we will be studying here is:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

These are the characters `^` and `$`. They are used to match the beginning and end of a string. In this case, we are using them to match the beginning and end of the email address.

- The `^` character is used to match the beginning of the string. This means that the regex will only match if the email address begins with the characters that follow the `^` character.
- The `$` character is used to match the end of the string. This means that the regex will only match if the email address ends with the characters that precede the `$` character.
- The `^` and `$` characters are used together to match the entire string. This means that the regex will only match if the email address is exactly the same as the characters that follow the `^` character and precede the `$` character.

### Quantifiers
Quantifiers are used to match a certain number of characters.

In our regex, these are the characters `+` and `{}`. They are used to match a certain number of characters.
- The `+` character is used to match one or more of the preceding character. In this case, we are using it to match one or more of the characters `a-z`, `0-9`, `_`, `.`, and `-`.
- The `{}` character is used to match a specific number of the preceding character. In this case, we are using it to match two or six of the characters `a-z` and `.`.

### Grouping Constructs
Grouping constructs are used to group characters together that match a specific pattern specified by the regex author. 

There are 3 grouping constructs present in this regex:
- `()` is used to group characters together that match a specific pattern specified by the regex author. In this case, we are using it to group the characters that match the bracket expression `[a-z0-9_\.-]+`.
- `()` is used to group characters together that match a specific pattern specified by the regex author. In this case, we are using it to group the characters that match the bracket expression `[\da-z\.-]+`.
- `()` is used to group characters together that match a specific pattern specified by the regex author. In this case, we are using it to group the characters that match the bracket expression `[a-z\.]{2,6}`.

### Bracket Expressions
Bracket expressions are used to group characters together that match a specific pattern specified by the regex author. 

There are 3 brackets expressions present in this regex:
- `[a-z0-9_\.-]` is used to match one or more of the characters `a-z`, `0-9`, `_`, `.`, and `-`. This is used to match the local part of the email address.
- `[\da-z\.-]` is used to match one or more of the characters `a-z`, `0-9`, and `-`. This is used to match the domain name of the email address.
- `[a-z\.]` is used to match two or six of the characters `a-z` and `.`. This is used to match the top-level domain of the email address.

### Character Classes
There are 5 character classes present in this regex:

- `\d` is used to match any digit character. This is used to match the digits in the domain name of the email address.
- `a-z` is used to match any lowercase letter character. This is used to match the lowercase letters in the local part and domain name of the email address (i.e. it is making sure that the email address is all lowercase).
- `0-9` is used to match any digit character. This is used to match the digits in the local part of the email address if any are present.
- `_` is used to match the underscore character. This is used to match the underscore character in the local part of the email address.
- `-` is used to match the hyphen character. This is used to match the hyphen character in the local part and domain name of the email address.
- `.` is used to match the period character. This is used to match the period character in the local part and domain name of the email address.

### The OR Operator
There is not an explicitly defined OR operator in this regex. 

### Flags
There are no flags present in this regex.

### Character Escapes
In a regex, a character escape is used to match a designated character for that specific regex use case.

There are 3 character escapes present in this regex:
- `\.` is used to match the period character in the submission. This is used to match the period character in the domain name of the email address.
- `\d` is used to match any digit character in the submission. This is used to match the digits in the domain name of the email address.
- `\-` is used to match the hyphen character in the submission. This is used to match the hyphen character in the domain name of the email address.

## Author

This tutorial was written by Ben Sboto. You can find me on GitHub at [ionscion](https://github.com/ionscion).
