# EJS Partials

Partials are a way to reuse the same HTML across multiple pages/views.
You can define a block/bundle of code in one file and reuse that file in every page you need to.

Once you have created a partial such as header.ejs or footer.ejs you can use this in any page.
For example in the home.ejs or a home page you can render the header.ejs file by using ejs templating

  - `<%- include('partials/header') %>` this will render the HTML for the header.ejs in your current page

This can be used for all pages and will make the site easier to maintain and also look the same through out.


