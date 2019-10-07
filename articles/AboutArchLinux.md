 
---

![alt text](https://www.archlinux.org/static/logos/archlinux-logo-light-90dpi.d36c53534a2b.png "ARCH LINUX")

---

## ABOUT : 
Arch linux is a linux distribution made for computers based on x86-64 architectures developed by [Aaron Griffin and his team](https://www.archlinux.org/people/developers "team info") . It is composed of both **free and non-free open source software**, which means it supports community involvement.

The design principle that is followed by it's development team is __KISS__ ("keep it simple and stupid."). As the general guideline; it focuses on the following:
+ elegance
+ code correctness
+ minimalism  
+ simplicity  
and in return, they expect the user to understand the system's operation. 

Arch uses a rolling release model which means that there is no "_major release_" of new versions of the system; a regular sytem update is required to obtain the latest Arch software; the installation images released by the team are simply up-to-date snapshots of the main system components.

---

## HISTORY:

Inspired by [CRUX](https://en.wikipedia.org/wiki/CRUX), another minimalist distribution, Judd Vinet started the Arch Linux project in March 2002. The name was chosen because Vinet liked the word's meaning of "the principal," as in "arch-enemy".

Originally only for 32-bit x86 CPUs, the first x86_64 installation ISO was released in April 2006.

Vinet led Arch Linux until 1 October 2007, when he stepped down due to lack of time, transferring control of the project to Aaron Griffin.

The end of i686 support was announced in January 2017, with the February 2017 ISO being the last one including i686 and making the architecture unsupported in November 2017. Since then, the community derivative Arch Linux 32 can be used for i686 hardware.

---

![alt text](https://4.bp.blogspot.com/-VNbuQfZFT_o/U1nM9yZsufI/AAAAAAAAKGE/tR9Gd3PwIQQ/s1600/Screenshot+from+2014-04-25+09:47:59.png " cli view of arch system info")

---

## PACKAGE MANAGEMENT:
Arch linux's only supported binary platform is x86_64. The Arch package repositories and User Repository (AUR) contain 58,000 binary source packages, which comes close to [Debian](https://en.wikipedia.org/wiki/Debian "more info about Debian") distribution which has almost 68,000 packages;   

However, the two distributions' approaches to packaging differ, making direct comparisons difficult. The Arch User Repository also contains a writerperfect package which installs several document format converters, while Debian provides each of the more than 20 converters in its own subpackage.

### PACKAGE MANAGER:
To facilitate regular package changes, [pacman](https://wiki.archlinux.org/index.php/pacman "pacman info") (The Arch Package Manager, its name a contraction of "package manager") was developed by [Judd Vinet](https://www.linux.com/news/interview-judd-vinet-arch-linux/ "Judd Vinet interview") to provide Arch with its own package manager able to track dependencies. It is written in C.

All packages are managed using the pacman [package manager](https://en.wikipedia.org/wiki/Package_manager "package manager"). Pacman handles package installation, upgrades, removal, and downgrades, and features automatic dependency resolution. The packages for Arch Linux are obtained from the Arch Linux package tree and are compiled for the x86-64 architecture. It uses binary packages in the tar.xz format, with .pkg placed before this to indicate that it is a pacman package (giving .pkg.tar.xz).

---
![alt text](https://i.ytimg.com/vi/Ac-T4VNss0g/maxresdefault.jpg " cli view of arch system info")

---

## REPOSITORIES:
The official binary Repositories existing are,

+ CORE, which contains all the the basic essential packages for setting up a "Base System".
+ EXTRA, which contains packages other than Core Packages, Desktop Environment and Programs.
+ COMMUNITY, which contains packages created by the community and mostly accepted by the trusted community users.
+ MULTILIB, it's a concentrated repository for x86-64 users to reliabily support 32-bit applications in a 64-bit environment.

Except for these, there are 3 other repositories, called testing repositories, that contains binary packages for candidates of other repositories:
- testing : packages for extra              and core
- community : packages for                    community 
- multilib-testing : packages for multilib.

Other repositories for newest version of certain desktop environments: 
- gnome-unstable
- kde-unstable

both the repositories contain packages of their respective desktop environments before being released into testing.

---

## ABS (Arch Build System) AND AUR (Arch User Repository):

The Arch Build System (ABS) is a ports-like source packaging system that compiles source tarballs into binary packages, which are installed via pacman. The Arch Build System provides a directory tree of shell scripts, called PKGBUILDs, that enable any and all official Arch packages to be customized and compiled. Rebuilding the entire system using modified compiler flags is also supported by the Arch Build System. The Arch Build System makepkg tool can be used to create custom pkg.tar.xz packages from third-party sources. The resulting packages are also installable and trackable via pacman.

In addition to the repositories, the Arch User Repository (AUR) provides user-made PKGBUILD scripts for packages not included in the repositories. These PKGBUILD scripts simplify building from source by explicitly listing and checking for dependencies and configuring the install to match the Arch architecture. Arch User Repository helper programs can further streamline the downloading of PKGBUILD scripts and associated building process. However, this comes at the cost of executing PKGBUILDs not validated by a trusted person; as a result, Arch developers have stated that the utilities for automatic finding, downloading and executing of PKGBUILDs will never be included in the official repositories. The Arch User Repository provides the community with packages that are not included in the repositories. Reasons include:

- Licensing issues: software that cannot be redistributed, but is free to use, can be included in the Arch User Repository since all that is hosted by the Arch Linux website is a shell script that downloads the actual software from elsewhere. Examples include proprietary freeware such as Google Earth and RealPlayer.
- Modified official packages: the Arch User Repository also contains many variations on the official packaging as well as beta versions of software that is contained within the repositories as stable releases.
- Rarity of the software: rarely used programs have not been added to the official repositories (yet).
- Betas or "nightly" versions of software which are very new and thus unstable. Examples include the "firefox-nightly" package, which gives new daily builds of the Firefox web browser.
    
PKGBUILDs for any software can be contributed by ordinary users and any PKGBUILD that is not confined to the Arch User Repository for policy reasons can be voted into the community repositories.

--- 
# REFERENCES : <img src="https://cdn4.iconfinder.com/data/icons/miu/24/common-search-lookup-outline-stroke-512.png" width="20">
- https://en.wikipedia.org/wiki/Arch_Linux#History
- https://www.archlinux.org/