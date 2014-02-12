grelease
========

#### Grelease is a script to quickly and easily create a tarball of a git repository.

Installation
======
>**NOTE**
Grelease requires the **git** binary to function

Grelease is ready out of the box, simply run it with `./grelease`
It is recommended that you move it into your $PATH for easy access anywhere, but grelease doesn't really mind either way.

Usage
======
From `grelease -h`:
>grelease DIR COMMIT [OPTIONS] ...
Options:
-p NAME   Set the output package name
-o DIR    Set output package directory (default ../REPO)
-V STRING Set the output version string
-v        Verbose mode
-h        Show this message

Examples
======

#### Creating a 'repo' release from tag '1.0.0' but naming the version '1.0.0~RC1'
`grelease repo 1.0.0 -V 1.0.0~RC1`

#### Creating a 'repo' release from inside the 'badname' folder
`grelease badname 1.0.0 -p repo`

#### Setting the tarball output location
`grelease repo 1.0.0 -o ~/some/dir`