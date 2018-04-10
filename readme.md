## Step 1 
生成ssh密钥对：
``` bash
$ ssh-keygen
```

## Step 2 
将ssh公钥拷贝到项目目录，Vagrant在启动虚机时会将该文件拷贝到虚机的root主目录下，使得本机可以直接通过root访问虚机
``` bash
$ ln -s ~/.ssh/id_rsa.pub id_rsa.pub
```

## Step 3
启动Vagrant
``` bash
$ vagrant up
```