---
date: 2021-05-16
permalink: "/install-ns2-on-windows-2021/"
---

# Installing ns2 on Windows/Cygwin (2021)
For #ModuleMESI.

See _[The Network Simulator ns-2: Building Ns version 2](https://www.isi.edu/nsnam/ns/ns-build.html)_
&sect; "Getting everything at once". `[saved:ns-allinone-2.35.tar.gz]`

- [gcc - No gcc4 in Cygwin's package list | Stack Overflow](https://stackoverflow.com/questions/21105574/no-gcc4-in-cygwins-package-list)
    * > I had to use NS-2 on Windows.
    * KAITO: Tried some options, none helped.


## That github user's repo

[@enfoss/**ns2-win32**](https://github.com/enfoss/ns2-win32)
  * "a compilation of **NS-2.1b9a** which bundles with it Tcl 8.3 and NAM"

Same SHA1 hashes of `ns-2.1b9a-win32.exe` and `nam-1.0a11a-win32.exe` (00FB407E498CB6F0BC670CA3F07F2A3F4318FA4A and D8F983CB77C6A49C69DA4C96A519BC6290028755)
that this webpage references
http://www.winlab.rutgers.edu/~sumathi/ns2-install.html
and that I downloaded ISI.edu via Wayback Machine.
Also, `tcl830.exe`

http://web.archive.org/web/20131126125528/http://www.isi.edu/nsnam/dist/binary/ns-2.1b9a-win32.exe
http://web.archive.org/web/20150704010730/http://www.isi.edu/nsnam/dist/binary/nam-1.0a11a-win32.exe

http://web.archive.org/web/20080524203749/http://www.isi.edu/nsnam/dist/binary/ns-allinone-2.28-cygwin-binaries.zip

---

Page not found
https://www.isi.edu/nsnam/dist/binary/ns-allinone-2.29-cygwin-binaries.zip


## Install Cygwin

Mirror: https://mirror.clarkson.edu

* Default packages
* "Develop" category: install all packages for `gcc*` and other dev stuff.
* "X11" category: choose `xorg-server xinit libX11-devel libXmu-devel`.
* Uncheck "**Hide obsolete packages**", search for and select a version for `w32api` version (currently one `9999-1` is available).


## Build ns-allinone (FAILED)

Download ns-allinone from ["Getting everything at once" section, "The Network Simulator ns-2: Building Ns version 2" | ISI.edu](https://www.isi.edu/nsnam/ns/ns-build.html)
    * [DL for ns-allinone-2.35.tar.gz](http://sourceforge.net/projects/nsnam/files/allinone/ns-allinone-2.35/ns-allinone-2.35.tar.gz/download)

## Extract

```sh
# E**x**tract (**v**erbosely) the **f**ile `ns-allinone-2.35.tar.gz` into the cwd
tar -xvf ns-allinone-2.35.tar.gz

cd ns-allinone-2.35

./install
```

```diff
-gcc4 and gcc4-g++
+gcc-core and gcc-g++

w32api
```

---

END.
