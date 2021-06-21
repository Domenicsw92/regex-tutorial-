# Regex-Tutorial
Regular expressions (also known as regex) are character sequences that define search patterns. These expressions can be used to discover certain patterns of characters inside a string or to find/replace a character or characters within a string. Regex can also be used to validate input.
## Summary
Matching an Email: 
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
Using the regex shown to match an email address.
the tutorial will explain the components of the regex.
## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Conclusion](#conclusion)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
Regex expressions require a means to indicate the beginning and conclusion of the expression. In this example, the beginning of the string is denoted by:

The end of our string is denoted by the symbol $

If there are square brackets around the circumflex accent, this rule does not apply (as shown below). If this is the case, the meaning shifts to "not." [^]
### Quantifiers
Quantifiers inform the regex engine that the quantity of the character or expression to its left must be matched. Here are several examples:

    ?, +, *, {n}, {n, }, {n,m}

This regex has two quantifiers: + and. We can denote the former as i+ and understand that it corresponds to the preceding item i one or more times. The latter, written as i{n,m} indicates that it corresponds to the previous item I between n and m times, where m must be bigger than n and both n and m must be positive integers.
### Grouping Constructs
We can validate the characters in a particular group by grouping expressions. As a group, we define text between parenthesis. We have three groupings in this situation. The first is ([a-z0-9_.-]+), the second is ([\da-z.-]+), and the third is ([a-z.]2,6).
Email matching, we have three capture groups that allow us to apply different string criteria to each. ([a-z0-9_.-]+) separated by the special character @, then the second capture group ([da-z.-]+), and finally the third capture group ([a-z.]{2,6}).
### Bracket Expressions & Character Classes
Characters that can be matched are defined using bracket expressions. In this example, we'll use 
    [a-z0-9_.-] [\da-z\.-] [a-z\.]
The first, [a-z0-9_.-], implies that all characters from a to z, as well as numeric characters from 0 to 9, shall be matched.
The second, [da-z.-], looks for letters a-z as well as d, which is a digital digit match.
The third, [a-z.], - indicates that any character between a and z will be matched, as well as a dot. Character Classes


### Character Escapes
The preceding \ the dash and period "escapes" these letters, indicating that the dash and period are not regex special characters. There's no need to remove the period between the square brackets.

### Conclusion 
This tutorial dissected an email matching regex and its components. These components are divided into three primary groups that comprise our validation expressions. These capture groups are separated by parenthesis, and our entire expression includes the commercial at @ symbol, which looks for this character.

### Refences 
https://support.google.com/a/answer/1371417?hl=en
https://www.regular-expressions.info/email.html
https://javascript.info/regular-expressions


## Author

Domenic Wilhelm currently attending a Bootcamp offered by  Denver University to learn Coding/ Frontend Web-Development and get my Certificate visit my portfolio at 
https://domenicsw92.github.io/Wilhelm-Web-Developer/ or my github repo at https://domenicsw92.github.io/Wilhelm-Web-Developer/
 
