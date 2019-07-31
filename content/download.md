---
title: "Download"
date: "2019-07-29"
---

Two branches of libmodbus are currently maintained:

- development release [v{{< devversion >}}]({{< releaseurl >}}libmodbus-{{< devversion >}}.tar.gz),
  released on 2019-07-31. See the [release notes](https://github.com/stephane/libmodbus/releases/tag/v{{< devversion >}}).
  This development version is very stable and will be marked as stable very soon.

- old release [v{{< stableversion >}}]({{< releaseurl >}}libmodbus-{{< stableversion >}}.tar.gz).
  See the [release notes](https://github.com/stephane/libmodbus/releases/tag/v{{< stableversion >}}).
  Almost no changes since 2013-10-06, should NOT be used on new project.

Download the tarball of the version you want by clicking and the version numbers and run:
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
