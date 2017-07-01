**Note:** Srain is still under development.

## Dependencies

- make          (makedepends)
- gcc           (makedepends)
- pkg-config    (makedepends)
- gettext       (makedepends)
- imagemagick   (makedepends)
- gtk >= 3.16
- python >= 3.2
- libcurl
- libnotify
- libconfig

## Build & Debug

    mkdir build
    ./configure --prefix=$PWD/build --config-dir=$PWD/build/etc --enable-debug
    make
    make run

## Install

### Arch Linux

    yaourt -S srain-git # git version
    yaourt -S srain     # latest release

or:

    # Add archlinuxcn mirror, then
    pacman -S archlinuxcn/srain-git

### Gentoo

Look at the [Install Guide](https://github.com/rtlanceroad/gentoo-srain)

### For Other Linux Distributions

    # Intall the above dependencies, then
    # Note: the configure script doesn't check dependiencies.
    mkdir build
    ./configure --prefix=/usr/local --config-dir=/etc --disable-debug
    make
    make DESTDIR=/ install

## Feature

- Beautiful User Interface
- Relay bot message transform
- Preview image from URL
- Get avatar according to user's real name (plugin)
- Auto upload image to pastebin (plugin)

## Screenshot

As you see, its theme is inspired by Telegram Desktop.

![screenshot](http://img.tjm.moe/47/ceece073d29563da0c22ab6e8e8c3cdc534113.png)

## Need Help?

Feel free to contact me if you have any question about srain.

- **IRC Channel**: [#srain](irc://irc.freenode.net/srain) @ freenode
- Email: silverrainz at outlook dot com
- Github: file an issue [Here](https://github.com/SilverRainZ/srain/issues)

## License

GNU General Public License Version 3
