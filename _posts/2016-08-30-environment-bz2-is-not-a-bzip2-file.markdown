---
layout: post
title: "Gentoo: \"environment.bz2 is not a bzip2 file\""
date: 2016-08-30 07:08:00 +0300
categories: gentoo portage gnu linux
---

It seems to be a weird [rare issue](https://www.google.com/#newwindow=1&q=%22environment.bz2+is+not+a+bzip2+file%22) (none of the links helped me).
For me it happens during the installation of `www-client/chromium` binary package, made with `quickpkg`.
The `environment.bz2` is a plain text **in my case**.

If anybody else running into exactly **the same** issue, here's a dirty workaround:

```bash
#/etc/portage/make.conf

PORTAGE_BZIP2_COMMAND="/usr/local/sbin/bzip2_or_cat"
```

```bash
#!/bin/bash
#/usr/local/sbin/bzip2_or_cat

FILENAME="${@: -1}"
bzip2 $@ || cat "${FILENAME}"
```

Also here's a performance improvement I use (requires `app-arch/lbzip2`):

```bash
#!/bin/bash
#/usr/local/sbin/bzip2_or_cat

FILENAME="${@: -1}"
lbunzip2 -n8 $@ || bzip2 $@ || cat "${FILENAME}"
```

And don't forget to `chmod +x bzip2_or_cat`.
