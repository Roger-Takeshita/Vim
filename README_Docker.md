- [How To Make Vim Amazing From Scratch](https://www.youtube.com/watch?v=mbSaK3EOqO8)

```Bash
  docker run -it ubuntu:latest /usr/bin/bash
```

```Bash
  # Create user admin to avoid using the root user
  useradd -m admin
  # Check the new user
  ls /home

  # Create a password to our admin user
  passwd admin
  # 123
  # 123

  # Add admin privileges to the user
  usermod -aG sudo admin
  # -a append
  # G supplementary group
  # sudo - group
  # admin - account

  apt-get update
  apt-get install sudo -y
  su admin
  sudo apt-get install vim -y
```

Disable `root` user

```Bash
  sudo vim /etc/passwd
```

```Bash
  root:x:0:0:root:/root:/bin/bash
  # ...
  admin:x:1000:1000::/home/admin:/bin/sh
```

```Bash
  root:x:0:0:root:/root:/sbin/nologin
  # ...
  admin:x:1000:1000::/home/admin:/bin/bash
```

Restart shell

```Bash
  exit
  su admin
  sudo apt-get install git -y
  cd
  sudo git clone https://github.com/selikapro/vimrc-likapro.git
  sudo mv vimrc-likapro/.vimrc ./
```

Install Curl

```Bash
  sudo apt-get install curl -y
```

Install Vim Plug

- [Vim-Plug](https://github.com/junegunn/vim-plug)

```Bash
  curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

```Bash
  sudo mv vimrc-likapro/hotkeys .vim
  sudo chmod 444 .vim/hotkeys
  sudo vim .vimrc
```

```Bash
  sudo apt-get install nodejs npm
  sudo npm cache clean -f
  sudo npm install -g n
  sudo n stable
  exit
  sudo admin
  node --version
  sudo npm install -g yarn
  sudo apt-get install ripgrep
  sudo apt-get install python3 python3-pip python3.8-venv -y
```

```Bash
  sudo apt-get install wget
  sudo wget -c https://golang.org/dl/go1.17.2.linux-amd64.tar.gz
  tar -xzf go1.17.2.linux-amd64.tar.gz
  sudo mv go /usr/local/
```

```Bash
  sudo vim .profile

  export PATH=$PATH:/usr/local/go/bin
  export TERM=xterm-256color
```

```Bash
  alias b='sudo vim ~/.bashrc'
  alias sb='source ~/.bashrc'
  alias lsa='ls -lah'
  alias v='sudo vim ~/.vimrc'

  export TERM=xterm-256color
```

```Bash
  :PlugInstall
```

```Bash
  docker run -it ubuntu:latest /usr/bin/bash

  useradd -m admin
  passwd admin

  usermod -aG sudo admin
  apt-get update
  apt-get install sudo -y

  su admin
  sudo apt-get install vim -y
  sudo vim /etc/passwd

  exit
  su admin
  sudo apt-get install git -y
  cd

  sudo git clone https://github.com/selikapro/vimrc-likapro.git

  sudo mv vimrc-likapro/.vimrc ./
  sudo apt-get install curl -y
  curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

  sudo mv vimrc-likapro/hotkeys .vim
  sudo chmod 444 .vim/hotkeys
  sudo vim .vimrc

  sudo apt-get install nodejs npm
  sudo npm cache clean -f
  sudo npm install -g n
  sudo n stable
  exit
  sudo admin
  node --version
  sudo npm install -g yarn
  sudo apt-get install ripgrep
  sudo apt-get install python3 python3-pip python3.8-venv -y
```
