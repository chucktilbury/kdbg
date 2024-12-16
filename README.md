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
sudo apt install libkf5iconthemes-dev libkf5xmlgui-dev kde-config-gtk-style
sudo apt install gettext xterm extra-cmake-modules breeze-gtk-theme breeze-cursor-theme
git clone https://github.com/chucktilbury/kdbg.git
cd kdbg/
git tag -l
git checkout kdbg-3.0.1
mkdir build; cd build
cmake ..
make
sudo make install
```
In addition to these build steps, I also installed the "breeze" icons for Plasma to mitigate a runtime warning.
