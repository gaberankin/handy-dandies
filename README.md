handy-dandies
=============

Repo for the things I make that help me work

git-lint
--------
I normally run this script prior to commiting things.  It reads the output from `git status`, checks if any of the files within are php or javascript files, and lints them for errors (and in javascript's case, fiddly things that are easy to miss).

It requires python.  A little configuration may be required prior to running this script.  First off, edit the file and change the `PHP_PATH` and `JSHINT_PATH` variables to the locations where your system can find your copies of the programs.  If you don't want to have the script linting certain types of things, just set the associated `*_PATH` variable to `None`.

Once you've done that, copy the script somewhere where your system can easily find it (i created a 'bin' directory in my systems home directory and added it to my path) and then do

```bash
sudo chmod +x git-lint
```

I guess nowadays I should point out that this was written when python 2.7 was the version of python everyone used.  I think it's still the case now, but a lot of people are moving up to v 3.x (at least, that's what I've observed in the student code reviews I'm involved in)
