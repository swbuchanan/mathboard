Installation for Ubuntu
-----------

To install the layout on Ubuntu, one should paste the contents of `math-dvorak` into `/usr/share/X11/xkb/symbols/us`
Copy or move `us` to `/usr/share/X11/xkb/symbols/us`, and copy or move `evdev.xml` to `/usr/share/X11/xkb/rules/evdev.xml`.

Alternatively, you could paste the contents of `math-dvorak` into `/usr/share/X11/xkb/symbols/us` (pretty much anywhere is fine I think), and add the following to `sudo vim /usr/share/X11/xkb/rules/evdev.xml`, near the other English keyboards:

```
<variant>
    <configItem>
        <name>math-dvorak</name>
        <description>English (math Dvorak)</description>
        <vendor>Steven</vendor>
    </configItem>
</variant>
```

