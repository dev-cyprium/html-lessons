# Basics of html
Do structure a basic document you need to use a system of **tags**, which are the essential
building blocks of Web site. Think of them as the skeleton of your website, as they define
the layout of your website.

Every tag has what's know as their area of influence and that's between it's open and close
notation like so:

```html
<tag>
  Area of influence
</tag>
```

Which means that any content (even other tags) in the area of influence will be **affected by that tag**

Every webpage you'll make has the following base set of tags:

```html
<!DOCTYPE html>
<html>
  <head>

  </head>
  <body>

  </body>
</html>
```

So from now on every document you'll make will have the structure as above. Each of the tags has some sort of meaning:

  - `html` is the root html tag which described an html document
  - `head` contains mostly tags that instruct the **browser** on how to do things
  - `body` the content of our web site, and the part that the actual site users experiences

## The anatomy of a tag
A HTML tag can either be a pair of opening and closing tags, or a more rare self closing tag.
```html
<h1>I'm a closing tag</h1>
<img /> 
```

Self closing tags might seem offputting, as a tag without content doesn't seem to add any function. Well, that's
why my friend you need tag **attributes**.

**Attributes** are a way of adding tiny bits of extra metadata to HTML tags and they include a huge set of things 
they can do, from adding a location where the link leads, adding a source to an image, to grouping HTML elements
for easier styling.

Attributes can be specified for **any html tag** and look like this:
```html
<h1 myAttribute='value' myOtherAttribute='someOtherValue' class='foo-bar'>
```

We just applied the 3 attributes `myAttribute`, `myOtherAttribute` and `class` to our `<h1>` html element!

Attributes themselfs can be categorized into organizational tags like eg. `class` and `id` and functional tags,
like eg. `type`, `href` and `src`. Organizational tags *don't do anything on their own*, but rather help
us group tags into meaningful groups so we can easly style them later (more on styling later), while functional
tags give additional functionality from the browser to the tags.

Note that you can use organizational tags on *any HTML tag*, and you can't use `href` on any other tag other then
the anchor `<a>` because it will not have any effect.