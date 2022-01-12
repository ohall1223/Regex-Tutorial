# Title Regex Tutorial

Regular expressions are patterns used to match character combinations in strings. In JavaScript regular expressions are also objects.Regular expressions are blocks of code that can be used in various computing applications. One example of regular expressions is for URL's as it can be used to create and check that a URL is unique and properly created. In the following gist we will analyze a regular expression used in javascript and the components that make the block of code.

## Summary

In this tutorial we will look at URL regex's used in JavaScript and in modern computing. We will study how the regular expression works, and the different parts that make it function properly.

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

Anchors allow the user to describe or find a term based on locations. For example, finding certain words that are the first or last on a line. Some examples of anchors are:

^-Matches at the start of the string the regex pattern is applied to.
$- Matches to the end of the string the regex pattern is applied to.
\`- Matches at the start of the match attempt.
\'-Matches at the end of the string the regex pattern is applied to.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. Some examples of quantifiers are:

x{n} - where n is a positive integer, matches exactly "n" occurences of the preceeding item "x".
x\* - Matches the preceeding item "x" 0 or more times.
x+ - Matches the preceeding item "x" 1 or more times.
x? - Matches the preceding item "x" 0 or 1 times.

### Grouping Constructs

Grouping constructs delineate the subexpressions of a regular expression and capture the substrings of an input string. You can use grouping constructs to do the following:

Match a subexpression that us repeated in the input string.

Apply a quantifier to a subexpression that has multiple regular expression language elements.

Include a subexpression in hte string that us returned by the Regex.Replace and Match.Result methods.

Retrieve individual subexpressions from the Match.Groups property and process them seperately from the matched text as a whole.

### Bracket Expressions

A bracket expression is a regular expression that shall match a speific set of single characters, and may match a specific set of multi-character collating elements based on the non-empty set of list expressions contained in the bracket expression. Brackets indicate a set of characters to match. Any individual character between the brackets will match. For example:

'elephant'.match(/[abcd]/) -> matches 'a'

### Character Classes

With a character class you can tell the regex engine to match only one out of several characters. Simply place the characters you want to match between square brackets. If you want to match an a or e use [ae] you could use this in gr[ae]y to match either gray or grey.

### The OR Operator

When building an operator that uses logic, more than likely one will run into logics based on the concept of or. In JavaScript using or can tell the operator to perform one function or the other or some other operation based on the condition. The most common expression for the "or" operator is ||. In factm one can add as many choices as long as they utilize the | expression. For example:

"I like (dogs|penguins) but not (lions|tigers).

The above results can match any of the folowing: I like dogs but not lions. I like dogs but not tigers. I like penguins but not lions. I like penguins but not tigers.

### Flags

Flags, in a regular expression, are tokens that modify its behavior or searching. Basically, flags are a form of optional parameters that users can use in addition to plain expression to make it search in a different way. Each flag is denoted by a single alphabetic character, and serves different purposes in modifying the expression's searching behavior. For example:

The flag 'i' ignores casing, which ignores any case-sensitive /hello/i ==> ignores all case-sensitivity.

The flag 'g' stands for global, it makes the expression look for all its matches instead of stopping at the first one. For example the string "cats love cats" /cats/ only matches the first "cats" /cats/g matches all "cats".

### Character Escapes

In JavaScript and computation in general, an escape character is a character that invokes an alternative interpretation on the following characters in a character sequence. What this means is a character that is attached to the following sequence of characters, the sequence can be seen in a different way. An escape character is a particulat case of metacharacters. Generally the judgement of whether something is an escape character or not depends on the context of the code that follows it.

In regex, the "" character is the expression that denotes a specific character is a escaped character. For example:

\d => matches any digit, \D => matches any non-digit, \f => matches a form feed.

## Author

Author: Olivia Hall

Github Account: [ohall1223](https://github.com/ohall1223)
