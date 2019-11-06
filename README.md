<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table Of Content

- [Microsoft Online VS-code](#microsoft-online-vs-code)
- [coder-server](#coder-server)
  - [Install Docker on Ubuntu](#install-docker-on-ubuntu)
  - [Install code-server](#install-code-server)
- [References](#references)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Microsoft Online VS-code
- [Login](https://online.visualstudio.com/environments)


## coder-server
### Install Docker on Ubuntu
```sh
sudo apt-get update
sudo apt-get remove docker docker-engine docker.io # optional
sudo apt install docker.io
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
docker run hello-world
```

### Install code-server
- [Releases](https://github.com/cdr/code-server/releases/tag/2.1665-vsc1.39.2)
- [QuickStart](https://github.com/cdr/code-server/blob/master/doc/quickstart.md)
```sh
# download
wget https://github.com/cdr/code-server/releases/download/2.1665-vsc1.39.2/code-server2.1665-vsc1.39.2-linux-x86_64.tar.gz
# unzip
tar -xvzf code-server2.1665-vsc1.39.2-linux-x86_64.tar.gz
# set password
export PASSWORD="<your_password>"
# run silently at port 8080
cd code-server2.1665-vsc1.39.2-linux-x86_64
nohup ./code-server
```

## References
- [How to install docker on Ubuntu](https://phoenixnap.com/kb/how-to-install-docker-on-ubuntu-18-04)
- [Got permission denied while trying to connect to the Docker daemon socket](https://www.digitalocean.com/community/questions/how-to-fix-docker-got-permission-denied-while-trying-to-connect-to-the-docker-daemon-socket)


