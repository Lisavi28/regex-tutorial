# Title: Regex matching an email

This tutorial explains the use of the regular expression for email validations in text searches.

## Summary

The formal language that helps to express the sequence of characters in specific search patterns in an email is the regular expression or Regex, it allows us to validate the registration or login process.

The email is composed of the following elements

1. is the username
2. @
3. email hostname
4. .
5. Domain

(`username@email.com`)

so when you want to validate user input in an email you use

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})\$/

We will go deeper into it later.

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

Anchors help you match a position before or after characters.

      `^` : The caret is used to indicate that character next to it must be at the beginning of the text.
      `$` : The dollar anchor is used to indicate that character next to it must be at the end of the text.

If we check the validation regular expression at its beginning and end.

/^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}\$/

we will see that it complies with ``^`(caret) and`\$` (dollar) anchors.

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
