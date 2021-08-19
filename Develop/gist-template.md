# Regex 101: Matching a Hex Value

In this tutorial I will be giving you all a breakdown of a regular expression. The regular expression (also know as "regex") that I chose to dissect for this lesson will be a hex value. I am sure that many of you are wondering what a hex value even is, right? Rest assured knowing that a hex value is a hexadecimal way to represent a color in a RGB format by combining three values to create any color. Hex value has been seen and used a lot by many front end developers, for the purpose of styling.

## Summary

Here is the regex sequence that we will be covering today: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

In the following contents below, I will be covering the different components in breif details in regards to the expression mentioned above in regards to the anchors, quantifiers, grouping constructs, bracket expressions and the or operator.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [The OR Operator](#the-or-operator)

## Regex Components

### Anchors

The two anchors that are in this expression are ^ $

The ^ lets the code reader know to look for the foillowing character to begin interpreting the code.

- In this case, the # starts the code search for the color hex code

The $ lets the code reader know that the end of the expression is completed directly before it.

- In this case, the code ends with the quanifier {3}.

### Quantifiers

The quantifiers that are in the regular expression above are ? {6} {3}

The ? means that the expression can only be matched zero to one time. The grouping constructs that encapsilated within the parenthesis is the pattern that can be only ran once. This is the pattern that outputs the selected color in which the user hovers over in the hex value search.

{6} limits the number of characters to 6 which are allowed to be associated with that specific portion of the expression. The included characters for this piece of expression could range from a-f and any whole integer from 0-9.

{3} limits the number of characters to 3 which are allowed to be associated with that specific portion of the expression. The included characters for this piece of expression could range from a-f and any whole integer from 0-9.

### Grouping Constructs

[a-f0-9]{6}|[a-f0-9]{3}

As seen in the above demo expression, this snippet of code is considered to be a grouping construct because it is wrapped in the parenthesis together which completes the grouped expression.

### Bracket Expressions

[a-f0-9]

Bracket expressions are any expressions that are wrapped in brackets as the above snippet of code. Bracket expresseions are usually associated with different components to complete a regex.

### The OR Operator

|

([a-f0-9]{6}|[a-f0-9]{3})

This pipe symbol represents the Or operator. What this symbol states is run the first group of the expression, if it is not true, run the second group of the expression. This Or operant makes for more flexibilty when it comes down to creating and accepting given pattens for a regular expression.

## Author

This tutorial was created by Tyree Nettles.

Here is a hyperLink to my gitHub account: https://github.com/tpnettles1
