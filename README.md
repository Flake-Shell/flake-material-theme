# Flake Material GTK
> **Important**: `flake-material-gtk` is a fork of [SakibShahariar/material-gnome-theme](https://github.com/SakibShahariar/material-gnome-theme), but we are not affiliated with, endorsed by, or sponsored by the original author.

## 📦 Debian Package

Build and install the package from a repository checkout:

```bash
sudo apt install debhelper dpkg-dev
dpkg-buildpackage -b -us -uc
sudo apt install ../flake-material-gtk_*_all.deb
```

The theme is installed to `/usr/share/themes/flake-material-gtk`. GTK4/libadwaita apps also need its stylesheets linked into your config directory:

```bash
mkdir -p ~/.config/gtk-4.0
for f in gtk.css gtk-dark.css colors.css; do
  ln -sf /usr/share/themes/flake-material-gtk/gtk-4.0/$f ~/.config/gtk-4.0/$f
done
```


## 📜 License

This project is licensed under the **GPL-3.0 License** - see the [LICENSE](LICENSE) file for details.
