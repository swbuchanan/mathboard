# todo: I don't think this stuff is right

Using Ubuntu
-----------

Add it to your systems keyboard and restart your computer.

```
cp math-dvorak >> ~/.config/xkb/math-dvorak
```

I think instead what one should do is paste the contents of math-dvorak into `/usr/share/X11/xkb/symbols/us`

Then you have to update the `sudo vim /usr/share/X11/xkb/rules/evdev.xml` with the following, add it near the other English keyboards

```
<variant>
    <configItem>
        <name>math-dvorak</name>
        <description>English (Math Dvorak)</description>
        <vendor>Steven</vendor>
    </configItem>
</variant>
```

