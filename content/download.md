---
title: "Download"
date: "2019-07-29"
---

Two versions of libmodbus are currently maintained:

- stable release is [libmodbus-{{< stableversion >}}]({{< releaseurl >}}libmodbus-{{< stableversion >}}.tar.gz)
  (2019-07-29 but almost no changes since 2013-10-06)

- development release is [libmodbus-{{< devversion >}}]({{< releaseurl >}}libmodbus-{{< devversion >}}.tar.gz) (2019-07-29).
  This development release is very stable!

Download the tarball of the version you want and run:
{{< highlight sh >}}
./configure && make && make install;
{{< /highlight >}}
to compile and install libmodbus on your system.

The latest stable release is also available in many Linux distributions:

- [Archlinux](https://aur.archlinux.org/packages/libmodbus/)
- [Fedora](https://community.dev.fedoraproject.org/packages/libmodbus)
- [Debian](http://packages.debian.org/search?keywords=libmodbus)
- [Ubuntu](http://packages.ubuntu.com/search?keywords=libmodbus)
- [Buildroot](http://buildroot.uclibc.org/)
- [Fink](http://pdb.finkproject.org/pdb/package.php/libmodbus)

You can also browse the source code on
[github](http://github.com/stephane/libmodbus) or clone with the command
`git clone git://github.com/stephane/libmodbus` to compile and test the latest version.
