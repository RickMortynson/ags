# Aylur's Gtk Shell

This is a library built for [GJS](https://gitlab.gnome.org/GNOME/gjs) to allow defining GTK widgets in a declarative way. It also provides services and other utilities to interact with the system so that these widgets can have functionality.
GJS is a JavaScript runtime built on Firefox's SpiderMonkey JavaScript engine and the GNOME platform libraries, the same runtime [GNOME Shell](https://gitlab.gnome.org/GNOME/gnome-shell) runs on. 

It was heavily inspired by [EWW](https://github.com/elkowar/eww).

Currently, only Wayland is supported, but it also works on X11, [see #19](https://github.com/Aylur/ags/issues/19).

## Get started

To get started read the [wiki](https://aylur.github.io/ags-docs).

### Installation
Instructions were adapted from the [wiki](https://aylur.github.io/ags-docs/config/installation/) to accomodate this fork.
#### From source
```bash
# Arch
sudo pacman -S typescript npm meson gjs gtk3 gtk-layer-shell gnome-bluetooth-3.0 upower networkmanager gobject-introspection libdbusmenu-gtk3 libsoup3 glib2-devel
```
```bash
# Fedora
sudo dnf install typescript npm meson gjs-devel gtk3-devel gtk-layer-shell gnome-bluetooth upower NetworkManager pulseaudio-libs-devel libdbusmenu-gtk3 libsoup3
```
```bash
# Ubuntu
sudo apt install node-typescript npm meson libgjs-dev gjs libgtk-layer-shell-dev libgtk-3-dev libpulse-dev network-manager-dev libgnome-bluetooth-3.0-dev libdbusmenu-gtk3-dev libsoup-3.0-dev
```
```bash
# clone, build, install
git clone --recursive https://github.com/striped-bass/ags.git
cd ags
npm install
meson setup build
meson install -C build
```
#### Running
```bash
ags --help
```
