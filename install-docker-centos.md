### install docker (installs depedencies and repo)
curl -fsSL https://get.docker.com/ | sh

### make user execute docker commands
usermod -aG docker $(whoami)

### enable docker service
systemctl enable docker.service

### start docker service
systemctl start docker.service

### install docker-compose
curl -L "https://github.com/docker/compose/releases/download/1.25.5/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
