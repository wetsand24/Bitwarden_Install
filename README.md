$ ``apt update -y``  
$ ``apt install apt-transport-https ca-certificates curl software-properties-common -y``  
$ ``curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -``  
$ ``add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu jammy stable"``  
$ ``apt install docker-ce -y``  
$ ``systemctl status docker``  
$ ``curl -sL "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose``  
$ ``chmod +x /usr/local/bin/docker-compose``  
$ ``docker-compose --version``  
$ ``useradd -G docker,sudo -s /bin/bash -m -d /opt/bitwarden bitwarden``  
$ ``passwd bitwarden``  
$ ``chown -R bitwarden: /opt/bitwarden``  
$ ``su - bitwarden``  
$ ``cd /opt/bitwarden``  
$ ``curl -Lso bitwarden.sh https://go.btwrdn.co/bw-sh``  
$ ``chmod +x bitwarden.sh``  
$ ``./bitwarden.sh install``  
$ ``./bitwarden.sh start``  
