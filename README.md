# build-nodejs-for-android-perfectly-on-Linux
build NodeJS for android perfectly(without disable nor change anything) on Linux

**`perfectly` means do not add any `--without-...` option, nor modifying any source (include build settings)**

[NodeJS](https://github.com/nodejs/node): 6.3.1-6.5.0

Linux Ubuntu 16.04, NDK 12.1.29

I'v made a tool [android-gcc-toolchain](https://github.com/sjitech/android-gcc-toolchain) 
to use NDK toolchain easily and do some hack to overcome some common mistaken of cross-compile settings.

So the build commands are:

- arm64

    ```
    android-gcc-toolchain arm64 --hack -C <<< "./configure --dest-cpu=arm64 --dest-os=android && make"
    ```

- arm

    Under test

- x86

    Under test

- x64

    Under test

See also: [build-nodejs-for-android-perfectly-on-Mac](https://github.com/sjitech/build-nodejs-for-android-perfectly-on-Mac)

Good luck.
