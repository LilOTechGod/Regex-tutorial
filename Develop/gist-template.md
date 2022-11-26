# Matching a URL regex breakdown

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

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

A regex is considered a literal, so the pattern must be wrapped in a slash characters (/). By examining the "Matching a URL" regex, you'll see that this is true:

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

#### Now let's take a look at the components of a regex.

### Anchors

The characters ^ and $ after and before regex components(/) are both considered to be anchors.

The ^ anchor signifies a string that begins with the characters that follow it. This could be in one of two formats but, in this case:

* An exact string match, such as "(htpps?: \/\/)"

The $ anchor signifies a string that ends with the characters that precede it.

* Just as with the ^ character, in this case it's preceded by an exact string match.

### Quantifiers

Quantifiers are limitations to the string that your regex matches(or an individual section of the string). Almost always include the minimum and maximum number of characters that your regex is looking for.

There are two types of Quantifiers, greedy and lazy. Each type has the same description.

* * Matches the pattern zero or more times.
* + Matches the pattern one or more times.
* ? Matches the pattern zero or one time.
* {} Curly brackets can provide three different ways to set limits for a match:

1. { n } Matches the pattern exactly n number of times.
2. { n, } Matches the pattern at least n number of times.
3. { n, m } Matches the pattern from a minimum of n number of times to a maximum of x number of times.

By examining the "Matching a URL" regex, you'll see that this is true:

* https?          Because of the "?" Matches the pattern one time.
* [\da-z\.-]+     Because of the "+" The pattern matches the following components one or more times (\d) matches a single digit, group of letters (a-z), dot (.) or hyphen (-).
* [a-z\.]{2,6}    Because of the "{2,6}" it matches 2 to 6 copies of the sequence ([a-z\.].
* [\/\w \.-]*)    Because of the "*" the pattern matches '/', '.', '-', 'www', '//'.

### Grouping Constructs

Grouping expressions allows us to keep things more organized and easier to determine that different sections fulfill different requirements. To break these sections up, you'll need to use grouping constructs which uses parentheses "()".



### Bracket Expressions

### Character Classes

Charcater classes ensure that a given sequence of characters matches a large set of characters.

* [a-z]       Matches lowercase alphabetic characters between a and z.
* \w          Matches a single word.
* \d          Matches a single character that is a digit 0-9.
* .           Matches any character.

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
