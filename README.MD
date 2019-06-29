# Simple linux centos using docker

## Server Requirements

1. Docker (version >= 17.0.0)
1. Docker-Compose v3.7

### Install Docker
```bash
  $ sudo apt-get install -y apparmor lxc cgroup-lite curl
  $ wget -qO- https://get.docker.com/ | sh
  $ sudo usermod -aG docker YourUserNameHere
  $ sudo service docker restart
```

### Build
```bash
  $ docker build --rm -t local/c7-systemd .
```

### Start Container
```bash
  $ docker-compose up -d
```