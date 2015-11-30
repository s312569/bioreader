# bioreader

A simple library for opening readers on compressed files. Currently
supports gzipped, zipped and bzipped files using strings or
java.io.File objects as inputs. The type of compression is determined
by examining the extension of the file - '.gz' for gunzipped, ".zip"
for zipped or ".bz2" for bzipped.

## Usage

Library defines a single function `bioreader' which takes a string or
a java.io.File object as an input and returns a buffered reader. If
the underlying file is zipped, gzipped or bzipped the appropriate
input streams are applied before returning the buffered reader.

## License

Copyright © 2015 Jason Mulvenna

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
