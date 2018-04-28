# ansible-role-openvpn-pia
Ansible role for installing and configuring Private Internet Access VPN

## configure
Edit the /etc/openvpn/secret file and set your credentials.
```
$ vi /etc/openvpn/secret
```

## change default server
Create a directory .pia in your home dir. In the .pia directory create
a symlink to one of the openvpn configuration settings. For example:
```
$ cd ~
$ mkdir .pia
$ cd .pia
$ ln -s /etc/openvpn/pia/Sweden.ovpn
```
The configuation in the local homedir will now be read by the script.
