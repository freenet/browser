freenetbrowser - easy, secured Freenet usage for *nix
======================================

Description of freenetbrowser.

See NEWS for user-visible changes.
See ChangeLog or the history for detailed changes.

## Usage

$ freenetbrowser [options] [arguments]

## Requirements

- curl or wget
- gnupg for installing
- Java openjdk 9 or later
- icecat, waterfox or firefox

## Install

$ ./bootstrap.sh && make install

To install only for the current user, use

$ ./bootstrap.sh --prefix=$HOME/.local && make install

Also see

$ make help

For details on installing a release, see INSTALL

## Contributors

See AUTHORS

Licensed under GPLv3 or later.

(this is the default of conf. To use a different license, replace
COPYING and the header in the main code file)

## Release Process

* Check/Update NEWS
* Increase version in configure.ac (see semver.org)
* Commit, merge to stable and tag (see branching[1])
$ ./bootstrap.sh && make distcheck

[1]: See do a release in
     http://www.draketo.de/branching-strategy#action-maintainer

