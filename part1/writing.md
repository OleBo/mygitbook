# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag

Hello {#id}
-----

# Hello {#id}

# Hello # {#id}

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

~~This text will be crossed out.~~

_You **can** combine them_

* Item 1
* Item 2
  * Item 2a
  * Item 2b
  

This is [an example](http://example.com/ "Title") inline link with a title.

[This link](http://example.net/) has no title attribute.

This is [an example][id] reference-style link.

[id]: http://example.com/  "Optional Title Here"

An image: ![gras](img/image.jpg)

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

This is a sample code block.

    Continued here.
    
    
```
function test() {
  console.log("notice the blank line before this function?");
}
```

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

Use `gitbook` to convert the `text` in markdown
syntax to HTML.

Text prior to footnote reference.[^2]

[^2]: Comment to include in footnote.

<div>
Markdown here will not be **parsed**
</div>


Three or more...

---

Hyphens

***

Asterisks

