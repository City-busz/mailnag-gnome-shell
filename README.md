# mailnag-gnome-shell
Mailnag GNOME-Shell extension.

#### Features
* Notifies about new mails via the messaging tray (including a counter badge).
* Shows an indicator in the top panel (including counter badge and popup menu).

## Installation
This extension requires the [Mailnag daemon](https://github.com/pulb/mailnag).  
Prior to installation, run `mailnag-config` and ensure that the *libnotify* plugin is disabled.

### Arch Linux
The extension is available in the [AUR](https://aur.archlinux.org/packages/mailnag-gnome-shell/) repository.  
Please either run `yaourt -S mailnag-gnome-shell` or `packer -S mailnag-gnome-shell` (as root) to install the package.

### Generic Tarballs
Distribution independent tarball releases are available [here](https://github.com/pulb/mailnag-gnome-shell/releases).  
To install the extension type the following commands in a terminal (root is *not* required):

	tar xvf mailnag-gnome-shell-*.tar.gz
	cd mailnag-gnome-shell-*
	make install-local

That's it. Now fire up `gnome-tweak-tool` and enable the extension.  

###### Requirements
* vala (at compiletime only)
* libfolks
* mailnag

## Screenshots
![Screenshot](https://raw.github.com/pulb/mailnag-gnome-shell/docs/docs/screenshots/mailnag-gnome-shell.png)