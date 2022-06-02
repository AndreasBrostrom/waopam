# WAOPAM
WIndows all in One PAckage Manager or WAOPAM for short are a package manager wrapper that will simplyfy the life for windows users. The wrapper will make sure you can use all package managers in windows via one terminal experience simplyfying the hassel.

## Install
TBD

## Integrated package managers 
- [scoop](https://scoop.sh/)
- [chocolatey](https://chocolatey.org/)
- [winget](https://apps.microsoft.com/store/detail/appinstallationsprogram/9NBLGGH4NNS1?hl=sv-se&gl=SE)

## Usage
```bat
waopam install sudo         # installs sudo program from scoop
waopam -S sudo              # installs sudo program from scoop pacman style
```

```bat
waopam search git
waopam git
```

waopam update               # updates database

```bat
waopam upgrade
waopam upgrade git          # Updates git only
```

```bat
waopam install git --choco  # install global using chocolatey
waopam install git --winget # install global using winget
waopam install git --user   # install for user from scoop
waopam install git          # install globaly using scoop
waopam -S git               # install globaly using scoop pacman style
```

## Package manager install priority order
Priority of installations are using the following priority order with some exceptions.

1. scoop  (Portable and terminal tools (sudo, rufus and git for instance))
1. winget
1. choco