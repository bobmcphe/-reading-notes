# EJS Partials

Partials are meant to help people to not repeat the same process multiple times. Consequently, by using partials, we can not only save time, make code management easier, but also we can speed up websites as well.

Since EJS is able to work with HTML, we can take sections of HTML code that would exist on multiple pages, (e.g. a header section) and put this code in one page, called a partial, and house it within our views foldier, yet another folder titled partials. The example provided would be extracting the data from the header into the header.ejs file, as such:

```
<!-- views/partials/navbar.ejs -->
    <div class="header clearfix">
        <nav>
            <ul class="nav nav-pills pull-right">
                <li role="presentation"><a href="/">Home</a></li>
            </ul>
            <h3 class="text-muted">Node.js Blog</h3>
        </nav>
    </div>
```

This section would then be replaced with the following EJS line of code:

```
<%- include('partials/header') %>
```

That is about all that is needed to know to get started. 