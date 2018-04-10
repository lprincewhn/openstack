## Step 1: 生成ssh密钥对
``` bash
$ ssh-keygen
```

## Step 2: 在项目目录下创建上面生成的ssh公钥的符号链接
``` bash
$ ln -s ~/.ssh/id_rsa.pub id_rsa.pub
```
VagrantFile中定义了将该文件拷贝到虚机的root主目录下，使得本机可以直接通过root访问虚机。

## Step 3:启动Vagrant
``` bash
$ vagrant up
```
