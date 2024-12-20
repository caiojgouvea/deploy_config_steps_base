# Installing Docker

### Installing
> sudo apt update && sudo apt upgrade -y

> sudo apt remove docker docker-engine docker.io containerd runc

> sudo apt install -y apt-transport-https ca-certificates curl software-properties-common

> curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

> echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

> sudo apt update

> sudo apt install -y docker-ce docker-ce-cli containerd.io

> sudo docker --version

### Allow execution without sudo

> sudo usermod -aG docker $USER

> sudo systemctl start docker

> sudo systemctl enable docker

### Installing 'docker-compose'

> sudo apt install docker-compose