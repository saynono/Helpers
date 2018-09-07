# Helpers
A random collection of little useful helpers. 

### Commandline thingies

This will copy your public key to a remote machine. No more login credentials needed after that.

```cat ~/.ssh/id_rsa.pub | ssh <username>@<address>  "mkdir -p .ssh; cat >> ~/.ssh/authorized_keys"```


### delete annoying hidden osx files in all subdirectories
```find . -iname '._*' -exec rm -rf {} \;```

### Linux: Open Serial port without sudo ###
```sudo usermod -a -G dialout [username]```
https://unix.stackexchange.com/questions/14354/read-write-to-a-serial-port-without-root



#### oh oh windows ####

### installing mingw ###
http://www.codebind.com/cprogramming/install-mingw-windows-10-gcc/
Also tells you how to add path variables to the os. If cmake tells you something is broken you might need to add mingw bins to path.

### installing cmake ###
https://www.scivision.co/windows-gcc-gfortran-cmake-make-install/

### linux fun on windows!!! ###

Serial within WSL
https://www.scivision.co/usb-tty-windows-subsystem-for-linux/

b2 -j8 toolset=msvc-14.1 address-model=64 architecture=x86 link=static threading=multi runtime-link=shared --build-type=complete stage
