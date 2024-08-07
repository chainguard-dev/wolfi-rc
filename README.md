# wolfi-rc

These are set of shell functions that facilitate package and image development
on Wolfi and Chainguard, within a command line environment.

You'll need to source this file into your bash profile.

I've tested it on Ubuntu and Google Cloud Shell's Debian.  It probably needs some work, to operate properly on a Mac.  PR's appreciated!

## To install wolfi-rc

```
mkdir -p ~/src
cd ~/src
git clone git@github.com:chainguard-dev/wolfi-rc.git
echo ". $PWD/wolfi-rc/wolfi-rc" >> ~/.bashrc
. ~/.bashrc
```

## wolfi-rc commands

These are set of shell functions that facilitate package and image development
on Wolfi and Chainguard, within a command line environment.

Below, you can find some helpful hints on the available commands, and what
they do...

 - wolfi-branch [BRANCH_NAME]: Get your branch of the Wolfi OS source code
   - NOTE: You must set GH_USER to your github username
 - wolfi-convert-alpine [PACKAGE]: Attempt to port an existing Alpine package to Wolfi
 - wolfi-grype [TARGET]: Run grype on a given target
 - wolfi-local: Launch latest Wolfi in a docker container, with a local package repository
 - wolfi-pr: Print a URL where you can go to submit your PR from your branch to wolfi
 - wolfi-sdk: Launch latest Wolfi in a docker container for building packages
 - wolfi-sandbox: cd into a temporary directory in the form /tmp/wolfi-YYYYMMDD-HHMMSS-XXXXXXXX
 - wolfi-shell: Launch latest Wolfi in a docker container
 - wolfi-source: Get the current Wolfi OS and Images source code, in a new wolfi-sandbox directory
 - wolfi-work: start your workstation and ssh to it
 - wolfi-yam: Reformat yaml to Wolfi specifications
 - wolfi-lastchanged: The last time an APK inside a Chainguard image was updated
 - wolfi-lastbuilt: The last time a Chainguard image was built (signed) even if contents have not changed
 - wolfi-changesummary: Friendly summary of lastchanged and lastbuilt
 - wolfi-cdiff-fs: Diff two image filesystems
 - wolfi-cdiff-cfg: Diff two image configs
 - wolfi-cdiff-mf: Diff two image manifests
 - wolfi-imgsize: Get image size
 - wolfi-cls: List files in image
 - wolfi-ccat: Cat file in image
