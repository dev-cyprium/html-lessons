# Basics of html
To structure a basic document you need to use a system of **tags**, which are the essential
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

So from now on every document you'll make will have the structure as above.

  - `html` is always the first html tag you'll write and is the root of the document
  - `head` contains mostly tags that instruct the **browser** on how to do things
  - `body` the content of our web site, and the part that the actual site users experiences

You might have also noticed `<!DOCTYPE html>` in the above example, and this is not a tag!
This is important for the browser itself, so that it knows that you're doing a **version 5 of html** (HTML 5)

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
the anchor `<a>` because it will not have any effect. To get a full list of attributes a tag can accept, just
go to [W3Schools](https://www.w3schools.com/tags/tag_img.asp)

So to get back at our `<img />` example, it doesn't do anything on it's own, but if you add `src` attribute
to it, you'll get the browser to display an image from that `src` attribute. The image can come from your own
location, or somewhere online.

```html
<img src="https://via.placeholder.com/150" />
```

Let's say you also want to add a link functionality to an image, and you can. Just combine what we've learned so
far!

```html
<a href="https://via.placeholder.com/150" target="_blank">
  <img src="https://via.placeholder.com/150" />
</a>
```

Try clicking it! You'll see that the image will open in the new tab 

## Now It's your turn!
The most fun you'll have is exploring on your own, here are some ideas you can do:
 - Go to [W3 Schools](https://www.w3schools.com/html/html_intro.asp) read their HTML tutorial
 - Open up your Visual Studio Code + Live Server, try adding various tags too see their effects
 - Using HTML tags, try making this example yourself
 - ![exercise](https://github.com/dev-cyprium/html-lessons/blob/master/docs/assets/exercise.png)