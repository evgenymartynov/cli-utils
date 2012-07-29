gist
----

    gist [file1] [file2] [...]

Creates a new Github Gist with the given files.
Uses Github API v3.
Also accepts a file on stdin if no arguments were given.

codepad
-------

    codepad [file1] [file2] [...]

Uploads a bunch of given files to codepad.org
Also accepts a file on stdin if no arguments were given.

sloc
----

    sloc [file1] [file2] [...]

Counts number of non-empty code lines, and comment lines (starting with "//").
Also counts mixed code-comment lines.
Also works from stdin.

evgeny_screenshot
-----------------

    evgeny_screenshot -h

Takes a screenshot of the entire screen, current window, or a selected area on screen.
Depends on `scrot` and `python-paramiko` package.

Best used in conjunction with `screenshot` in this repo.

screenshot
----------

    screenshot [--area | --window]

Wrapper around `evgeny_screenshot`.
Will copy the screenshot to a server of your choice, into a dir of your choice, with the optional /yyyy-mm/ subdirectory structure.

Copies resultant URL into both X clipboard and GTK clipboard.
