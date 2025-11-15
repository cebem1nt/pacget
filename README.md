# Pacget

Tiny AUR helper. Just lets you download and search for PKGBUILDS

## Usage

```
$ pacget <name> 
```

Need to clone more than one? 
```
$ pacget <name 1> <name n>
```

Want to clone to exact directory?
```
$ pacget <name 1> <name 2> --dest <dir 1> <dir 2> 
```

Searching?
```
$ pacgtet -s zen qt5  
```

## Misc
```
pacget --help
usage: pacget [-h] [-d DIR [DIR ...]] [-S DIR] [-i] [-f] [-s] [-v] [-D] [names ...]

Search & Get PKGBUILD's from Arch User Repository

positional arguments:
  names                 Name[s] of PKGBUILD[s] to search for

options:
  -h, --help            show this help message and exit
  -d, --dest DIR [DIR ...]
                        Optional directories where to clone to
  -S, --storage-dir DIR
                        Default directory where to clone to by default
  -i, --install         After clonning, automatically install
  -f, --force           Do not check if PKGBUILD[s] exist[s], forcefully clone
  -s, --search          Search for PKGBUILD[s] instead of cloning
  -v, --version         If searching, also print version
  -D, --detailed        If searching, print more detailed information (Description, souce URL)
```
