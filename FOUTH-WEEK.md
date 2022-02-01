MONDAY CHALLENGES

REGULAR EXPRESSIONS:

A regrex(regular expression) consists of a sequence of sub-expressons. A regex may match a portion of the input (substrings) or the entire input. 
In fact, it could match zero or more substrings of the input (with global modifier). This regex matches any numeric substring (of digit 0 to 9) of the input.

For example in JS we find all "matching" patters with the method match() for example:

const matches = 'Some Text'.match(regex);

We'll use search for a single match for example:

const index='Some Text'.search(regex);

For replace matching patterns we'll use:

const next='Some Text'.replace(regex, 'Hi Mom!');

const regex=/"in this area we will put the pattern we are looking for"/ but if it has an particular behaviour must add a particular flag, these are the flags available:

i = with this flag the search is case-insensitive: no difference between A and a

g= with this flag the search looks for all matches, without it - only the first match is returned

m= multiline mode (covered in the chapter Multiline mode of anchors ^ $, flag "m")

s= enables "dotall" mode, that allows a dot "." to match newline character \n (covered in the chapter Character classes (\d= is from digit) (\s= is from space)(\w is from word)
or any inverse classes 

u= enables full unicode support. The flag enables correct processing of surrogate pairs.

y= "Stycky" mode: searching at the exact position tin the text

ir order to crear more RegEx we can combine . ^ $ * + - ? () [] {} \ |

to create a logical we use |
to group we use ()
to allow 0 or 1 times we use ?
to allow 0 or many times we use *
to allow 1 or many times we use +
to an explicit counts we use {MIN, MAX}
to escape special chars we use \
to search any digit we should use \d
to exclude any digit we should use \D
to set an specific characters we use []
to do the opposite of an specific character we use [^LBC]

we can use pages like "regexr.com" or "regex101.com" to test any regular expression buit by yourself

















