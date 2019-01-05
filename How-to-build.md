# Build chocolate-doom

## Install SDL2_net & SDL2_mixer
The easiest is to use the [chocpkg](https://github.com/chocolate-doom/chocpkg) script:

`git clone https://github.com/chocolate-doom/chocpkg`
`cd chockpkg`
`./chockpkg/chockpkg install chocolate-doom`

## Configure chocolate-doom
clone project

cd to project

`autoreconf -fi`

After this, you need to set the PKG_CONFIG_PATH before you try to run configure

`export PKG_CONFIG_PATH=/Users/peter/Programming/C/chocpkg/install/lib/pkgconfig:${PKG_CONFIG_PATH:-}`

Now you can configure, make and install

`./configure`

`make`

or

`make install`

The game is now installed in `/usr/local/bin`

If you want to unstall:

`make uninstall`
