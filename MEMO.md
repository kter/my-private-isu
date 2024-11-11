```
sudo apt update
sudo apt install git
sudo apt install make
sudo apt install unzip
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/debian/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc
echo   "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/debian \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" |   sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo apt install httptools
sudo apt install apache2-utils
sudo apt install apt-file
sudo apt-file update
sudo apt install mariadb-client
sudo apt install iotop
sudo apt install dstat
```

```
ab -c 1 -t 30 http://localhost/
```

```
mysqldumpslow webapp/logs/mysql/mysql-slow.log
```

```
curl -L -O https://github.com/tkuchiki/alp/releases/download/v1.0.21/alp_linux_amd64.tar.gz
tar xf alp_linux_amd64.tar.gz
sudo mv alp /usr/local/bin
alp json --file webapp/logs/nginx/access.log
```

```
top
iotop
htop
dstat
dstat --cpu
```

```
sudo apt install gpg
sudo gpg -k
sudo gpg --no-default-keyring --keyring /usr/share/keyrings/k6-archive-keyring.gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C5AD17C747E3415A3642D57D77C6C491D6AC1D69
echo "deb [signed-by=/usr/share/keyrings/k6-archive-keyring.gpg] https://dl.k6.io/deb stable main" | sudo tee /etc/apt/sources.list.d/k6.list
sudo apt-get update
sudo apt-get install k6
```
