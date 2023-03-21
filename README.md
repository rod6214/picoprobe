# Picoprobe
Picoprobe allows a Pico / RP2040 to be used as USB -> SWD and UART bridge. This means it can be used as a debugger and serial console for another Pico.

# How to compile for Windows and MSYS2
To complete the following instructions we recommend to open up a MSYS2 command pront in x64 mode.
- Configure SDK pico path and:

    ```
    set PICO_SDK_PATH=C:\Develop\RaspberryProjects\pico-sdk
    ```

- Set the route path of Python 3 you can download it [here](https://www.python.org/downloads/release/python-390/). Note: don't use installer instead download .zip then you can put in in the root of your preference.
    ```
    set path=%path%;C:\Python3\python-3.9.0-embed-amd64
    ```
- Clone picoprobe repository make it.
    ```
    git clone --recurse-submodules https://github.com/raspberrypi/picoprobe.git 
    cd picoprobe 
    mkdir build 
    cd build 
    Cmake -G “Unix Makefiles” .. 
    make
    ```

# Documentation
Picoprobe documentation can be found in the [Pico Getting Started Guide](https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf). See "Appendix A: Using Picoprobe".
