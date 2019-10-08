#DNF
DNF is a software package manager that installs, updates, and removes packages on RPM-based Linux distributions. 
It automatically computes dependencies and determines the actions required to install packages. DNF also makes it easier to maintain groups of machines, eliminating the need to manually update each one using rpm. Introduced in Fedora 18, it has been the default package manager since Fedora 22. 

DNF or Dandified yum is the next generation version of yum. It roughly maintains CLI compatibility with yum and defines a strict API for extensions and plugins. Plugins can modify or extend features of DNF or provide additional CLI commands.
 
##*Features*
- Support for multiple repositories
-  Simple configuration
- Dependency calculation based on modern depsolving technology
-    Faster and less memory-intensive operation
-    RPM-consistent behavior
-   Package group support, including multiple-repository groups
-   Simple interface
-    Documented, solid Python API
-    DNF runs in both Python 2 and Python 3
-    C bindings for lower level libraries:
   -     hawkey for package querying and depsolving. PackageKit is already making use of hawkey
   -  librepo for repo operations. PackageKit is already making use of librepo
   -     libcomps for comps operations

##*Dependencies*
**libdnf**

   - High-level API for DNF and underlying libraries
   - C, C++, LGPLv2+

**libsolv**

  - A free package dependency solver using a satisfiability algorithm
  - For solving packages and reading repositories
  -  C, New BSD License

**librepo**

 -  A library providing C and Python (libcURL like) API for downloading Linux repository metadata and packages
 -   C, LGPLv2+

**libcomps**

 -  Libcomps is alternative for yum.comps library. It is written in pure C as library and there are bindings for python2 and python3.
 -  C, GPLv2+

##*Installation*

DNF comes with Fedora since version 18, but DNF can installed by using the yum Command:

    # yum install dnf

As of Fedora 22, yum has been replaced with DNF and doesn't need to be installed. 


##* Usage*

In the basic methods, DNF can be used almost exactly as yum to search, install or remove packages:

    # dnf search audacity

    # dnf install audacity 

    # dnf remove audacity 

##*Updating software*

If you want to keep your system updated, the PackageKit update applet will help you. It will notify you about updated packages and security updates. Its settings can be changed at   
*System > Preferences > Software Updates*

 If you want to update your system manually, open the GNOME Software application or run

    #dnf upgrade




##*Installing / Removing software*

If you want to install or remove software, open the GNOME Software application. To install or uninstall packages, click the Install or Remove boxes. To install packages on the command line, simply type:

    dnf install package1 package2 package3

To remove packages:

    dnf remove package2


##*dnf shell*

Open the dnf shell with:

    #dnf shell

Once inside the shell, you can type dnf commands directly, such as:

    update
    install firefox emesene
    remove pidgin
    transaction run

You can use any valid dnf command in the dnf shell. To see what it will do, type:

    transaction list

To accept the changes, type:

    transaction run

For more information about the dnf shell, have a look at the dnf-shell manual page.

    man dnf-shell

##*Searching software*

You can search software in the graphical GNOME Software application by entering search terms in the search box or on the command line by typing

    dnf search searchterm1 searchterm2

##*Sources*
- Wikipedia
  - [DNF (software)](https://en.wikipedia.org/wiki/DNF_(software))
- Fedora Wiki
  - [DNF](https://fedoraproject.org/wiki/DNF?rd=Dnf)
  - [Package Management](https://fedoraproject.org/wiki/Differences_to_Ubuntu#Package_Management)
