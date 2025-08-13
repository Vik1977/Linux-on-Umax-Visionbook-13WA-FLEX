# Linux-on-Umax-Visionbook-13WA-FLEX
Family member gave me this laptop, mine has a problematic keyboard, missing 3 keys, so it`s not much usable.

To this time i tried various distro and DE on it:
- Fedora whit [GNOME](https://fedoraproject.org/workstation/), [KDE mobile](https://fedoraproject.org/workstation/), [Phosh](https://puri.sm/posts/phosh-overview/)
- [Linux Mint](https://www.linuxmint.com/)
- [Debian Trixie](https://www.debian.org/) whit [Phosh](https://puri.sm/posts/phosh-overview/), Lomiri

Linux mint is not a so touch friendly environment, so ruled that one out, KDE mobile worked really well and could be a vaild option, vanilla GNOME worked good but it went a bit too heavy on the resources expecially when switchig tabs it would freeze, on the other hand Phosh which is based on GNOME behaved really well, no stutter, good touch support, no lag when logging in and out and well integrated login screen, suspend works well too. To install posh on their page is no documentation to install it because it comes with their own os: PureOS,  
anyway to install it on Fedora just:  
```bash
dnf install phosh
```
and on Debian:  
```bash
apt install phosh
```
Last i tried Lomiri and not a bad expirience after all, i think phosh is more fluid but try it yourself i thisnk they are both really interesting piece of softweare, Lomiri is the DE of Ubuntu touch so too a fork of GNOME, it`s not available on fedora, on Debian 13 just:  
```bash
apt update
```
and
```
apt install lomiri lomiri-desktop-session
```

## During my testing i encountered various problems:

- the trackpad isn`t recognized
- the fingerprint reader doesn`t work
- the automatic orientation of the screen orientates in the opposite way that you hold the device

## And wanted to apply some tweaks:

- make the device switch beetween laptop and tablet mode and disable automatically trackpad,keyboard and power button

## Usecases I came up with:

- use it to disply music notes
- to read books
- use it like tablet to menage my home and homelab trough web interface or app

## Progress:

- [ ] functioning trackpad
- [ ] functioni fingerprint reader
- [ ] fixed reversed rotation
- [ ] disable power button, keyboard and trackpad when in tablet mode


## Collaboration:

I am new to github and dont know how to accept merge request and pushes but i am open and will appriciate any type of help or tip someone wants to share
