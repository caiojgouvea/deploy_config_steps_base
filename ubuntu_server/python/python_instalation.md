# Python Alt Instalation - Specific Version

### Pre Instalation Packages
> sudo apt update

> sudo apt install -y build-essential checkinstall

> sudo apt-get install -y libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev curl

### Downloading specific version
> cd /usr/src

> sudo wget https://www.python.org/ftp/python/3.7.9/Python-3.7.9.tgz

> sudo tar xzf Python-3.7.9.tgz

> cd Python-3.7.9

> sudo ./configure --enable-optimizations

> sudo make altinstall

> python3.7 --version