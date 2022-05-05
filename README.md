# en_SE
fork of https://github.com/u296/en_SE with "," as a decimalpoint seperator instead of "."

## Steps

First, put the file `en_SE` into the directory `/usr/share/i18n/locales`. Now you can generate the locale file.
To do this, write the line `en_SE.UTF-8 UTF-8` somewhere in the file `/etc/locale.gen` and run `sudo locale-gen` Finally, to select the 
locale, either do it through the GUI or write `LANG=en_SE.UTF-8` in the file `/etc/locale.conf`.

Now, to fix key composing, add the line `en_US.UTF-8/Compose: en_SE.UTF-8` to the file `/usr/share/X11/locale/compose.dir`

Det borde funka nu :D
