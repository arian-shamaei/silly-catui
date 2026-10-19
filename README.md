[![downloads](https://img.shields.io/github/downloads/arian-shamaei/silly-catui/total)](https://github.com/arian-shamaei/silly-catui/releases)

Meow meow meow meow meow meow meow meow meow meow meow? silly-catui meow meow meow meow sillycat meow meow meow.  Meow meow meow meow meow meow meow meow sillyness meow 10x!

**Build and install**

    make            # detects the platform and builds ./meow
    make install    # installs to /usr/local if writable, else ~/.local
    make info       # show what was detected
    make run        # build and run

Platform is detected rather than configured. macOS builds with clang; Linux
builds with gcc and adds `-D_DEFAULT_SOURCE`, which glibc needs to expose the
ioctl declarations under `-std=c11`. An explicit `CC=` or `PREFIX=` always wins.

The install prefix falls back to `~/.local` when `/usr/local/bin` is not
writable, so `make install` works on shared machines without root.

**Usage**
- `meow`
- Debug overlay: `meow --debug`
- Fit mode: `meow --fit=contain` (default) or `meow --fit=cover`
- Pixel mode: `meow --pixel-mode=auto|braille|half|full` (default: auto)


                                          ⡀
                                                 ⣠⣀⡀     ⡠⠊⣲  ⣀⡤⠂⠲⡀
                                                 ⣺ ⠈⠒⠦⣀⡠⠊  ⠊⠈⠈⣀⡢  ⡆
                                                 ⠸⡀   ⠈     ⠈⠈    ⡆
                                                  ⡆    ⡠⠤⣤⡀  ⢠⣂⠲⡄ ⡆
                                                ⣀⣀⣸⡀  ⢰⣶⡀ ⠂  ⢸⣾⡀⠸⡀⣆
                                                ⠈⠢⡀   ⠸⠾      ⠚⠂  ⢨
                                      ⣀  ⡠⡀      ⢠⡂⡀⣀⡀     ⡀⡠⣀⡀ ⣀⡠⠂
                                     ⣠⠺⡀⢀⠂⣆       ⠈⠈⠸⣚⠒⠂   ⠈   ⣈⡌
                                     ⡸⡀⢢⣸ ⠈⣆        ⠠⠮⣠    ⣀  ⠈⢦⡐⡲⠦⡀⣀⡀
                                     ⣆  ⠂  ⠈⢢⡀       ⢀⡎    ⠈⠢⣈⣪⠈⡀    ⠈⡆
                                     ⢸⡀      ⠈⠲⠦⡤⣀⣀⡀⡠⠂       ⠈⠲⣂⡈⠒⠲⠲⠲⠊
                                      ⢢⡀           ⣸     ⠈⠲⣤⣀⡀⣀⡨
                                       ⣈⣢⡀⡀        ⣺           ⡆
                                       ⠈⠪⣈⡀        ⡎    ⡊⠂⣆    ⢸⡀
                                          ⠈⠈⠒⠲⠢⠦⠒⡀⢠⠂    ⡆ ⢸     ⡆
                                                 ⢠⠂     ⡂ ⡆    ⣰
                                                 ⠨⠂⡀   ⡰  ⡂   ⣠⠂
                                                   ⠈ ⠒⠊   ⠲⠤⣀⠠⠂
