# Creating Debian packages
A talk to be given at the [Perth Linux Users' Group][PLUG] on 9 Oct 2018.

    [PLUG]: http://www.plug.org.au/

## Blurb

Once upon a time, Debian was a GNU/Linux distribution that was mainly for hobbyists.  It always existed in the shadow of commercial distributions such as Red Hat, and their derivatives.  Then Canonical used it to create Ubuntu, and the world changed.  (In the interim though, there were a lot of businesses relying on Debian as a stable, low-TCO server OS with good security support.)

If you are running Debian on a personal host or in production, you might have wondered how Debian packages work and whether you have a use case for which they could make your life simpler.  This talk will attempt to shed light on these questions.

Topics covered:

  - .deb package format
  - Source Packages
  - Creating .deb files

It is even possible to host your own package archive on an HTTP or FTP server, with secure downloads provided by Debian's package signing mechanism.

Please note that this talk will *not* cover becoming a Debian maintainer/developer, which is usually what is required to upload new/changed packages to the official Debian package archives.

## Outline

1. Principles
1. Package format
1. Intro to Debian packages
  1. Dependencies
  1. Patches (Quilt)
  1. Package signing
1. Source Packages
  1. Old -- upstream tarball + diff
  1. New -- upstream tarball + Debian tarball
  1. Native -- upstream tarball with debian subdirectory
  1. .dsc file
1. Creating .deb files
  1. debian subdirectory
      1. Debian changelog
      1. control
      1. rules
      1. compat
      1. copyright
  1. Debhelper
      1. Automatic inclusions
      1. Minimal rules file
  1. Preparation
      1. build-essential
  1. Build process
      1. dpkg-buildpackage
1. Archives

## Presenter bio

Alastair is a Software Engineer and system administrator by trade.  He has a BSc in Computer Science from Curtin University.

His computer-related interests lie in various areas within his trade; suffice to say that he is a "geek of many colours". :)  Alastair is a die-hard FOSS user and Linux fan.

He is also a freelancer with his own business.  [Warpspace IT](http://www.warpspace.net/) is a consultancy with a fairly broad focus on the technical side of IT.

## Slides

[presentation.odp](presentation.odp)
