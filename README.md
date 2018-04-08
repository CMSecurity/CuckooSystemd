# CuckooSystemd
This Repo contains Systemd Unit Files for usage with cuckoo
Just copy these files into `/etc/systemd/system` and perform a `systemctl daemon-reload` to load the services.

These services:
- assume that you have the user and group named `cuckoo`
- will run `cuckoo rooter` as root
- will run the analysis engine and the web interface as `cuckoo` user
- will run the web interface bound to all ips (0.0.0.0)
