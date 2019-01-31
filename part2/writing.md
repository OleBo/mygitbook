My name is {{ name }}, nice to meet you

{{ foo.bar }}
{{ foo["bar"] }}

All the variables set via the book.json are available through the book variable.

book.author is {{ book.author }}

# Chapters about GitBook

{% for article in glossary.terms['gitbook'].articles %}
* [{{ article.title }}]({{ article.path }})
{% endfor %}

set lets you create/modify a variable.

{% set softwareVersion = "1.0.0" %}

Current version is {{ softwareVersion }}.
[Download it](website.com/download/{{ softwareVersion }})


Inline math: $$\int_{-\infty}^\infty g(x) dx$$


Block math:

$$
\int_{-\infty}^\infty g(x) dx
$$

Or using the templating syntax:

{% math %}\int_{-\infty}^\infty g(x) dx{% endmath %}


{% exercise %}
Define a variable `x` equal to 10.

{% initial %}
var x =

{% solution %}
var x = 10;

{% validation %}
assert(x == 10);

{% context %}
// This is context code available everywhere
// The user will be able to evaluate `exposedVar`
var exposedVar = 3;
// ... or call `exposedFunction`
function exposedFunction {
    return 3;
}
{% endexercise %}
