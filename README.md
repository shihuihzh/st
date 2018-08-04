### st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


### Requirements
------------
In order to build st you need the Xlib header files.

### Patches
------------
Base on version v0.8.1. Add some patches from [https://st.suckless.org/patches/](https://st.suckless.org/patches/)

1. alapha
2. dracula
3. scrollback
4. xresources

### Key Bind
------------
* Copy change to `Ctrl` + `Insert`
* Paste chate to `Shift` + `Insert`
* Scroll use `Shift` + `Up/Down` or `Shift` + mouse wheel


### Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


### Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

### Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

Add patch by Howe Huang
