# SSH settings
    1  ssh-keygen -t rsa -C 'vagrant@vagrant1'
    2  ssh-copy-id -i ~/.ssh/id_rsa.pub vagrant@192.168.33.2
    3  ssh vagrant@192.168.33.2
    4  ssh-copy-id -i ~/.ssh/id_rsa.pub vagrant@192.168.33.3
    5  ssh vagrant@192.168.33.3
# Install Ansible (Ubuntu 14.0.4) 
    $ sudo apt-get install software-properties-common
    $ sudo apt-add-repository ppa:ansible/ansible
    $ sudo apt-get update
    $ sudo apt-get install ansible
# Config Ansible HOST
    sudo vim /etc/ansible/hosts
    
    [test]
    192.168.33.2
    192.168.33.3
# Test Ansible
    ansible test -m ping

<http://docs.ansible.com/ansible/intro_installation.html#what-version-to-pick>

# TLS
  openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -subj /CN=localhost -keyout files/nginx.key -out files/nginx.crt


