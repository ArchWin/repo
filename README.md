# ArchWin Repository
Pacman repository with some packages.

## Adding it.
You can add ArchWin to your system (it has nothing for you though). Just run the following commands:

```css
sudo pacman-key --recv-keys FE2A530C7559974F84829978A55CD2880240ABD7 --keyserver keyserver.ubuntu.com
sudo pacman-key --lsign-key FE2A530C7559974F84829978A55CD2880240ABD7
sudo pacman -U 'https://archwin.github.io/repo/x86_64/archwin-keyring-20230702-1-any.pkg.tar.zst'
```
Append (adding to the end of the file) to `/etc/pacman.conf`:
```ini
[archwin]
Server = https://archwin.github.io/repo/$arch
```
