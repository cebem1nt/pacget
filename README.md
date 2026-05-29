# Pacget

Tiny af AUR helper. Lets you download, search for PKGBUILDS and more things. **Doesn't mix AUR packages and oficial arch packages**

## Usage

```
pacget <name>
```

Need to clone more than one? 
```
pacget <name 1> <name n>
```

Clone, and pull all the PKGBUILD dependencies?
```
pacget -p hyprland-git
```

Clone, install automatically, and pull dependencies?
```
pacget -pi hyprland-git
```

Install but check the PKGBUILD content for anything malicious before?
```
pacget --safe-mode -i browsh-bin
```

Clone to exact directory?
```
pacget <name 1> <name 2> --dest <dir 1> <dir 2> 
```

Searching?
```
pacget -s zen qt5  
```

Clone PKGBUILDS to a specific directory by default?
```
pacget --storage-dir=~/.local/src/ waybar-git
```

## Misc
```
usage: pacget [-h] [-d DIR [DIR ...]] [-s] [-b [{name,name-desc,maintainer,depends,makedepends,optdepends,checkdepends}]] [-i] [-f] [-p] [--brief] [--safe-mode]
              [--storage-dir DIR]
              names [names ...]

Search & Get PKGBUILD's from Arch User Repository

positional arguments:
  names                 Name[s] of PKGBUILD[s] to search for

options:
  -h, --help            show this help message and exit
  -d, --dest DIR [DIR ...]
                        Optional directories where to clone to
  -s, --search          Search for PKGBUILD[s] instead of cloning.
  -b, --by [{name,name-desc,maintainer,depends,makedepends,optdepends,checkdepends}]
                        An attribute to search by
  -i, --install         After clonning, automatically install
  -f, --force           Do not check if PKGBUILD[s] exist[s], forcefully clone
  -p, --pull-deps       Pull dependency PKGBUILD[s] as well
  --brief               If searching, do not output additional info (description, version)
  --safe-mode           if -i is provided, print the content of PKGBUILD and prompt for continuation
  --storage-dir DIR     Default directory where to clone to
```
