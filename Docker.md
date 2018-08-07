# Docker

- Quick Setup
```
# download & install
$ wget https://download.docker.com/linux/centos/7/x86_64/stable/Packages/docker-ce-18.03.1.ce-1.el7.centos.x86_64.rpm
$ sudo yum install docker-*.rpm

# start daemon & first test run
$ sudo systemctl start docker
$ sudo docker run hello-world

# add to docker group
$ sudo groupadd docker
$ sudo usermod -aG docker $USER
```
ref: https://docs.docker.com/install/linux/docker-ce/centos/#upgrade-docker-ce  
ref: https://docs.docker.com/install/linux/linux-postinstall/#manage-docker-as-a-non-root-user
