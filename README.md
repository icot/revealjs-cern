revealjs-cern
=============

A [Reveal.js](http://lab.hakim.se/reveal-js/#/) theme trying to follow the official [CERN] (www.cern.ch) template for presentations as shown 
[here] (http://design-guidelines.web.cern.ch/presentations).

[CERN] (www.cern.ch) is the source of the images used as ghaphic resources for this theme, and retains the sole
copyright of all related imagery. For more information regarding this, please take a look to their [copyright](http://cern.ch/copyright).

You can see a demostration of how it looks by clicking [here] (https://icot.github.io/revealjs-cern/#/)

#### TODO

* Improve the footer CSS
* Change fonts?
* Adjust size of badges in Top and Tail slides
* Add style for customizable templates (currently only the 'strictly CERN' template is replicated


### Instructions

Anyone using [Reveal.js](http://lab.hakim.se/reveal-js/#/) should know how to use this and should be able to place any file wherever they want.
If you want to use it as provided:

1. Copy the project main folder in your **reveal.js/** folder.
2. Copy (and rename, if desried) *revealjs-cern/cern-template.html* up to the reveal.js/ folder
3. Edit your Gruntfile.js to add the SASS CERN css theme generation:

        sass: {
            main: {
                files: {
                    'css/theme/default.css': 'css/theme/source/default.scss',
                    'css/theme/beige.css': 'css/theme/source/beige.scss',
                    'css/theme/night.css': 'css/theme/source/night.scss',
                    'css/theme/serif.css': 'css/theme/source/serif.scss',
                    'css/theme/simple.css': 'css/theme/source/simple.scss',
                    'css/theme/sky.css': 'css/theme/source/sky.scss',
                    'css/theme/moon.css': 'css/theme/source/moon.scss',
                    'css/theme/solarized.css': 'css/theme/source/solarized.scss',
                    'css/theme/blood.css': 'css/theme/source/blood.scss',
                    'css/theme/cern.css': 'revealjs-cern/css/cern.scss',
                }
            }
        },

4. Run `$ grunt themes` to generate the CSS file


### Screenshots

![Top](screenshots/bluebadge.png "Top Slide")

![Title slide](screenshots/frontpage.png "Title slide")

![Generic Slide](screenshots/generic.png "Generic slide")

![Tail](screenshots/last.png "Tail slide")
