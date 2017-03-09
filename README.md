# README #

A quick exploration of using `entr` to watch for filechanges.

### How do I get set up? ###

* `brew install entr` if you have homebrew installed. `entr` is an open source project hosted on http://entrproject.org.

### How do I do stuff? ###

`entr [-cdprs] utility [argument /_ ...]`

`entr` takes a list of whitespace separated file paths from standard input and watches them for changes. The fun part is that you're able to supply an arbitrary command to run which can be pretty much anything. It can be a test, or to automatically build a project, a script, or even a child process entr can restart on its own when you supply the `-r` flag - like a server or a daemon. I dunno - it's useful!

There's a few examples in this project to help you get started.
