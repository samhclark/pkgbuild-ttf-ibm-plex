# pkgbuild-ttf-ibm-plex
Arch Linux PKGBUILD for IBM's font called Plex

Don't use this. 
It's part of `extra`, so it's managed by Arch already.

## Development

It's pretty easy to test it out.
Run the following in this directory: 
```shell
makepkg
```

That should produce a file like `ttf-ibm-plex-${pkgver}-1-any.pkg.tar.zst`. 

You can inspect the contents of that file with 
```shell
pacman -Qlp *.zst
```

## Installation

You can install the fonts by building the package and then installing it with pacman.

```shell
makepkg
sudo pacman -U ttf-ibm-plex-${pkgver}-1-any.pkg.tar.zst
```