grunt-set-static
================

grunt-set for a static site.

## Features

* concat js files
* auto include bower dependencies
* pre-process less files
* process html files with handlebars
* support for partials
* support for layouts

## Suggested Structure

```
src/
  index.html
  page2.html
  styles/
    vars.less
  scripts/
    global.js
  layouts/
    layout1.html
  modules/
    module-name/
      view.html (available to load as a partial)
      style.less
      script.js
  images/
    logo.png
  fonts/
    app.ttf
```

## Ouput

```
www/
  index.html
  page2.html
  styles/
    site.css
  scripts/
    site.js
  images/
    logo.png
  fonts/
    app.ttf
```

## Commands

* `dev` - run a dev server and watch for changed files
* `dist` - minify files and write everything to `dist` folder
* `deploy` - deploy site to s3
