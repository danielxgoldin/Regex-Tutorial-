# Regex Tutorial 

To find certain patterns within a string, you can use regular expressions. In a string you can also find or replace a set of characters. These characters can also be used to validate imput. The regex code below is used to validate an email address. 

## Summary

We will be explaining this code: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
Anchors are regex tokens that don't match any characters but that say or assert something about the string or the matching process. For instance the anchors for this expression are ^ to start, and $ to finish.

### Quantifiers
A quantifier matches the preceding element zero or more times but as few times as possible. For instance, In this example,  the + symbol is used to tell the system there is another sequence to be matched as a greedy quantifier. {2,6} is used as another greedy quantifer to specify the input should be a minimum of 2 characrtors and a maximum of 6 characters.

### Character Classes

In regular expressions, a character class is a set of characters enclosed within square brackets. For instance in the above code, the character class is /d. Character classes classifies the use of any digit from 0 to 9.

### Flags

A flag is an optional parameter to a regex that modifies its behavior of searching. 

### Grouping and Capturing

A group is a part of a regex pattern enclosed in parentheses () metacharacter and capturing groups are a way to treat multiple characters as a single unit. For instance, In the above code 3 groups are being captured. The user name of the email will be in group #1 and will consist of [a-z0-9_\.-]. The domain or email service being used will be captured in group #2 and will consist of [\da-z\.-]. group # 3 will consist of the domain extension and use the following. [a-z\.]{2,6}

### Bracket Expressions

Bracket expressions are a list of characters and/or character classes enclosed in brackets []. For instance, the above example contains 3 bracket expressions. The bracket expression is used to identify which information is allowed to be matached. 

The first Bracket Expression will include the numbers from 0-9, case sensitive letters from a - z, it will contain periods a hypen and an underscore. [a-z0-9_\.-]

The second Bracket Expression will contain case sensitive letters from a - z, all the digits, a hypen, and a period. [\da-z\.-]

The third Bracket Expression will contain case sensitive letters from a-z and a period. [a-z\.]


### Greedy and Lazy Match

Basically, 'Greedy' means match longest possible string. 'Lazy' means match shortest possible string. We have only used Greedy match in the example above which are + and {}, this will allow it to expand the match infinitely until a match is found. 

### Boundaries

The metacharacter \b is an anchor like the caret and the dollar sign. It matches at a position that is called a “word boundary”. The above example does not have a "word boundary" as it does not contain a \b.

### Back-references
A back-reference is a regular expression commands which refer to a previous part of the matched regular expression.

There are no Back-references contained in the above example.

## Author

Hi, I am Daniel Goldin. I am about to finish up my coding boot camp at UT Austin. You may find me at the github below! 

Github:  https://github.com/danielxgoldin

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)