
This is a fork of [reveal.js](https://github.com/hakimel/reveal.js/) that uses [Jade](https://github.com/visionmedia/jade) templates and a custom theme to create web presentations.

For more on reveal.js, [check out the live demo](http://lab.hakim.se/reveal-js/). See [reveal.js github page](https://github.com/hakimel/reveal.js/) for documentation on how to configure and use.

## Setup

All configuration and content goes in the `source` directory. In that directory are the following files:

`_config.jade` - set the variables in here to set meta-data for the generated presentation.

`index.jade` - this is where you files should go. The file should look something like this.

    extends includes/layout

    block slides
      //- each slide should start with section, or nest sections for vertical
      section
        h1 TITLE
        h2 subtitle
      section
        h2 Agenda
        ul
          li some <strong>stuff</strong>?
          li more stuff!
        aside.notes
          | notes go here.

The theme assumes `h1` is used for main presentation titles, while `h2` is used for the title on each content slide.

You should not need to edit the files in the `includes` directory.


## Build

To build the jade templates, run `grunt`:

    ./node_modules/grunt/bin/grunt


To watch for changes to the template, run:

    npm run-script watch


## License

MIT licensed

Copyright (C) 2013 Hakim El Hattab, http://hakim.se