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

### [jDownloader](https://jdownloader.org/)
JDownloader is a free, open-source download management tool with a huge community that makes downloading as easy and fast as it should be. \
DockerHub: [jlesage/jdownloader-2](https://hub.docker.com/r/jlesage/jdownloader-2) \
GitHub: [jlesage/docker-jdownloader-2](https://github.com/jlesage/docker-jdownloader-2)

### [Wordpress](https://wordpress.org/download/)
The world’s most popular website builder. \
DockerHub: [wordpress](https://hub.docker.com/_/wordpress) \
GitHub: [wordpress](https://github.com/docker-library/wordpress) 
## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
