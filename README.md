# README

This is KDbg, a graphical user interface around GDB using
KDE, the K Desktop Environment.

To build and install:

	cmake .
	make
	sudo make install

It may be necessary to tell the install location explicitly,
then use, for example,

	cmake -DCMAKE_INSTALL_PREFIX=/usr .

The KDE header files libraries must be available. Make sure
that the development packages are installed.

The homepage is at

	http://www.kdbg.org/

Johannes Sixt <j6t@kdbg.org>

# Build
These build steps worked for me.

```
sudo apt install cmake-extra extra-cmake-modules
sudo apt install libkf5iconthemes-dev libkf5xmlgui-dev
sudo apt install gettext xterm
git clone https://github.com/chucktilbury/kdbg.git
cd kdbg/
git tag -l
git checkout kdbg-3.0.1
mkdir build; cd build
cmake ..
make
sudo make install
```
