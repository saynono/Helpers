# Helpers
A random collection of little useful helpers. 

### Commandline thingies

This will copy your public key to a remote machine. No more login credentials needed after that.
```cat ~/.ssh/id_rsa.pub | ssh <username>@<address>  "mkdir -p .ssh; cat >> ~/.ssh/authorized_keys"```


