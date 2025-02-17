## Install Docker
```
sudo dnf config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.rep
sudo dnf install -y docker-ce docker-ce-cli containerd.io docker-compose-plug
```

## Start and Enable Docker
```
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
docker --version
```

## Basic Docker Commands
Pull and run:
```
docker pull (image)
docker run (image)
```

View containers:
```
docker ps
```

Run flags:
-d: detached, doesn't occupy terminal
-p: port mapping, maps first port to second port

Stop and remove container:
```
docker stop (container)
docker rm (container)
```

Remove image:
```
docker rmi (image)
```

Access detached container:
```
docker exec -it (container) (terminal emulator, bash, ubuntu, etc)
```
![containerization screenshot](/images/containerization.jpg)