# Devour: X11 Window Swallower

Devour hides your current window before launching an external program and unhides it after quitting.

This fork implements shell aliases out of the box.

## Dependencies

- Xlib (client-side header files)

## Installation

```sh
git clone https://github.com/vulns-are-features-too/devour.git && cd devour && sudo make install
```

## Usage

```sh
devour CMD ...
```

## Pro Tip

**Hint:** If you are one of those unfortunate souls who uses **xdg-open** instead of
[a custom launch script](https://gist.github.com/salman-abedin/6f52c52e465d89d489f9ea8d891c7332),
then go to your **~/.local/share/applications** directory and modify the applications you launch from your file explorer like below and enjoy the true devouring experience.

```
[Desktop Entry]
Type=Application
Name=PDF Reader
Exec=/usr/local/bin/devour /usr/bin/zathura %U
```

## Update

```sh
cd devour
git pull --no-rebase && sudo make install
```

## Uninstallation

```sh
cd devour
sudo make uninstall
```
