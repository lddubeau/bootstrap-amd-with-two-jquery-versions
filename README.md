This repo demonstrates how to load two different versions of jQuery, and use one of them for Bootstrap.

* Version 1.8.3 installs itself as the globals ``$`` and ``jQuery``.

* Version 1.10.2 is installed as an AMD module. It is reachable *only* through using RequireJS.

The bootstrap-amd tool was used to generate an version of Boostrap which is an AMD module. Here's the recipe I used:

    $ git clone https://github.com/twbs/bootstrap.git
    $ npm install bootstrap-amd
    $ mkdir bootstrap/amd # Work around bug in bootstrap-amd.
    $ node_modules/.bin/bootstrap-amd bootstrap

This repository contains only the **finished** product without all the intermediary tools necessary to create it.
