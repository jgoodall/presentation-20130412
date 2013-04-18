Presentation at [The Center for Intelligent Systems and Machine Learning (CISML)](http://cisml.utk.edu/) on 2013/04/12 on Visual Analytics.

Presentation created using [revealjs](https://github.com/hakimel/reveal.js).


## Build

To build the jade templates, run `grunt`:

    ./node_modules/grunt/bin/grunt

To create and push the presentation to the `gh-pages` branch:

    git checkout --orphan gh-pages
    git add .
    git commit -m 'initial commit on gh-pages'
    git push origin gh-pages