st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.


Changes made by Dhanus
---------------------
1. Applied the [colorschemes patch](https://st.suckless.org/patches/colorschemes/).
2. Applied the [scrollback patch](https://st.suckless.org/patches/scrollback/).
3. Changed the scrollback binding to `shift+ctrl+j/k`.
4. Changed the fontsize change binding to `ctrl+ +/-`.


Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

