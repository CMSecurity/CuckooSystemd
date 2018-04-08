# CuckooSystemd
This Repo contains Systemd Unit Files for usage with cuckoo  
Just copy these files into `/etc/systemd/system` and perform a `systemctl daemon-reload` to load the services.  

These services:
- assume that you have the user and group named `cuckoo`
- will run `cuckoo rooter` as root
- will run the analysis engine and the web interface as `cuckoo` user
- will run the web interface bound to all ips (0.0.0.0)
- will run the API bound to all ips (0.0.0.0) on port 8090

Tested on an Ubuntu 16.04 LTS with a fresh cuckoo install according to their documentation
