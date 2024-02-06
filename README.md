# wolfi-rc

These are set of shell functions that facilitate package and image development
on Wolfi and Chainguard, within a command line environment.

You'll need to source this file into your bash profile.

I've tested it on Ubuntu and Google Cloud Shell's Debian.  It probably needs some work, to operate properly on a Mac.  PR's appreciated!

To use:

```
mkdir -p ~/src
cd ~/src
git clone https://github.com/chainguard-dev/wolfi-rc
echo ". $PWD/wolfi-rc" >> ~/.bashrc
. ~/.bashrc
```

Below, you can find some helpful hints on the available commands, and what
they do...

 - `wolfi-branch [BRANCH_NAME]`: Get your branch of the Wolfi OS source code
 - `wolfi-grype [TARGET]`: Run grype on a given target
 - `wolfi-local`: Launch latest Wolfi in a docker container, with a local package repository
 - `wolfi-sdk`: Launch latest Wolfi in a docker container for building packages
 - `wolfi-sandbox`: cd into a temporary directory in the form /tmp/wolfi-YYYYMMDD-HHMMSS-XXXXXXXX
 - `wolfi-shell`: Launch latest Wolfi in a docker container
 - `wolfi-source`: Get the current Wolfi OS and Images source code, in a new wolfi-sandbox directory
 - `wolfi-yam`: Reformat yaml to Wolfi specifications
