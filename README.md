dash-docsets
============

`sphinx2dash` generate docsets from sphinx-doc project


Usage
-----

    ./sphinx2dash -h #for help

e.g.

    ./sphinx2dash -g "git@github.com:kennethreitz/requests.git"

Under the hood
--------------

1. Clone code to `repo_lib` fold from git url specify by `-g`

2. Go to docs fold of the project in `repo_lib`, and make a copy of `Makefile` 
named `Makefile.dash` , and add nosidebar option to `Makefile.dash`

3. Run `Make -f Makefile.dash html`

4. Run `doc2dash` to generate docset, and add to dash
