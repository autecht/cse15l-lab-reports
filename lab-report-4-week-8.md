https://docs.google.com/document/d/1pRCPCxCt_zvS4dEZXCNvsFvaejKSj--nC9fMYW81by8/edit#

# Adding and Reviewing Tests
In this report, we are adding tests to markdown-parse implementations and discussing whether the implementations pass and how easily they could be improved.
## Links
[Here](https://github.com/autecht/markdown-parser) is the first markdown-parse repository, which is mine.

And [here](https://github.com/ddn005UCSD/markdown-parser) is the second one, which is the one our group reviewed in the week 7 lab.

## Tests
### Snippet 1
The first test looked like this:
```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```

`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)

Expected output
How I turned it into a test
test output for mine
test output for theirs

### Snippet 2
The second test looked like this:
```
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
```
[a [nested link](a.com)](b.com)
[a nested parenthesized url](a.com(()))

Expected output
How I turned it into a test
test output for mine
test output for theirs
### Snippet 3
The third test looked like this:
```
[this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
```
Expected output
How I turned it into a test
test output for mine
test output for theirs
    

