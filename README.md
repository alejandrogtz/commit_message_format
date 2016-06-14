Commit message format (version 1.7)
===================

##What is it?
This is a proposal of tags to be used in commit messages. The goal is to identify easily the different types of changes in the project's repo.

##Commit Message rules

####Subject description (first line)
>1. Prefix the line with an applicable emoji (tag)
>2. Limit the subject line to 50 characters
>3. Separate subject from body with a blank line
>4. Capitalize the subject line
>5. Do not end the subject line with a period
>6. Use the imperative mood in the subject line

####Message body
>7. Wrap the body at 72 characters
>8. Use the body to explain the problems, limitations, and why it is necessary. Then to explain how was addressed the issue and the effects.

A complete description, rules and tips can be seen in [1].

####Tags and meaning for source code
**NOTE:** The first commit does not have a label, and the message always is "**Initial commit**" as convention.

>* [api] when functions, methods or classes have been added, modified or removed; method signatures or return types have changed
>* [code] when improving the format/structure of the code, without modifying the previous functionality
>* [main] when dealing with a file that is used as view, notebook or main file
>* [misc] anything not covered by the above categories, e.g. rename or move files, add configuration files, add dataset
>* [new] when adding a new feature (see *Rules* section)
>* [pkg] when libraries, frameworks, packages  or modules are added
>* [style] when writing documentation, formatting or comments on code; no code change
>* [test] when adding tests, refactoring tests; no production code change



####Tags and meaning for database

>* [ak] alternate key
>* [chk] check restriction
>* [col] column
>* [dt] data type
>* [fk] foreign key
>* [idx] index
>* [mv] materialize view
>* [pk] primary key
>* [seq] sequence
>* [tbl] table
>* [trg] trigger
>* [vw] view

####Subtags
Those subtags are used in order to provide the action that the commit does
>* *add* when something new has been added
>* *boost* when improving performance
>* *bug* when a bug is found (see *Rules* section)
>* *fix* when fixing a bug (see *Rules* section)
>* *edit* when changes in files have been made
>* *move* when files are moved between directories
>* *remove* when files or directories are deleted
>* *rename* when files or directories are renamed
>* *update* when a package's version is changed, module is added, removed or modified (see *Rules* section)


When fixing something on:
>* *and* (*Android*)
>* *ios*
>* *linux*
>* *macos*
>* *win*


Those subtags must be used just in combination with other tags to specify a particular change related to an O.S.
>Example:
>  [api->macos] Subject description

####Rules
1. The tag [new] is only used when you are doing a merge between a feature-branch and develop.

2. The tag [update] must be used just when a package is updates ([pkg|update]).

3. Sometimes when you are doing modifications on your source code, it is likely to find a bug, in this case two actions can occur:

>+ [api->modify+bug] when the code was modified, a bug was found but NOT fixed
>+ [api->modify+fix] when the code was modified, a bug was found and WAS fixed

##REFERENCES

1. [How to Write a Git Commit Message](http://chris.beams.io/posts/git-commit/#why-not-how) Chris Beams
2. [TYPO3 CMS](http://wiki.typo3.org/CommitMessage_Format_(Git))
3. [Atom](https://atom.io/docs/v0.186.0/contributing)
4. [Karma](http://karma-runner.github.io/0.8/dev/git-commit-msg.html)

-------------
This document was last modified on : June 13th, 2016.
