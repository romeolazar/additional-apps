# Home Media Server

LANG=:us:

### Prerequisites.
- A public domain name. Buy one at [https://www.namecheap.com/](https://www.namecheap.com/)
- Use one for free at [https://duckdns.org](https://duckdns.org)
- Docker: [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
- Docker Compose: [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)
- Server platform: [Rocky Linux 8](https://rockylinux.org/download)

# Applications
## additional-apps
### [Transmission](https://transmissionbt.com)
A Fast, Easy and Free Bittorrent Client For macOS, Windows and Linux. \
GitHub: [linuxserver/docker-transmission](https://github.com/linuxserver/docker-transmission)

to be updated:
> TimeMachine, Teedy, Readarr, Prism, Photostructure, Nextcloud, Elkarbackup, Duckdns
### [Heimdall](https://heimdall.site)
Is a way to organise all those links to your most used web sites and web applications in a simple way. Simplicity is the key to Heimdall. Why not use it as your browser start page? \
DockerHub: [linuxserver/heimdall](https://hub.docker.com/r/linuxserver/heimdall) \
GitHub:[linuxserver/Heimdall](https://github.com/linuxserver/Heimdall)

### Owntone
(iTunes) is a media server with support for AirPlay devices, Apple Remote (and compatibles), Chromecast, MPD and internet radio. \
DockerHub: [owntone/forked-daapd](https://github.com/owntone/forked-daapd) \
GitHub: [linuxserver/daapd](https://hub.docker.com/r/linuxserver/daapd)

### Watchtower
With watchtower you can update the running version of your containerized app simply by pushing a new image to the Docker Hub or your own image registry. Watchtower will pull down your new image, gracefully shut down your existing container and restart it with the same options that were used when it was deployed initially. \

DockerHub: [containrrr/watchtower](https://hub.docker.com/r/containrrr/watchtower) \
GitHub: [containrrr/watchtower](https://github.com/containrrr/watchtower)
## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
