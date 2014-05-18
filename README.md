edmv
====

A small tool for bulk-renaming files using the editor of your choice.

WARNING: May delete everything on your computer. Read the LICENSE file and don't sue me.

todo
----

- better cli:
  . -e/--editor flag
  . better usage string
  . --help
  . --version

- don't use strip() to remove whitespace, just remove the single trailing newline

- add an extra newline at the end of the file, the remove it

- add sanity checks, only rename files if they all pass for every file:
  . check that names are different, skip moving file if they're the same
  . check that the source file exists
  . check that the source file can be removed
  . check that the destination directory exist
  . check that the destination file does not exist

- add tests:
  . create a bunch of files
  . small commands to filter text
  . check that files are where expected
  . check that if there are problems the operation is aborted

- nicer post-move reporting
  . line up pre and post names

- better demo video:
  . more complex renames
  . multiple editor types: command line, sed filter, os x app, vim, emacs

- better readme
  . os x app example: `export EDMV_EDITOR='open -Wa "Sublime Text 2"'`

- better temporary file name

- accept arguments from stdin
  . should it do it via an '-' argument, a flag, or just if anything is available on stdin?
