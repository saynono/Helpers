# Helpers
A random collection of little useful helpers. 

### Commandline thingies

This will copy your public key to a remote machine. No more login credentials needed after that.

```cat ~/.ssh/id_rsa.pub | ssh <username>@<address>  "mkdir -p .ssh; cat >> ~/.ssh/authorized_keys"```


### delete annoying hidden osx files in all subdirectories
```find . -iname '._*' -exec rm -rf {} \;```






#### oh oh windows ####

### installing mingw ###
http://www.codebind.com/cprogramming/install-mingw-windows-10-gcc/
Also tells you how to add path variables to the os. If cmake tells you something is broken you might need to add mingw bins to path.

### installing cmake ###
https://www.scivision.co/windows-gcc-gfortran-cmake-make-install/
