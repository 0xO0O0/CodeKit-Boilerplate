CodeKit Boilerplate
===================

Basic setup for [CodeKit](http://incident57.com/codekit/) based on my personal preferences for building responsive web sites. It features:

* [Haml](http://haml.info/)
* [Sass](http://sass-lang.com/)
* [CoffeeScript](http://coffeescript.org/)
* [HTML5 Boilerplate](http://html5boilerplate.com/) (including [normalize.css](http://necolas.github.io/normalize.css/) and [Modernizr](http://modernizr.com/))
* [Bourbon](http://bourbon.io/) + [Neat](http://neat.bourbon.io/)
* [Respond.js](https://github.com/scottjehl/Respond) (_for IE < 9_)
* [jQuery Debounced Resize](https://github.com/louisremi/jquery-smartresize)

Compiled files are ignored by Git so the following files need to be compiled after cloning (_build-paths should be auto-configured when importing the project in CodeKit_).

    src/haml/index.haml  ->  build/index.html
    src/sass/style.scss  ->  build/css/style.css
    src/js/main.coffee   ->  build/js/main.js
    src/js/plugins.js    ->  build/js/plugins.js

Bourbon Neat's visual grid is enabled by default. To disable it, set `$visual-grid` to `false` in `src/sass/partials/_settings-grid.scss`.
