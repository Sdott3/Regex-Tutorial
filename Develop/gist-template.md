# Regex for a matching Url

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

 ^ – The caret anchor matches the beginning of the text.
 $ – The dollar anchor matches the end of the text.

Anchors assert that the engine's current position in the string matches a location. This is useful because, it is expressive: it lets you specify that you want to match digits at the end of a line, but not anywhere else. When you tell the engine that you want to find a pattern at a given location, it doesn't have to spend time trying to find that pattern at many other locations.

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
