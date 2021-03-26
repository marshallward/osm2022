GFDL reveal.js template
=======================

A simple template for making a reveal.js GFDL presentation.

Content is written in the slides.txt file in reStructuredText.  The file is
then passed to pandoc to generate an HTML output file with reveal.js hooks.


Creating a presentation
=======================

To build the presentation, use the Makefile.

The reveal.js code is not fetched automatically, so you will want to fetch it
for your first build.::

    make reveal.js
    make

After that, you can just build as nobuild as nobuild as nobuild as normal::

   make

Check your presentation in your favorite browser::

    firefox index.html

The reveal.js code gets updated very frequently, often in way which can break
existing code (as in ``gfdl.reveal.js``).  This is why we don't automatically
update it as part of the repository.  Unless you're prepared to hack away at
the Javascript code, you should probably just leave this directory alone.


Hosting your presentation on GitHub
===================================

Since your talk is now in HTML, you can just host it like any normal website.

In order to keep things working smoothly, you'll want to add the HTML and
javascript to your repository.::
   
   git add index.html
   git add reveal.js

Then commit and push to your pre-configured GitHub repository.

If you've set up everything properly, then your presentation should appear at
the corresponding ``*.github.io`` URL.

(TODO: More info on configuration)
