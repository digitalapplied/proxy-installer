# Proxy Installer

Auto install proxy on:

Ubuntu 18.04
Ubuntu 14.04
Ubuntu 16.04
Debian 8 

## Install Proxy

To install, run the script:

```
wget https://raw.githubusercontent.com/digitalapplied/proxy-installer/master/proxy-install.sh
chmod 755 proxy-install.sh
sudo ./proxy-install.sh
```

Auto install script:
To change the proxy username > change 'usern'
To change the proxy password > change 'passw'

```
#!/bin/sh

wget https://raw.githubusercontent.com/digitalapplied/proxy-installer/master/proxy-install.sh
bash proxy-install.sh
/usr/bin/htpasswd -b -c /etc/squid/passwd usern passw
```

# Create Users

To create users, run:

```
/usr/bin/htpasswd -b -c /etc/squid/passwd USERNAME_HERE PASSWORD_HERE
```

To update password for am existing user, run

```
/usr/bin/htpasswd /etc/squid/passwd USERNAME_HERE
```


replace USERNAME_HERE and PASSWORD_HERE with your desired user name and password.
