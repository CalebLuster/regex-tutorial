# Email Regular Expression Tutorial

In this gist I will tell you about the specific regular expression, or regex for short, that is used for matching emails. Regexs are mainly used when you are trying to match a certain sequence of number, letters, or special characters in a string. You can use regexs for alot more then just mathing emails, but for the purpose of this weeks challenge I have chosen to do a tutorial on this specific regex becuase I feel like it is most useful.

## Summary

The regex I choose was matching an email. Here is a code snippet I found for a simple email

      ^\w+@[a-zA-Z_]+?\.[a-zA-Z]{2,3}$

What we can get from this code snippet is that it is an simple email expression. This doesn't allot numbers in the domain name. It also does not allow for top level domains that are LESS than 2 or more than 3 letters. We can see this inside the curly braces of the expression.

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

    ^\w+@[a-zA-Z_]+?\.[a-zA-Z]{2,3}$

In this code example we can see the anchors, which are the "^" at the start and the "$" at the end.

In this code snippet we are looking for something that starts with 

    ^\w+@[a-zA-Z_]+?\

If this is found then what follows alos has to end with the other half. The period in the expression kind of seperates the two anchors in this given example. Notice how the second half follows with a period as normal javascript would.

    .[a-zA-Z]{2,3}$

If the code does not start or end with these anchors then the email will not match.
### Quantifiers

A quantifier is kind of exactaly what it sounds it would be. It decides how many TIMES a certain number, letter, or special character is going to have to be PRESENT in order to find a match. 

    abc+

So in this code we have the abc+ which will match our string becuase ours is 

    ^\w+@[a-zA-Z_]+?\

If you notice it says "a-z" which menas this will match.

### OR Operator

Our specific example does not use this but the OR Operator is as simple as it sounds.

It uses x or y to match. Here is a unrealistic example

    x|y

This is a very simplified example but it is essientaly saying these requirments OR those requirments to match.

### Character Classes

Character classes make sure that a letter follows the @ symbol in an email and not a special character or number. It is stated after the @ symbol when trying to match an email.

### Flags

No flags are being used in this example

### Grouping and Capturing

This is just essentially checking each section and varifying it matchs before moving on to the next one. The first group that appears is

    ^\w+@[a-zA-Z_]+?\

and once that matches it checks the next group in our regex which is 

    .[a-zA-Z]{2,3}$

The guidelines must be matching to move on the the next section or group of characters.

### Bracket Expressions

    ^\w+@[a-zA-Z_]+?\.[a-zA-Z]{2,3}$

In our example we can see that there are, in fact, brackets in our snippet!

These are simply SETTING the guidlines for group. In the first expression we have [a-zA-Z_] this means any letter a-z, A_Z, or an underscore.

Pretty cool stuff!

### Greedy and Lazy Match

No examples in this code snippet

### Boundaries

No examples in this code snippet

### Back-references

No examples in this code snippet

### Look-ahead and Look-behind

No examples in this code snippet

## Author

Created by Caleb Luster

If you need to contact me ⬇️

<a href="mailto:cwl117@outlook.com">Email<a>

<a href="https://github.com/CalebLuster">GitHub<a>

