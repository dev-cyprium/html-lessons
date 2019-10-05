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

