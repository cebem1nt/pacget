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
usage: pacget [-h] [-d DIR [DIR ...]] [-s] [-sb [{name,name-desc,maintainer,depends,makedepends,optdepends,checkdepends}]] [-i] [-f] [-p] [-b] [--safe-mode] [--storage-dir DIR]
              [names ...]

Search & Get PKGBUILD's from Arch User Repository

positional arguments:
  names                 Name[s] of PKGBUILD[s] to search for

options:
  -h, --help            show this help message and exit
  -d, --dest DIR [DIR ...]
                        Optional directories where to clone to
  -s, --search          Search for PKGBUILD[s] instead of cloning.
  -sb, --search-by [{name,name-desc,maintainer,depends,makedepends,optdepends,checkdepends}]
                        Search for PKGBUILD[s], takes search by param
  -i, --install         After clonning, automatically install
  -f, --force           Do not check if PKGBUILD[s] exist[s], forcefully clone
  -p, --pull-deps       Pull dependency PKGBUILD[s] as well
  -b, --brief           If searching, do not output additional info (description, version)
  --safe-mode           if -i is provided, print the content of PKGBUILD and prompt for continuation
  --storage-dir DIR     Default directory where to clone to
```
