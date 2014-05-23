apt-cyg
=======

A command-line software installer for Cygwin

Quick start
-----------

apt-cyg is a simple script. Once you have a copy, make it executable:

    # chmod +x /bin/apt-cyg

Optionally place apt-cyg in a bin/ folder on your path.


First of all Update package repository 
   
    # apt-cyg -m  http://ftp.jaist.ac.jp/pub/cygwin/x86_64/
    # apt-cyg -m  http://ftp.jaist.ac.jp/pub/cygwin/x86/ 　#for x86

Then use apt-cyg, for example:

    # apt-cyg install nano

Subcommands:
-----
apt-cyg: Installs and removes Cygwin packages.

    "apt-cyg install <package names>" to install packages
    "apt-cyg remove <package names>" to remove packages
    "apt-cyg update" to update setup.ini
    "apt-cyg show" to show installed packages
    "apt-cyg find <patterns>" to find packages matching patterns
    "apt-cyg search <patterns>" to find packages matching patterns
    "apt-cyg describe <patterns>" to describe packages matching patterns
    "apt-cyg packageof <commands or files>" to locate parent packages

Options:
----

     --mirror, -m <url> : set mirror
     --cache, -c <dir>  : set cache
     --file, -f <file>  : read package names from file
     --noupdate, -u     : don't update setup.ini from mirror
     --help
     --version


Contributing
------------

This project has been cloned from original to make contributing easier. Feel free to fork and modify this script.

The [Google Code project](https://code.google.com/p/apt-cyg/) has a list of open issues.


TroubleShooting
-------------

If apt-cyg fail to install or mal install database, remove package entry from install.db

     /etc/setup/install.db
  


