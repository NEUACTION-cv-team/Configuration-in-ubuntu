### Hades Canyon Configuration

Copyright © 2018 FortiSTray_Action. All Rights Reserved.

---
#### How to install ubuntu alongside Windows
##### Refer to this article to assign disks
https://blog.csdn.net/lxlong89940101/article/details/80604937        
https://blog.csdn.net/baidu_36602427/article/details/86548203

#### Preparation before installing libraries

##### Change Ubuntu source to tuna

```bash
sudo gedit /etc/apt/sources.list
```

Replace all contains to follows  （this is fot ubuntu18.04）

if you want more source for different ubuntu, go to this website
https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/

```bash
# 默认注释了源码镜像以提高 apt update 速度，如有需要可自行取消注释
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse

# 预发布软件源，不建议启用
# deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-proposed main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-proposed main restricted universe multiverse

```

```bash
sudo apt-get update && sudo apt-get upgrade 
```

##### Install Git

```bash
sudo apt-get install git
```

##### Install CMake

```bash
sudo apt-get install cmake
```




#### Work environment optimization

##### Install chromium

```bash
sudo apt-get install chromium-browser
```

##### Install vscode

Download `.deb` file from official website

```bash
sudo apt-get install -f
sudo dpkg -i code_1.29.1-1542309157_amd64.deb
```

#### Install sougoupinyin

https://www.cnblogs.com/lfri/p/10769144.html

##### Resolve dependencies
```bash
sudo apt-get install -f
```



