# EJS

`npm install ejs` - installs ejs dependencies

`app.set('view engine', 'ejs')` - sets ejs as teh view engine and will look in views folder when rendering to the page.\

## Create EJS Partials

Like a lot of the applications we build, there will be a lot of code that is reused. 
We’ll call those partials and define three files we’ll use across all of our site: head.ejs, header.ejs, and footer.ejs

`<%- include('RELATIVE/PATH/TO/FILE') %>` - adds the partials to HTML
  - The hyphen <%- instead of just <% to tell EJS to render raw HTML.

## Pass Data to Views

```
app.get('/', function(req, res) {
    var mascots = [
        { name: 'Sammy', organization: "DigitalOcean", birth_year: 2012},
        { name: 'Tux', organization: "Linux", birth_year: 1996},
        { name: 'Moby Dock', organization: "Docker", birth_year: 2013}
    ];
    var tagline = "No programming concept is complete without a cute animal mascot.";

    res.render('pages/index', {
        mascots: mascots,
        tagline: tagline
    });
});
```

```
<h2>Variable</h2>
<p><%= tagline %></p>
```
  - Render single variable to HTML
  


