# Pacget

Tiny AUR helper. Just lets you download and search for PKGBUILDS

## Usage

Checks if requested PKGBUILD exists, and clones it to `rofi-git` directory
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
usage: pacget [-h] [-s] [-f] [-d DIR [DIR ...]] [names ...]

Search & Get PKGBUILD's from Arch User Repository

positional arguments:
  names                 Names of PKGBUILD[s] to get/search for

options:
  -h, --help            show this help message and exit
  -s, --search          Search for name[s] of packages instead of installing
  -f, --force           Do not check if PKGBUILD with given name exists, forcefully clone
  -d, --dest DIR [DIR ...]
                        Optional directories where to clone PKGBUILD[s] to
```
