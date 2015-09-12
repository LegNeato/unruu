unruu
=====

unruu is a simple command line utility to extract the rom.zip file from a 
HTC RUU update executable.

Please note that it'll output the rom.zip file to your current directory.

Requirements (libunshield v0.9 or higher):
------------------------------------------

    $ git clone https://github.com/twogood/unshield.git
    $ cd unshield/
    $ ./bootstrap
    $ ./configure --prefix=/usr
    $ make
    $ sudo make install

Building:
---------

    $ ./autogen.sh
    $ ./configure
    $ make

Building (Mac OS X):
--------------------

It is easiest to use [Homebrew](http://brew.sh/) for dependencies.

    $ brew install autogen libgcrypt
    $ brew install unshield
    $ ./autogen.sh
    $ export LDFLAGS='-L/usr/local/Cellar/unshield/1.0/lib/'
    $ ./configure
    $ make

Installing:
-----------

    $ sudo make install

Using:
------

    $ unruu /path/to/RUU.exe
