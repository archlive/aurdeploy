---
title: "Configuration"
---
# Configuration

The `config` directory is structured to accept the following files.
Hash prefixed comments are permitted in them to add some personal note.
These are all optional, depending on what you need to do with your builds.

## aur.list

The most important package list where to add the names of AUR packages if
you are going to build them.

**Note**: you need to specify explicitely the dependency files for your packages,
this is a limitation of the current system.

## pacman.list

Create one and add package names as in `aur.list` if you need to install
unofficial packages from external repositories,
this might help to avoid to build also them as dependencies of your AUR packages.

## gpgkeys.list

Here you can add the GnuPG keys required for the signed packages you are going
to process that are not included in the system.

## pacman.conf

Appended at the end of the `docker` container's `/etc/pacman.conf`, to make
available additional external repositories to use for package dependencies.

## makepkg.conf

Used to customize the build, Travis script will copy and then use it
during the build process.
