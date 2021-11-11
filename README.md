PnF-OS
===========

Getting started
---------------

First of All follow this [guide](https://github.com/PnF-OS/docs/blob/main/env-setup.md) to setup your Build Environment. Then follow the steps below.

Initialzing ROM Sources:
-------------------------
```bash
repo init -u https://github.com/PnF-OS/manifest -b v1.0
```
or alternatively you can use the --depth argument as shown below to shallow clone the repo to save up some space
```bash
repo init --depth=1 -u https://github.com/PnF-OS/manifest/ -b v1.0
```
Syncing Sources:
------------------
 
Enter the Below command to Sync the sources this may take a long time depending on your internet connection
```bash 
 repo sync -j$(nproc --all) --force-sync --no-tags --no-clone-bundle
```
Alright now you are all set. Now sync your device sources and start building. Good luck.
