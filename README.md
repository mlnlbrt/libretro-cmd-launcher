# libretro-cmd-launcher

This is a VERY quick-and-dirty way to launch non-libretro games/apps directly from Retroarch, especially useful in Lakka.

Based on Rob Loach's [libretro-dolphin-launcher](https://raw.githubusercontent.com/RobLoach/libretro-dolphin-launcher).

## How to use

Just create a .sh file like this and launch it in Retroarch using "libretro-cmd-launcher" core:
``` bash
#!/bin/sh

systemctl stop retroarch

cd /storage/your/app/directory
./your-app-binary
systemctl start retroarch

```
