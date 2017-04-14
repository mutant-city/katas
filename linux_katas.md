
## Compression

`
tar -xvzf filename.tar.gz
x: extract (vs compress)
v: verbose
z: use gzip
f: file to use (must be last)

gunzip -kv filename.gz
k: keep original file (default is to delete)
v: verbose

gzip

`



## File System 

`

top

ps - bsd syntax vs unix/linux syntax 
-----

ps aux  != ps -aux


ps aux or ps -ef -u


df -h
h: human readable


free -m or -g

`



## Random usefulness
`
watch -n 1 'command'
n: number of seconds


`


## Networking stuff
`
scp user@remote_host.com:/some/remote/directory/file ~/my_local_file.txt


lsof -i:3306
check whats running at a port

`


* [port forwarding](http://thekeesh.com/2014/01/connecting-to-a-rds-server-from-a-local-computer-using-ssh-tunneling-on-a-mac/)

