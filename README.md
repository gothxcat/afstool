# afstool

Commadore Amiga Fast Filesystem interaction shell script for GNU/Linux.

## Functions

Provide a user-friendly CLI to:

- Extract files from AFFS disk images to an output directory
- Create ZIP archives from AFFS disk images
- Recursively update extracted Amiga file and directory attributes to UNIX-compatible flags

## Dependencies

- bash >= 4.x.x
- GNU coreutils
- mount, affs driver (Linux Kernel >= 2.x.x)
- zip (Info-ZIP)

## Usage

`./afstool -h` displays usage

<pre>
usage: afstool [options]
Amiga filesystem interaction script for GNU/Linux.

options:
 -x, --extract [filename]           extracts an AFFS disk image
                                      (use with -o)
 -a, --archive [filename]           creates a ZIP archive from an AFFS disk image
                                      (use with -o)
 -u, --update-attr [directory]      recursively update file attributes

 -o, --output [filename|directory]  specify output destination
 -s, --sudo                         request superuser
 -f, --force                        use existing directories and overwrite existing files

 -h, --help                         shows help message and exits
 -v, --version                      prints version information and exits

Usage examples:
 afstool -x DISKIMAGE.adf -o Contents
</pre>

