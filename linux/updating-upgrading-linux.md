# Updating and Upgrading Linux Software


I recently starting playing around on Linux using [Virtualbox] (https://www.virtualbox.org/wiki/Downloads). After installing [Linux Mint](http://www.linuxmint.com/) I wanted to update the packages using the command line. 

### Update

Run the following to resynchronize all of package index files from their sources:

```bash
$ sudo apt-get update
```
The System will ping all repos to update the local index of available software. An update should always be done before an `upgrade`.

### Upgrade

To install the newest versions of all packages currently installed on your system, run:

```bash
$ sudo apt-get upgrade
```
Packages currently installed with new versions available are retrieved and installed. New versions of currently installed packages that cannot be upgraded without effecting the install status of another package will be left at their current version. 

Always `update` before an `upgrade`.