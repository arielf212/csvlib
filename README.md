# a library for handling csv files for the LDPL programming language
csvlib is a single-file library written in LDPL, for LDPL.

it includes two procedures, one for writing a line and the other for reading a line.

## how to set up
include this file before any other file in your project.

for example, if you are compiling a file named "source.ldpl", your compilation line will look like this:

`$ ldpl csvlib.ldpl source.ldpl`

## examples and documentation
you can find examples of writing and reading into/from a file in the [examples](/examples) subfolder.

## but what if I want to know how to use the library right now and not burn time trying to understand your horrible documentation?

*fiiiine!*

store the filename inside `csvlib.filename`.
#### write
store everything you want to write inside `csvlib.writeValues` and call `csvlib.writeLine`.
#### read
store the line number inside `csvlib.lineNumber` and call `csvlib.readLine`.
your values should be stored inside `csvlib.readValues`.