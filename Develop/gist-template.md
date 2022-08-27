# Regex for matching a URL

Regular expressions (regex for short) are special text strings that are used for searching text. This tutorial explains regex used for a matching URL.

## Summary

The following regular expression can be used to verify that user input is a valid for matching a URL: /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

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
Anchors do not match any character. They match a position before or after characters.

* ^ – The caret anchor matches the beginning of the text.
* $ – The dollar anchor matches the end of the text.

Anchors assert that the engine's current position in the string matches a location. This is useful because, it is expressive: it lets you specify that you want to match digits at the end of a line, but not anywhere else. When you tell the engine that you want to find a pattern at a given location, it doesn't have to spend time trying to find that pattern at many other locations.

### Quantifiers
Quantifiers specify how many times a character, group, or character class must be present in the input for a match to be found.
    * * and *? Matches Zero or more times.
    * + and +? Matches One or more times.
    * ? and ?? Matches Zero or One times.
    * {n} and {n}? Matches exactly n times.
    * {n,} and {n,}? Matches atleast n times.
    * {n,m} and {n,m}? Matches from n to m times.

Example for matching URL:
    * https?          Matches 'https', 'http'
    * [\da-z\.-]+     Matches a single digit, group of letters (a-z), dot (.) or hyphen (-) 1 or more times
    * [a-z\.]{2,6}    Matches 2 to 6 copies of the sequence * [a-z\.]
    * [\/\w \.-]*     Matches '/', '.', '-', 'www', '//'

### OR Operator

### Character Classes
A character class, also called “character set”, defines a set of characters. You can tell the regex engine to match only one out of several characters. It ensures that a given sequence of characters matches a Larger set of characters. 

    [a-z]          Matches lowercase alphabetic characters between a and z
    \w             Matches a word
    \d             Matches a single character that is a digit
    .              Matches any character
### Flags

### Grouping and Capturing
Grouping Constructs are used check multiple parts or sections of a string for different requirements. By using parentheses (()) around different sections of the regex.


*    (https?:\/\/)       Matches: ' ', 'https://', 'http://'
*   ([\da-z\.-]+)       Matches: 'ab.c-7', 'ab'
*   ([a-z\.]{2,6})      Matches: 'ab.', '.ca'
*   ([\/\w \.-]*)       Matches: '/', '/ab.'

### Bracket Expressions
A bracket expression (an expression enclosed in square brackets, "[]" ). 

Bracket Expression examples:
* [\da-z\.-]
* [a-z\.]
* [\/\w \.-]

### Greedy and Lazy Match
Greedy means match longest possible string.

Lazy means match shortest possible string.

For example, the greedy h.+l matches 'hell' in 'hello' but the lazy h.+?l matches 'hel'.

([\da-z\.-]+)       The "+" operator is greedy as it allows character matching from one to an infinite amount of times.

### Boundaries

### Back-references
Back-references provide a way to identify a repeated character or substring within a string. 

Pattern	Description
* (?<1>a)	Match the character "a" and assign the result to the capturing group named 1.
* (?<1>\1b)*	Match zero or more occurrences of the group named 1 along with a "b", and assign the result to the capturing group named 1.

### Look-ahead and Look-behind

## Author

Shatyana Thomas a current student at UofM's Full-Stack Coding BootCamp. https://github.com/sdott3 