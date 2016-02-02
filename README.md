# SSH settings
    1  ssh-keygen -t rsa -C 'vagrant@vagrant1'
    2  ssh-copy-id -i ~/.ssh/id_rsa.pub vagrant@192.168.33.2
    3  ssh vagrant@192.168.33.2
    4  ssh-copy-id -i ~/.ssh/id_rsa.pub vagrant@192.168.33.3
    5  ssh vagrant@192.168.33.3
# Install Ansible 
<http://docs.ansible.com/ansible/intro_installation.html#what-version-to-pick>


