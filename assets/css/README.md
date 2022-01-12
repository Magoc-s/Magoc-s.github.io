## assets/css/styles.scss

This `styles.scss` file is included by default in the theme, but you may override it by including it locally. The template includes a copy of this `styles.scss` that is identical to the one in the theme (i.e. we override it with the exact same thing).

If you do not need to use this file, you may delete it (or even the /css/ directly) entirely.

## assets/css/

This directory can be used to include sass stylesheets which are used at build-time to generate css style sheets. `@import` tags in these files refer to the files in the `_sass` directory. 