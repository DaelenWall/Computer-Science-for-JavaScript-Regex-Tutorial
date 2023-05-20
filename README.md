# Computer-Science-for-JavaScript-Regex-Tutorial
A brief, but detailed introduction to Regex.

## Summary
Here's a JavaScript regular expression (regex) pattern that matches the email "johndoe_1@example.com": `/^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/`

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
* `^` - The caret symbol denotes the start of the string. This ensures that the email begins with the pattern specified next.

* `$` - The dollar sign represents the end of the string. It ensures that the email address ends after the TLD.

### Quantifiers
* `+` (plus sign): Matches one or more occurrences of the preceding element. In this regex, it applies to `[a-zA-Z0-9._-]`, `[a-zA-Z0-9.-]`, and `[a-zA-Z]{2,}`. It allows for one or more alphanumeric characters, periods, underscores, or hyphens in the local part of the email, one or more alphanumeric characters, periods, or hyphens in the domain name, and at least two alphabetic characters in the TLD.

### Grouping Constructs
* `()` (parentheses): Groups multiple elements together. In this regex, parentheses are not used for capturing groups; instead, they are used to group parts of the regex for applying quantifiers and operators.

### Bracket Expressions
* `[a-zA-Z0-9._-]`: Matches a single character that is either an uppercase letter (`A-Z`), lowercase letter (`a-z`), digit (`0-9`), period (`.`), underscore (`_`), or hyphen (`-`). It allows these characters in the local part of the email.
* `[a-zA-Z0-9.-]`: Matches a single character that is either an uppercase letter (`A-Z`), lowercase letter (`a-z`), digit (`0-9`), period (`.`), or hyphen (`-`). It allows these characters in the domain name.
* `[a-zA-Z]`: Matches a single alphabetic character. It ensures that the TLD consists of at least two letters.

### Character Classes
* `\.` (escaped period): Matches a literal period. It is used to match the dot in the domain name.

### The OR Operator
* `|` (pipe symbol): Matches either the expression on the left or the expression on the right. It is not used in this regex.

### Flags
* Flags modify the behavior of the regex pattern, such as case-insensitive matching (`i` flag), global matching (`g` flag), or multiline matching (`m` flag). Like the OR Operator, no flags are specified in this regex.

### Character Escapes
* Again, none are used in this regex. However, if any metacharacters (characters with special meaning in regex) needed to be matched as literal characters, they would need to be escaped with a backslash (`\`).

## Author
Made by Daelen Wall, a student at UCONN and a lover of life.

Github: https://github.com/DaelenWall