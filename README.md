# surf
My custom build of suckless terminal v0.9

## Patches applied

* st-alpha
* st-scrollback-ringbuffer
* st-scrollback-mouse
* st-scrollback-mouse-altscreen
* st-font2
* st-externalpipe (for the scripts used by this patch see my [dotfiles](https://github.com/fabioesantos/Dotfiles).
* st-boxdraw
* st-ligatures

## st - simple terminal

st is a simple terminal emulator for X which sucks less.


## Requirements

In order to build st you need the Xlib and Harfbuzz header files.


## Installation

Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
