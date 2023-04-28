# Ultimate-Regex-Tutorial
A regular expression is a special text string for describing a search pattern. It is commonly used to find patterns within a string, find/replace characters within a string or validate input. This tutortial will go walk through the components of a regex and how it applies to matching an email.


## Summary
This tutorial is going to explain the use of regex to match emails. This can be useful when validating emails using 
applications/technologies.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
Anchors don't match any characters but assert something about the 
string or the matching process.

The ^ anchor signifies the beginning of the string. 
The $ anchor signifies the ending of a string.

### Quantifiers
Quantifiers set the limits of the string that the regex matches, 
they frequently include a minimum and maximum number of characters 
the regex is looking for. 

(+) Matches the character before the + one or more times, connects 
the user email name + email service + .com.
{2,6} is saying that the requirement of the regex is between 2-6 
charcaters long. for the set [a-z\.].

### Character Classes
A character class matches any one of the enclosed characters 
enclosed in the square brackets. 

The \d Matches any digit (Arabic numeral), from 0-9. 

### Grouping and Capturing
Capturing groups are a way to treat multiple characters as a 
single unit. They are created by placing the characters to be 
grouped inside a set of parentheses. 

The [a-z0-9_\.-] matches the user email name.
The [\da-z\.-] matches the email service.
The [a-z\.] captures the .com.

### Bracket Expressions
Brackets indicate a set of characters to match, and  any 
individual character between the brackets will match. Hypens are 
also used to define a set.

The [a-z0-9_\.-] matches any letters form a-z and is case 
sensitive to lower case. It matches any number values between 0 
and 9. It matches also matches the characters "_", ".", and "-"
The [\da-z\.-] matches a single digit from 0-9. Any letter from 
a-z and is case sensitive to lower case. It also matches the 
characters "." and "-".
The [a-z\.] matches any letters form a-z and is case sensitive to 
lower case. It also matches the characters ".".

### Greedy and Lazy Match
This regrex include greedy matches. A greedy match means that By 
default, a quantifier tells the engine to match as much text as 
possible 

The + will match as many times as possible and giving back as 
needed.
The {} is used when matching the character or subexpression at least 2 times but no more than 6 times (as close to 6 as possible).

## Author
I am a full stack developer and you can view my projects at https://github.com/tlequernaque.