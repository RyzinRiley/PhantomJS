## Installation Instructions
-------------

System requirements:

  * C++ toolchain such as `g++` 7 or later
  * CMake version 3.5 or later
  * Qt 5 toolkit
  * Community QtWebKit version 5.212 or later
  * Python 2.7 (to run the tests)


### Installation on Linux
---------------------

Due to the required QtWebKit >= 5.212, only the following distributions will
be supported:

  * Debian 10 (buster) or later
  * Ubuntu 18.04 (bionic) or later
  * Fedora 28 or later

#### On Debian/Ubuntu, the requirements can be fulfilled by installing these packages:

```console
  sudo apt install g++ cmake qt5-default libqt5webkit5-dev python
```

After unpacking the source tarball or cloning the repository:

```console
  ./configure && make
```

Do a quick sanity check:

```console
  ./bin/phantomjs --version
```

Run the test suite:

```console
  make check
```

Install it (may require `sudo`):

```console
  make install
```

### Installation on Windows
-----------------------

Only MinGW is supported for now.

First, install MSYS2

Then, from the "MYS2 MinGW64 32-bit" shell, install the required packages:

```console
  pacman -S msys/make
  pacman -S mingw32/mingw-w64-i686-toolchain
  pacman -S mingw32/mingw-w64-i686-cmake
  pacman -S mingw32/mingw-w64-i686-qtwebkit
  pacman -S mingw32/mingw-w64-i686-python2
```

Note: add `--disable-download-timeout` as an additional argument, if the
installation failed due to the slow server responses.

After unpacking the source tarball or cloning the repository:

```console
  cmake . -G "MinGW Makefiles"
```

And then start the build process:

```console
  make
```

Do a quick sanity check:

```console
  ./bin/phantomjs.exe --version
```

##### Installation on macOS
---------------------

To be written. Likely using `brew`

