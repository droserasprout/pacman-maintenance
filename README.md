# pacman-maintenance

Perform pacman maintenance by timer:

* Download fresh packages, but, IMPORTANT, do not install them
* Remove orphaned packages
* Remove cached packages older than three latest versions
* Cleanup AUR helpers' cache

## Installation

```bash
$ git clone https://github.com/droserasprout/pacman-maintenance.git
$ cd pacman-maintenance; makepkg -si
$ sudo systemctl enable --now pacman-maintenance@$USER.timer
```