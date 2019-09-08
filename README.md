# Pluralizer

## Description

Two horses. Five monkeys. Twenty flies. One cat. Nine lives. Despite the English language being one of the most commonly used languages around the world, it is also quite complicated to learn if you are not a native speaker. Taking a noun and converting it to its plural form has a dozen rules and even more special cases. In this lab, you will write a program that takes words and makes them plural.

## Prerequisites

List any topics that would be required to complete the project (exclude extensions), for example:

- String manipulation
- Getting User Input
- Conditional statements
- Type conversion

## Prompt

Your program should take in two inputs: a non-negative number, and a singular noun. If the number entered is 1, then you would just print out "1 horse". However, if the number is 0 or greater than 1, you would print out the number and the pluralized version of the word - like "0 horses" or "4 horses".

Your program will be handling the following rules to pluralize nouns:

| If it ends in...                                                                                                             | Rule                    | Example                                             |
| ---------------------------------------------------------------------------------------------------------------------------- | ----------------------- | --------------------------------------------------- |
| -fe                                                                                                                          | Replace "fe" with "ves" | life, lives                                         |
| -y                                                                                                                           | Replace "y" with "ies"  | family, families                                    |
| -sh, -ch                                                                                                                     | Add "es" to the end     | bush, bushes                                        |
| -us                                                                                                                          | Replace "us" with "i"   | cactus, cacti                                       |
| -ay, -oy, -ey, -uy<br/>(The above rule is included because it is a special<br/>case that conflicts with the first "y" rule.) | Add "s" to the end      | guy, guys<br/>boy, boys<br/>key, keys<br/>day, days |
| All other cases                                                                                                              | Add "s" to the end      | cat, cats                                           |

Note that in order to handle cases where the word ends in "y" correctly, you will need to take some care. It is important that you order your conditions so that your code will check for the special case endings of "ay", "oy", "ey", and "uy" before simply checking whether a word ends in "y".

## Testing

Although it is a good idea to come up with some of your own test cases to realize the limitations your own code, the following are some inputs you can use to verify that your program works as intended. You can also test using the examples in the table above.

| Input (#) | Input (word) | Result   |
| --------- | ------------ | -------- |
| 0         | dog          | 0 dogs   |
| 1         | city         | 1 city   |
| 5         | fish         | 5 fishes |
| 33        | fly          | 33 flies |
| 8         | life         | 8 lives  |
| 20        | cactus       | 20 cacti |

## Extensions

There are many more rules to making words plural - see more [here](https://www.grammarly.com/blog/plural-nouns/). Try to see how many you can implement, including a few special cases as well!
