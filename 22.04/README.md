# sudo免密码
```sh
sudo visudo
```

```
# 加在最后一行
runyu ALL=(ALL) NOPASSWD: ALL
```

# apt换源
```sh
sudo nano /etc/apt/sources.list
```
```sh
deb http://mirrors.tencent.com/ubuntu/ jammy main restricted universe multiverse
deb http://mirrors.tencent.com/ubuntu/ jammy-security main restricted universe multiverse
deb http://mirrors.tencent.com/ubuntu/ jammy-updates main restricted universe multiverse
deb http://mirrors.tencent.com/ubuntu/ jammy-backports main restricted universe multiverse
#deb http://mirrors.tencent.com/ubuntu/ jammy-proposed main restricted universe multiverse
```

# apt更新
```sh
sudo apt update && sudo apt upgrade
```

# 安装软件
```sh
sudo apt install build-essential gdb gcc-aarch64-linux-gnu g++-aarch64-linux-gnu cmake llvm clang \
net-tools openssh-server git curl wget bash python3-pip \
 
```

# 一键代理
```sh
git clone https://ghp.ci/https://github.com/nelvko/clash-for-linux-install.git && cd clash-for-linux-install && sudo bash -c '. install.sh; exec bash' && cd 
```

# 安装字体等
```sh
git clone https://github.com/snwh/ubuntu-post-install.git && cd ubuntu-post-install && ./ubuntu-post-install-script.sh
```

# qt(在线安装包)
```sh
sudo apt install libxcb-cursor0 libxcb-cursor-dev
wget https://mirrors.cloud.tencent.com/qt/archive/online_installers/4.8/qt-online-installer-linux-x64-4.8.0.run
./qt-online-installer-linux-x64-4.8.0.run --mirror https://mirrors.cloud.tencent.com/qt
```

## qt5(apt方式)
```sh
sudo apt-get install qtbase5-dev qtchooser qt5-qmake qtbase5-dev-tools
sudo apt-get install qtcreator
sudo apt-get install qt5*
```
# ROS
```sh
wget http://fishros.com/install -O fishros && . fishros
```

# code 
```sh
sudo snap install code --classic
```

## pip换源
```sh
pip config set global.index-url https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple
```

## code插件（建议同步）
```sh
code --install-extension ms-vscode.cpptools
code --install-extension ms-python.python
code --install-extension ms-vscode.cpptools-extension-pack
code --install-extension ms-vscode.cpptools-themes
code --install-extension ms-vscode.makefile-tools
code --install-extension ms-vscode.remote-explorer
code --install-extension ms-vscode.remote-server
code --install-extension mhutchie.git-graph
code --install-extension ms-vscode.hexeditor
code --install-extension ms-azuretools.vscode-docker
code --install-extension alibaba-cloud.tongyi-lingma
```

# miniconda
```sh
wget https://repo.anaconda.com/miniconda/Miniconda3-py39_4.12.0-Linux-x86_64.sh
bash Miniconda3-py39_4.12.0-Linux-x86_64.sh
conda init bash
conda install -c conda-forge cmake
conda install -c conda-forge llvm-tools
```
