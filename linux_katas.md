
## Compression

```
tar -xvzf filename.tar.gz
x: extract (vs compress)
v: verbose
z: use gzip
f: file to use (must be last)

gunzip -kv filename.gz
k: keep original file (default is to delete)
v: verbose

gzip

```



## File System 

```

top

ps - bsd syntax vs unix/linux syntax 
-----

ps aux  != ps -aux


ps aux or ps -ef -u


df -h
h: human readable


free -m or -g

```



## Random usefulness
```
watch -n 1 'command'
n: number of seconds

pbcopy < ~/.ssh/id_rsa.pub
# Copies the contents of the id_rsa.pub file to your clipboard

tail -f <your file>
# continually tails a file
```

## OS info gathering
```
uname -a
lsb_release -a
```


## Networking stuff
```
scp ~/my_local_file.txt user@remote_host.com:/some/remote/directory/file 


lsof -i:3306
check whats running at a port

```
Just like ```top``` is for CPU usage, ```iftop``` is for network usage.

* [port forwarding](http://thekeesh.com/2014/01/connecting-to-a-rds-server-from-a-local-computer-using-ssh-tunneling-on-a-mac/)


## Public Ip
```curl ipinfo.io/ip```


## Packages
* list packages
```
apt list --installed
dpkg -l
dpkg --get-selections | grep -v deinstall
dpkg --get-selections | grep postgres
```

*  https://askubuntu.com/questions/17823/how-to-list-all-installed-packages



## login banner
* figlet - for large ascii fonts
* /etc/update-motd.d/00-header
* echo "myservername" | figlet
