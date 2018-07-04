# binaryanalysis-ng
Binary Analysis Next Generation (BANG)

BANG is a framework for unpacking files (like firmware) recursively and running checks on the unpacked files. Its intended use is to able to find out the provenance of the unpacked files and classify/label files, making them available for further analysis.

## Requirements:

* a recent Linux distribution (Fedora 26 or higher, or equivalent)
* Python 3.6.x or higher
* netpbm-progs
* pillow (drop in replacement for PIL, http://python-pillow.github.io/ )
* GNU binutils (for 'ar')
* squashfs-tools (for 'unsquashfs')
* cabextract

## Invocation

    $ python3 bang-scanner -c bang.config -f /path/to/binary
