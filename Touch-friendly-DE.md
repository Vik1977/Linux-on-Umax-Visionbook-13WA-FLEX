# Those are the Desktop Environments that I tried on the IMAX Vision book 13w FLEX

To this time i tried various distro and DE on it:
- Fedora whit [GNOME](https://fedoraproject.org/workstation/), [KDE mobile](https://fedoraproject.org/workstation/), [Phosh](https://puri.sm/posts/phosh-overview/)
- [Linux Mint](https://www.linuxmint.com/)
- [Debian Trixie](https://www.debian.org/) whit [Phosh](https://puri.sm/posts/phosh-overview/), Lomiri

Linux mint WITH cinnamon is not a so touch friendly environment, so ruled that one out, KDE mobile worked really well and could be a vaild option, vanilla GNOME worked good but it went a bit too heavy on the resources expecially when switchig tabs it would freeze, on the other hand Phosh which is based on GNOME behaved really well, no stutter, good touch support, no lag when logging in and out and well integrated login screen, suspend works well too. To install posh on their page is no documentation because it comes with their own os: PureOS,  
anyway to install it on Fedora just:  
```bash
dnf install phosh
```
and on Debian:  
```bash
apt install phosh
```
Last i tried Lomiri and not a bad expirience after all, i think phosh is more fluid but try it yourself i think they are both really interesting pieces of software, Lomiri is the DE of Ubuntu touch so a fork of GNOME too, it`s not available on fedora, but on Debian 13 just:  
```bash
apt update
```
and
```
apt install lomiri lomiri-desktop-session
```
