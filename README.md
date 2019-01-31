# Squid Proxy Installer

Auto install proxy on:

Ubuntu 18.04
Ubuntu 14.04
Ubuntu 16.04
Debian 8 

## Install Proxy

To install, run the script

```
wget https://raw.githubusercontent.com/digitalapplied/proxy-installer/master/proxy-install.sh
chmod 755 proxy-install.sh
sudo ./proxy-install.sh
```

# Create Users

To create users, run

```
/usr/bin/htpasswd -b -c /etc/squid/passwd USERNAME_HERE PASSWORD_HERE
```

To update password for am existing user, run

```
/usr/bin/htpasswd /etc/squid/passwd USERNAME_HERE
```


replace USERNAME_HERE and PASSWORD_HERE with your desired user name and password.
