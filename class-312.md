## EJS Partails 

> partains are akin to fucntions for **EJS**  you ca define a reusable bundle of code in a file and use it when ever you need it.

`<!-- views/partials/navbar.ejs -->
    <div class="header clearfix">
        <nav>
            <ul class="nav nav-pills pull-right">
                <li role="presentation"><a href="/">Home</a></li>
            </ul>
            <h3 class="text-muted">Node.js Blog</h3>
        </nav>
    </div>`

    >an example of a partail that would be found in views/partials directory

    > syntax to include partains is as follows

    ` <%- include(PARTAIL_FILEPATH)%>`
    