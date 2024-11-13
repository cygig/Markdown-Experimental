# Markdown-Experimental
This is for me to experiment with Github Flavoured Markdown.
<br>
<br>
<br>

# Newlines

Line 01: Newline on Line 2 will not be rendered.
Line 02: Unless it has trailing 2 spaces at the end like this,  
Line 03: then the newline will appear.

Line 05: Line 4 will show up as newline since Line 5 will be a new paragraph.


Line 08: Only one newline will show between the two on Line 6 and 7.
<br>
<br>
Line 11: br on Line 9 and 10, but only one newline shows, because the first br goes to Line 8.  
<br>
<br>
Line 14: br on Line 12 and 13 plus 2 trailing spaces on Line 11. Now the two newlines display correctly.

<br>
Line 17: Newline on Line 15 and br on Line 16. No trailing spaces on Line 14. Works as expected.

<br>

Line 21: Newline on Line 18 and 20, br on 19. No trailing spaces on 17. Did not work.
<br>

<br>
Line 25: Newline on Line 23, br on 22 and 24. No trailing spaces on 21. Only 2 newlines show instead of 3.
<br>
<br>
<br>

Line 29: Newline on Line 28, br on 26 and 27. No trailing spaces on 25. Only 2 newline show instead of 3.

<a name="bpnl"></a>
## Best practise for newlines

First line of text. No trailing spaces. Add as many br newlines you need and pad with a newline:
<br>
<br>

Second line of text has 2 newlines between the first.
<br>
<br>
<br>

# Spaces

One space between the arrows -> <-  
Two spaces between the arrows ->  <- but only one will show.  
One nbsp between the arrows ->&nbsp;<-  
Two nbsps between the arrows ->&nbsp;&nbsp;<- both spaces will show.  
Space, nbsp then space between the arrows -> &nbsp; <-, all three spaces will show.  
nbsp, space, nbsp between the arrows ->&nbsp; &nbsp;<-, all three spaces will show.  
space, space nbsp, space, space between the arrows ->  &nbsp;  <-, only three spaces will show since multiple spaces are collapsed into one.

## Best practise
For one space between the arrows -> <-, just use space normally.  
For two space between the arrows ->&nbsp;&nbsp;<-, use two nbsps.  
For more than 2 spaces between the arrows -> &nbsp;&nbsp; <-, pad the edges with space and use nbsps in the centre.  
<br>
<br>
<br>

# Headings

Text before heading doesn't seem to affect it.
### Heading 1
Text after heading also doesn't seem to affect it.

<br>
### Heading 2
Having a break with no text above the break will ruin the heading 

Break below a heading is fine
### Heading 3
<br>

But if you have some text above the break, the heading will be fine
<br>
### Heading 4
<br>
You can have some text after the heading too!

## Best Practise

### Leave a newline before the top and do not use breaks after
Then write your content directly underneth.
<br>
<br>
<br>

# Tables

Text before a table is fine!
| Header1 | Header2 | Header3 |
|---------|---------|---------|
| abc     | def     | ghi     |
Text directly after a table will be rendered as part of it.

You will need a new line to write text outside of table again.

<!-- Having a break with no text above the break will ruin the table  -->
<br>
| Header1 | Header2 | Header3 |
|---------|---------|---------|
| ruined  | with br | on top  |

But if you have some text above the break, the table will be fine
<br>
| Header1 | Header2 | Header3 |
|---------|---------|---------|
| abc     | def     | ghi     |
<br>
A break below table is fine.

## Best Practise

You can have some text before the table. It will automatically leave a newline. If you need more, use breaks and newline before table. See [this](#bpnl).
<br>
<br>

| Header1 | Header2 | Header3 |
|---------|---------|---------|
| abc     | def     | ghi     |

Leave a newline then type again.

# Headers

## You cannot **bold** or <u>underline</u> or <em>emphasise</em> text in H2 headers
## You can use `code blocks` or *italicise* or <sup>superscript</sup> or <sub>subscript</sub> or <mark>highlight</mark>text in H2 headers
