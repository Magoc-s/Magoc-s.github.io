## \_sass

The `_sass` directory contains all the scss stylesheets for the theme. All of these already exist in the theme repo itself and are pulled in via the bundler when the page is built. You can override/specify new theme variables in the custom-variables.scss file if you need too. There is a more detailed README file in the [jekyll-theme-anu repo.](https://gitlab.anu.edu.au/jekyll-anu/gems/jekyll-theme-anu/-/blob/3364b47a05677dd19252992519ed0551664c03a6/_sass/README.md)

Any new files you place in here will not be automatically included in the built webpage. But for more personalised/specific needs, you may edit the `./assets/css/styles.scss` and add additional `@import` tags.

## Licence

MIT
