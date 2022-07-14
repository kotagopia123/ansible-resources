# Check the Python Version
$ python --version

# Install pip module
$ sudo yum install python-pip -y

# Check the Pip 
$ pip --version

# Download the requirements.txt from GitLab
git clone https://gitlab.com/rns-devops/Ansible-Resources.git

$ cd Ansible-Resources/Ansible-Installation
$ sudo pip install -r requirements.txt
$ ansible --version

Tomcat Server Role:

# Install required roles
$ ansible-galaxy install robertdebock.bootstrap
$ ansible-galaxy install robertdebock.core_dependencies
$ ansible-galaxy install robertdebock.java
$ ansible-galaxy install robertdebock.service
$ ansible-galaxy install robertdebock.tomcat

# Run the Tomcat Playbook
$ cd ~/Ansible-Resources/Ansible-Installation
$ vi tomcat.yml
$ ansible-playbook tomcat.yml
$ netstat -nltp

# Test Tomcat Server
http://Public_IP:8080
http://Public_IP:8080/helloworld
http://Public_IP:8080/sample
