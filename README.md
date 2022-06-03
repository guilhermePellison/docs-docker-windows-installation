# INSTALAÇÃO DOCKER

### Baixe o ubuntu na microsoft store, em seguida abra e rode os comandos:

    sudo apt-get update

```
sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```

    sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

```
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable"
sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

```
sudo apt-get update
```

```
sudo apt-get install docker-ce docker-ce-cli containerd.io
```

```
sudo service docker start
```

```
sudo docker run hello-world
```

```
sudo apt-get update
```

```
sudo apt-get upgrade
```

```
sudo apt-get install docker-compose
```

<br>

##### Referência: https://docs.docker.com/engine/install/ubuntu/
