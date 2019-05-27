# General startup scripts for Raspberry Pi

## rc.local
This file should overwrite local copy of `/etc/rc.local`.

This version of rc.local waits 5 seconds during startup in order to allow dhcpcd to acquire a valid IPv4 address.
Of course 5 seconds is empirical and might not reflect every environment.

Once elapsed this time the file `/etc/issue` is overwritten with IP address information among other informations like OS name, version and architecture.

