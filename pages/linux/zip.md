# zip

> Packages and compresses (archives) files into zip file.
> More information: <https://manned.org/zip>.

- Archive specific files/directories [r]ecursively:

`zip -r {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}}`

- Add files/directories to a specific archive:

`zip -r {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}}`

- Remove files/directories from a specific archive:

`zip --delete {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}}`

- Archive files/directories e[x]cluding specified ones:

`zip {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}} --exclude {{path/to/excluded_files_or_directories}}`

- Archive files/directories with a specific compression level (`0` - the lowest, `9` - the highest):

`zip -r -{{0-9}} {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}}`

- Create an encrypted archive with a specific password:

`zip -r --encrypt {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}}`

- Archive files/directories to a multi-part [s]plit zip file (e.g. 3 GB parts):

`zip -r -s {{3g}} {{path/to/compressed.zip}} {{path/to/file_or_directory{1,2,...}}}`

- Print a specific archive contents:

`zip -sf {{path/to/compressed.zip}}`