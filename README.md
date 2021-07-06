# amigatools

Minimal Commodore Amiga software scripts for GNU/Linux.

## Dependencies

sh, bash, affs filesystem support (Linux kernel)

## Scripts

- `arcadf <source> <zip basename>`
	- Create a zip archive from an Amiga .adf floppy image
	- Depends on `extractadf` and `zipdir`
- `extractadf <source> <dest>`
	- Extract contents of an Amiga .adf floppy image
- `zipdir <source>`
	- Create an archive from a directory and delete the original directory