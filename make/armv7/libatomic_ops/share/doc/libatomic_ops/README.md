[![cogroid.com](https://github.com/cogroid/resources/raw/main/images/banner/cogroid-48.png)](https://cogroid.com)

# A library for atomic operations

### Packages on Ubuntu 18.04

* [libatomic-ops-dev (7.6.2-1)](https://packages.ubuntu.com/bionic/libatomic-ops-dev)
* [Source Package: libatomic-ops (7.6.2-1)](https://packages.ubuntu.com/source/bionic/libatomic-ops)

### Prerequisites

###### build-essential

```
sudo apt-get install build-essential
```

###### GLIBC == 2.27

```
ldd --version
```

* Ubuntu 18.04

###### GCC 32 bit

```
sudo apt install gcc-multilib

sudo apt install g++-multilib
```

###### NDK r18b

* [NDK Downloads](https://developer.android.com/ndk/downloads)
* [NDK r18b for Linux](https://dl.google.com/android/repository/android-ndk-r18b-linux-x86_64.zip)

```
Unzip to folder /home/cogroid/local/android-ndk-r18b
```

###### clang

```
sudo apt install clang
```

### Build for x64 machine

```
sudo apt update
cd ${AO_DIR}/make/x64
make > build.log&
```

```
sudo apt update
cd ${AO_DIR}/make/x64
make install
```

```
Built files are at /home/cogroid/local/libatomic_ops/x64
```

### Build for i386 machine

```
sudo apt update
cd ${AO_DIR}/make/i386
make > build.log&
```

```
sudo apt update
cd ${AO_DIR}/make/i386
make install
```

```
Built files are at /home/cogroid/local/libatomic_ops/i386
```

### Build for armv7-a machine

```
sudo apt update
cd ${AO_DIR}/make/armv7
make > build.log&
```

```
sudo apt update
cd ${AO_DIR}/make/armv7
make install
```

```
Built files are at /home/cogroid/local/libatomic_ops/armv7
```

---
[Head icons created by Freepik - Flaticon](https://www.flaticon.com/free-icons/head)
