# Limit the Journald jogs size

I just recently discovered that the journald logs (/var/logs/journald) took more than 1.5GB of space on most of my servers, 
which is quite a bit for servers with a disk of 25GB total. 

To check your current disk usage of said logs, run `journalctl --disk-usage`.

To limit the size of those logs, follow these steps:

1. Tell journald to not use more than a certain limit, which is undefined by default. 
  To do so, open the `/etc/systemd/journald.conf` config file. Then uncomment `#SystemMaxUse=` and set a value like `500M`
2. Restart the journald service for the changes to take effect: `systemctl restart systemd-journald.service`
3. To force the cleanup of all logs, you may run `journalctl --vacuum-size=500M` where 500M is the same value used for `SystemMaxUse=`.
