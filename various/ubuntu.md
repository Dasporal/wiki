# Ubuntu

Various stuff about Ubuntu

## Problem : 2nd screen in portrait mode not displaying correctly, even while using nouveau instead of nvidia

Happened on a fresh Ubuntu installation.

**Solution**

Use ```xrandr``` to get a detailed view of all your screens.

Then use the following command to configure.

```console
$ xrandr --output [screen-name] --mode [resolution] --rotate [normal|right|left]
```

Example : 

```console
$ xrandr --output HDMI-0 --mode 1920x1080 --rotate right
```
