# Interrubble's Regex Tutorial

Hello! Today I will be going over a Regular Expression (REGEX) e-mail matching example. There are a few other expressions that are used, but this tutorial will focus just on an e-mail expression.

## Summary


The e-mail expression I will be describing will be based on the 'flavors' or languages of .NET, Java, JavaScript, PCRE, Perl, and Python. The code snippet I will be using, <code>^[A-Z0-9+_.-]+@[A-Z0-9.-]+$</code>, has the constraints of being case sensitive and restrictions on characters allowed.


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

The anchors in this particular expression are <code>^</code> (which indicates the start of the expression/string) and <code>$</code> (which indicates the end point).

### Quantifiers

The quantifiers in this REGEX is the <code>+</code> operator, connecting the users email name, service, and '.com'.

### Grouping Constructs

In this REGEX are two capturing groups. The first one, <code>[A-Z0-9+_.-]</code>, is used to match the user email name. The second one, <code>[A-Z0-9.-]</code>, is used to match the domain of the email being used.

### Bracket Expressions

When it comes to validation for e-mail, there is the bracket expression <code>[A-Z0-9+_.-]</code> (the aforementioned first part), which sets the parameters of using any character set that contains any letter a-z, which is case sensitive, and matching any number 0-9, while also including the special characters "+", "_", ".", "-". The second part of validation, again pulling from above, but this time using the following bracket expression <code>[A-Z0-9.-]</code>. This expression matches for any character set that contains letter a-z, also case sensitive, any number 0-9, and only two special characters, ".", and "-". 

### Character Classes

This particular REGEX does not seem to include a character class. However, a character class that can be used is <code>\w</code>, which is a word character. A word character is a letter, number, or an underscore. It may be represented by the regex <code>[a-zA-Z0-9_]</code>. It looks similar to our bracket expressions, but does not match. 

### The OR Operator

This particular REGEX does not have an OR Operator. An example of an OR Operator is a 'pipe', or a <code>|</code>.

### Flags

Flags are characters outside of the REGEX, at the end, that can do a number of things. This particular REGEX does not have a flag, but an example of a flag is <code>m</code>, which checks for a multi-line match.

### Character Escapes

Escape characters, which are case sensitive, are characters preceded by a <code> \ </code>, sometimes with a letter after.

## Author

The author is Chris DeLaGarza. You can reach me at delagarzachris@icloud.com and check out my repos at www.github.com/Interrubble.
