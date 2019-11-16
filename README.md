> This repository is not longer maintained. I switched from Bloonix to Zabbix.

# Bloonix-Install.sh

Bloonix-Install.sh is a simple bash script to install the free and open-source monitoring-software [Bloonix](https://bloonix.org/) on Debian-based systems.

This script is in heavy development and I'd be happy about pull requests and/or bug reports.

**Tested on**:
  - Debian 8 (Jessie)
  - Debian 9 (Stretch)

But it should run on all debian-based distributions such as Ubuntu or elementary OS.

Please use this script with caution and **don't** run it on configured systems, only on fresh installs!

Have fun!

# Usage

Simply get the latest version of this script and set the executable bit
```sh
wget https://raw.githubusercontent.com/dominicpratt/bloonix-install/master/bloonix-install.sh
chmod +x bloonix-install.sh
```
and run it
```sh
bloonix-install.sh
```

That's it. Bloonix should be up and running on your routed domain. Initial login is admin/admin.

# Troubleshooting
  - check the bloonix-logs (/var/log/bloonix/)
  - check the nginx-log (/var/log/nginx/error.log)
  - check the syslog (/var/log/syslog)
  - create a [bug report](https://github.com/dominicpratt/bloonix-install/issues)

# TODO (in this order)
  - make apt more quiet (hints?)
  - add error handling
  - fully automate mysql-initialization
  - add installation routine for rpm-based systems
  - create distribution-packages (.deb and .rpm)

License
----

MIT
