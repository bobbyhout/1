Here you have all dependencies that you need to install for an optimal utilisation on Linux MInt/Ubuntu and Manjaro too.

                              # Installation software on Linux Mint/Ubuntu (and all Ubuntu derivated)

First, you must install all softwares asked for getting a full installation, Here the list :

* swig/swig2.0
* doxygen/doxypy
* cmake
* libunittest-dev
* python3-pyqt5
* python3-pyqt5.qtsql
* python3-pyqt5.qtquick
* python3-pyqt5.qtopengl
* python3-pyqt5.qtsvg
* python3-pyqt5.qtxmlpatterns
* python3-pyqt5.qtmultimedia
* python3-pyqt5.qtwebkit
* python3-simplejson
* build-essential
* qt5-default
* qt5-qmake
* libmagick++5 (wil install libmagickcore5/libmagickwand5/liblqr-1.0)
* libsdl1.2debian
* libxcursor1
* libxinerama1
* libasound2
* libqt5svg5
* libavformat54
* libavcodec54
* libavocdec-extra-54
* libavutil52
* libavutil-extra-52
* libswscale2
* libavdevice53
* libpostproc52
* libavfilter3
* libpython3

After, you must install all dev version of those and even more, Here the list :

* libsdl1.2-dev
* libxcursor-dev
* libxinerama-dev
* libasound2-dev
* python3-all-dev
* pyhton3-dev
* libpython3-all-dev
* libqt5svg5-dev
* libavformat-dev
* libavcodec-dev
* libswscale-dev
* libavdevice-dev
* libavutil-dev
* libavfilter-dev
* libmagick++5-dev (will install libmagickcore-dev/libmagickwand-dev)


Note : using Synaptic, you can search by keywords like libmagick++5 or libpython will install you some others dependencies.

Note : you can get/download a document explaining all dependencies needed for all systems i.e Linux, Windows, Mac here : http://bazaar.launchpad.net/~openshot.code/libopenshot/trunk/files/head:/doc/ .

                          # Installation software on Manjaro (Archlinux derivated)

On this kind of system you don't need the dev version because they are compiled sytems.

Here the list :

* libavformat
* libavcodec
* libavutil
* libavdevice
* libswscale
* libmagick++
* libmagickwand
* libmagickcore
* libsdl2
* libqt5
* cmake
* swig
* doxygen
* libunittest++
* qt5-default
* qtbase5-dev
* qtbase5-dev-tools
* qt5-qmake
* qtmultimedia5-dev
* python3-dev
* libxinerama
* libxcursor
* libasound
* qt5-multimedia
* qt5-svg
* qt5-tools
* qt5-webkit
* python-pyqt5
* pyqt5-common
* python-pytools
* doxypy/doxygen
* python-simplejson
* qt5-base
* python-opengl
* python-dbus
* qt5-xmlpatterns
* qt5-declarative
* qt5-serialport
* qt5-imageformats (previously in two packages qt5-image and qt5-formats)
* qt5-doc
* qt5-location
* qt5-translations

The following step is to compile libopenshot-audio and AFTER libopenshot

### Compile libopenshot-audio

1. mkdir build if not already done
2. cd build
3. cmake ..
4. make
5. sudo make install
6. openshot-audio-test-sound

### Compile libopenshot

1. mkdir build
2. cd build
3. cmake ..
4. make (-DCMAKE_PREFIX_PATH/usr/lib64/qt/5,2,1-1/ ../
5. sudo make install