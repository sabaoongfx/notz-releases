# notz releases

Installers for notz (Windows, macOS, Linux, Android). The source is private.

See the Releases tab for downloads, or [notz's download page](https://notz.web.app/download.html).

## Arch Linux, Manjaro, EndeavourOS (pacman)

A signed pacman repository, so updates arrive with the normal `sudo pacman -Syu`:

```bash
curl -fsSL https://sabaoongfx.github.io/notz-releases/KEY.gpg | sudo pacman-key --add -
sudo pacman-key --lsign-key "notz packages"
printf '\n[notz]\nServer = https://sabaoongfx.github.io/notz-releases/arch/$arch\n' \
  | sudo tee -a /etc/pacman.conf
sudo pacman -Sy notz
```
