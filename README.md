# PKGS
###### Da One Thicc Solution (for my arch local package management)

### Usage
put this `/etc/pacman.conf` snippet to connects this live repo to your arch sysetm
```
[personal]
SigLevel = PackageOptional DatabaseOptional
Server = https://raw.githubusercontent.com/RaafatTurki/pkgs/master/repo/$arch
```
or this one to connects a local version of it
```
[personal]
SigLevel = PackageOptional DatabaseOptional
Server = file:///path/to/pkgs/repo/$arch
```
follow the above with a system update
```bash
pacman -Syu
```
and that's all, you should be able to install whatever is hosted here via `pacman`


### Managment
```bash
repo_manager
```
builds everything in `pkgfiles`, stores them `repo`, then builds its database files
