## \_includes

The `_includes` directory is for `html` extensions. Extensions/plugins (like `liquid-boxes.html`) are placed in here, then can be accessed by a liquid include tag.

i.e.: {% include liquid-boxes.html %}

Style-wise, includes sourced externally (i.e. grabbed from github or some other open source code sharing platform) should be placed in a folder titled `vendor` inside the `_includes` folder. I.e. the filepath of the [Jekyll Anchor Headings](https://github.com/allejo/jekyll-anchor-headings) include would be:

`./_includes/vendor/anchor_headings.html`

Additional README's exist in the jekyll-theme-anu repo.

## Licence

MIT
