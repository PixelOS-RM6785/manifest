# PixelOS

Getting Started
===============

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository, use a command like this:

```bash
repo init -u https://github.com/PixelOS-RM6785/manifest.git -b thirteen
```

Then to sync up:
================

```bash
repo sync -j$(nproc --all)
```

Compilation of PixelOS
======================

From root directory of Project, perform following commands in terminal to start Compilation.

```bash
source build/envsetup.sh
lunch aosp_<devicecodename>-userdebug
make bacon -j$(nproc --all)
```
