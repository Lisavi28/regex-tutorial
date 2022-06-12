# Title: Regex matching an email

This tutorial explains the use of the regular expression for email validations in text searches.

## Summary

The formal language that helps to express the sequence of characters in specific search patterns in an email is the regular expression or Regex, it allows us to validate the registration or login process.

An email is composed of the following elements

1. `username` is the username
2. `@`
3. `email`is the email hostname
4. `.`
5. `com` is the Domain

(`username@email.com`)

so when you want to validate user input in an email you use

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})\$/`

We will explain the meaning of this chain in the tutorial.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

Anchors help you match a position before or after characters.
`^` : The caret is used to indicate that character next to it must be at the beginning of the text.
`$` : The dollar anchor is used to indicate that character next to it must be at the end of the text.

If we check the validation regular expression at its beginning and end.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})\$/`

we will see that it complies with `^`(caret) and `$` (dollar) anchors.

### Quantifiers

Quantifiers signal that the preceding token must match a certain number of times.

In the email validation regular expression, the quantifiers include the `+` operator, which will match a character as many times as neededIn other words, the characters may be repeated, but we don't specify the limit. Another quantifier for this regular expression includes `{2,6}`, which will allow a matching range of 2 to 6 characters for the character set `[a-z\.]`.

### Character Classes

The character class in this expression is `\d`, which matches a single characters that is a digit from 0-9.

### Grouping and Capturing

Grouping allows us to combine a set of logic to work to together.
In email validation we have three capture groups. 1. username: `([a-z0-9_\.-]+)` 2. email hostname: `([\da-z\.-]+)` 3. domain: `([a-z\.]{2,6})`

### Bracket Expressions

Bracket expressions allow any value inside the brackets `[]` to be present in the search term.
For example: `[a-z0-9_\.-]` will match a single digit from 0-9, any character a-z (case senstive), or the characters "." and "-".

## Author

Yazmín Sánchez feel free to contact me by email lisavi_28@yahoo.com.mx or https://github.com/Lisavi28
