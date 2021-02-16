# Task 3

## Task 3. Work with Ansible

### Task 3.1 Install and configure Ansible
Install Ansible to server
- `sudo apt install python-pip`
- `sudo pip install ansible`

Check version
- `ansible --version`

- `pheanix@userv00:~/task3$ ansible --version
ansible 2.10.5


Create SSH-Key

- `ssh-keygen -t rsa`
- `sudo chmod 600 ~/.ssh/userv00.pub`
- `ssh-copy-id -i /home/pheanix/.ssh/userv00.pub pheanix@192.168.77.106`
- `ssh-copy-id -i /home/pheanix/.ssh/userv00.pub pheanix@192.168.77.108`

Create files in folder task3
group_vars/servers (task3/group_vars/servers)
hosts.txt (task3/hosts.txt)
ansible.cfg (task3/ansible.cfg)


### Task 3.2 Command Ping-Pong

- `ansible all -m ping`
![ans000.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task3/images/ans000.png)


- `ansible-inventory --list`
![ans001.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task3/images/ans001.png)


Task 3.3

Create playbook `task3.yml` (task3/task3.yml)

- `ansible-playbook --ask-become-pass task3.yml`
![ans002.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task3/images/ans002.png)
