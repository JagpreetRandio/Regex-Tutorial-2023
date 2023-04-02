# Regex-Tutorial
2023

## What is a Regex?
A regular expression (often called regex expressions) is a sequence of characters that create patterns to match character combinations in strings. Regex expressions patterns are identified by using string-searching based algorithms and can also be used when validating inputs.  


## Summary
For this tutorial, we will be learning about utilizing regular expressions (regex expressions) when 
matching an HTML tag. The following tutorial will help demostrate the usage of an HTML tag.

We will be looking at and breaking down the folllowing regex that can be used to match an HTML tag:

`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`

As we discussed in the introduction, regex expressions are a group of characters that are used when matching character combinations. For example, if you wanted to make sure that the format for an email or an username is correct, regex expressions can help you make sure that the format are correct.

`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`

This regex expression helps the user when parsing or validating an HTML tag in a string. Keep in mind, regexes are very flexible and work with many different languages especially when working with matching HTML tags.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

Anchors are used in Regex expressions when checking the first and last symbols in an expression. There are two anchors for the beginning and ending of a regex expression. 

For the beginning of a regex expression, we use the caret, `^`. The caret shows us the start of the expression to indicate that the search should at the beginning. 

|  Anchor  | Description                                             |
| :------: | ------------------------------------------------------- |
| ```^```  | Matches the pattern at the beginning of the expression  |
| ```$```  | Matches the pattern at the end of the expression        |

For the ending of a regex expression, we use the dollar sign, `$`. The dollar sign shows us the start of the expression to indicate that the expression must end with the regex pattern. 

### Quantifiers

Quantifers indicate the number of characters in a expression to match. 

|  Quantifer  | Description                                             |
| :------:    | ------------------------------------------------------- |
| ```*```     | Indicates that the regex expression is zero or more     |
| ```+```     | Indicates that the regex expression is one or more      |
| ```?```     | Indicates that the regex expression is zero or one      |
| ```{}```    | Indicates that the  numbers in the {} will between those numbers |

```abc|cba``` Indicates that the characters for the regex expression will match each other


### OR Operator

The OR operator (```||```) is a operater set to look at one thing or multiple things. The OR operater acts like a boolean because the operator matches the regex expression before or after the ```| ```. Within the ``` | ```, the OR operator can work as a group or on the entire regex expression. 

For example, when we are look at this example; ```<123> | <456>```. We are looking for either ```<123>``` or ```<456>```.

### Character Classes

Character Classes distinguish the different kinds of character in a a regex expression. Like differentating between a number or a letter. 

|  Character  | Meaning                                             |
| :------:    | ------------------------------------------------------- |
| ```\w```  | "w" stands for a word. Either a letter of the latin alphabet or a digit or an underscore  |
| ```\d```  | "d" stands for a digit. A character from ``0`` to ``9`` |
| ```\s```  | "s" stands for a space. A space symbol ``  ``    |
| ```\W```  | "W" stands for a non-word. Opposite of ``\w``    |
| ```\D```  | "D" stands for a non-digit. Opposite of ``\d``    |
| ```\S```  | "S" stands for a non-space. Opposite of ``\s``   |
| ```.```   | "." is a special character it stands for any character except for a newline |


### Flags

A regex expression may have flags that can affect the search. A flag changes the default search behavior of the regex expression. 

| Flag | Description| 
|:----:|---------------|
|``i``| Ignores all case sensitivity |
|``g`` |Matches for all occurances   |
|``m``| Matches at the beginning and the end for each new line |
|``u``| Allows the matching to be outside of the unicode |
|``s``| Dot All. Matches all whitespace characters within a string. Seen as a global search               |
|``y``| Matches from the last index property position.             |



### Bracket Expressions

Bracket expression ``[]`` are characters or characters in enclosed in ``[]``. When using ``[]`` bracket expressions, we are matching single characters in a list, or a full set of characters in a list. 

Let's look at examples!

| Bracket Expressions | Matches    | 
|:--------------------:|-----------|
| ```[abc]``` | Matches a,b, or c   |
| ```[a-z]``` | Matches through the alphabet  |
| ```[^abc]``` | Matches any character but will not match a,b,c  |
| ```[[:alpha:]]``` | Matches any character that is not in the alphabet |


### Sources and References

* [JavascriptInfo](https://javascript.info/)
* [MDN](https://developer.mozilla.org/en-US/)
* [PlainEnglish](https://plainenglish.io/)
* [TrendMicro](https://docs.trendmicro.com/all/ent/imsva/v8.5/en-us/imsva8.5_olh/usg_kw_exp_regexp_brkt.html)

## Author
[JagpreetRandio](https://github.com/JagpreetRandio) is a student currently enrolled at UW learning how to code. 
