A Qt gui to control and debug my custom BLDC controller. A complete description and tutorial about how to use it can be found here: http://vedder.se/2015/01/vesc-open-source-esc/

Quick build instructions for Ubuntu:

1. sudo apt-get install qtcreator qt-sdk libudev-dev libqt5serialport5-dev

2. qmake

3. make

Windows and OS X builds available :

https://bldc-tool.support


---

#### Troubleshooting:

##### unknown QT: serialport

Full error:

    Project MESSAGE: Warning: unknown QT: serialport
    
You need to use qmake from qt5, (`/usr/lib/x86_64-linux-gnu/qt5/bin/qmake` on ubuntu) in the above steps (step 2).
You'll probably need to also install `qtserialport` from QT Mainainance Tool (a gui program you should have installed) and select "Add or remove components" > Your Qt version > Source Components, Add-Ons > qtserialport.
