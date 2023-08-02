# Understanding REGEX or Regular Expressions with Alex M🎉🎉 (replace with your title)

Introductory paragraph (replace this with your text)

Welcome, this is a markdown created with the purpose of explaining how regular expressions or REGEX work and why they are important to programmers. 

A regular expression is a search pattern used to look through a string of text. A way REXGEX
can be useful is validation, find and replace or simply filters for text that can be tweaked to be specialized or general. Regular expressions use literals which can simply be put as the characters found on your keyboard and Meta characters which are combinations of characters that define the search criteria. REGEX can be very useful to search and filter thought strings of text, in the markdown you will find out how and why there are so important. Lets looks out a REGEX and see how it works.

## Summary ✨

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

lets break down this REGEX responsible for finding zip codes like 84094 or 84094-1234:

`
[0-9]\{5\}(-[0-9]\{4\})?
`

at first glance this may seem like a complicated string of characters but once broken down into parts REGEX can be very powerful. lets break this down, the first part of this REGEX is 

`
[0-9]
`

This simply means that this REGEX will find any numbers `0-9` and the square brackets on the outside of the `[0-9]` simply indicate the range of which characters you wont to find and since we are looking for zip codes we can would need to be able to search for every number 0-9. The next part is:

`
\{5\}
`

The first part of this snippet is the `\` which is able to mark the next character as either special character or a literal which is useful for the next part of the REGEX which is `{5\}` which is looking to match the characters or numbers in this case to exactly 5 times. now the final part:

`
(-[0-9]\{4\})
`

Once again we are looking for numbers 0-9 that matches up for times which would be for some zip codes that have more then 5 numbers like 84094-1234 but now there are some characters in there that help us narrow down the last bit of numbers. our parenthesis `()` are a group which is helps us group the final 4 numbers of the zip code. and our `-` finds us the our dash in a longer zip code, the final part would be the question mark `?` which says that we don't need the final 4 numbers in zip code if the previous 5 numbers exists our question mark acts like an option so the last 4 numbers are optional. 

That is a quick overview of REGEX work and the last bit will be the working parts of REGEX that make the magic happen.
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
Two important anchors in REGEX are `^` and `$`, the `^` anchor signifies the begging of a string with the characters of the anchor that follow it or simply the matches the beginning of the input. The `$` signifies a string with the characters that precede it or simply matches the end of a input.
### Quantifiers
Set the range for us to make sure we can get the result we want. simply put they set the limits of the string that we want to match in REGEX. some important ones are: `* + ? {}` the star `*` matches the pattern zero or more times, the `+` matches the pattern one or more times and finally the `?` matches the pattern zero one time which is what we used in our summary to optionally find our last 4 numbers of our zip code. the `{}` matches the string either a specific amount of times that are inside of the brackets. 

### Grouping Constructs
grouping constructs are like bracket expressions but cooler and one example `(abc):(xyz)`
which would search for a string matching exactly abc:xyz. so they are used to look for exactly what you are looking for. 


### Bracket Expressions
As explained earlier in the summary the `[]` square brackets indicate a range of characters inside of the regular expression it can be `[a-z]` or `[0-9]` and we can also combine a range of numbers with an anchor which would give us a range of character's to be excluded in the range. 

### Character Classes
`.` - is the global characters inside of regular expressions it would find everything 



### The OR Operator
The or operator is `|` which can be seen as `A|B` which means we either want A OR B we want on or the other. 

### Flags
Expression flags changed how the string of text is interpreted and they are written following the closing forward slash of the expression. `/.+/igm `

`G `- is the global expression flag to find any character's matching that characters entered 

`I` - case insensitive search case where characters would be ignored inside of a search.

`m` - multi line search is a multi line input where strings would be treated as multiple lines 

### Character Escapes
since a lot of our meta characters are literal characters we need characters breaks which is `\` which makes all meta characters lose their value treating them as normal characters.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

