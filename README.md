lxc-clone-vagrant
=================

lxc-clone shell script fixed for vagrant-lxc provider. 

This is a fork of the lxc-clone shell script that ships with lxc-0.90. It includes a fix to a number of 
grep regular expressions that conflict with comments that vagrant-lxc drops into the lxc-container config files 
it creates.

The latest lxc-clone that ships with lxc (see https://github.com/lxc/lxc) appears to be a rewrite in C, which presumably 
will work as expected; the shell script has been abandoned. This should work for vagrant users until
the next major lxc-upgrade, at which point you could switch to the version that comes with the distribution. Alternatively,
you could simply upgrade.
