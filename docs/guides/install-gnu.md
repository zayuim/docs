## Downloading, Installing and Updating RetroArch

## GNU/Linux

### Flatpak

Flatpak is a distro-agnostic way to install RetroArch across many different GNU/Linux based operating systems. RetroArch currently resides in the FlatHub repository.

First you should ensure that [Flatpak is installed](http://flatpak.org/getting.html). Once installed, open the terminal emulator that came with your distro, and run the following command to see how to use it:

```
flatpak --help
```

Next you should add the Flathub repository, so that it may download from it:

```
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

To install RetroArch execute:

```
flatpak install --from https://flathub.org/repo/appstream/org.libretro.RetroArch.flatpakref
```

To update you should periodcally run

```
flatpak update
```

### Ubuntu-based

The best way to get RetroArch and the corresponding libretro cores on to a Ubuntu-based system is using PPA.

First open the terminal on Ubuntu. You now need to consider which branch you want to use, stable or testing? Stable will give you better stablity at the cost of slower updates, while testing gives you the chance to try features early and get updates quicker.

To add the stable branch to your system type:

```
sudo add-apt-repository ppa:libretro/stable
```

Or if you want the testing version:

```
sudo add-apt-repository ppa:libretro/testing
```

You should now update the repositories:

```
sudo apt-get update
```

And finally install RetroArch:

```
sudo apt-get install retroarch
```

Updating will happen system-wide, to change frequency update checks, you should change this in Ubuntu's software updater settings.

### Arch-based

The Arch repositories contain compiled versions of RetroArch.

You could either install the stable or the git version.

To install stable, execute:

```
sudo pacman -Sy retroarch
```

To install git, execute:

```
yaourt -Sy retroarch-git
```