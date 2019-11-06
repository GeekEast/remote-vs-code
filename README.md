
## Microsoft Online VS-code
- [Login](https://online.visualstudio.com/environments)


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
https://github.com/cdr/code-server/releases/download/2.1665-vsc1.39.2/code-server2.1665-vsc1.39.2-linux-x86_64.tar.gz
tar -xvzf code-server2.1665-vsc1.39.2-linux-x86_64.tar.gz
cd code-server2.1665-vsc1.39.2-linux-x86_64
./code-server
```

## References
- [How to install docker on Ubuntu](https://phoenixnap.com/kb/how-to-install-docker-on-ubuntu-18-04)
- [Got permission denied while trying to connect to the Docker daemon socket](https://www.digitalocean.com/community/questions/how-to-fix-docker-got-permission-denied-while-trying-to-connect-to-the-docker-daemon-socket)
