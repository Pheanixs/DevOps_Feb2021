# Task 4

## Task 4. Jenkins. Control it.

### Task 4.0

Readed theoretical material about Jenkins.

### Task 4.1 Installing Jenkins.
#### Task 4.1.1 Installing Jenkins on host.

Install Jenkins on host (commands and results in file task4/cmd_inst_jenkins.txt)

#### Task 4.1.2 Installing Jenkins in Docker.

Download image Jenkins (commands and results in file task4/cmd_pull_jenkins.txt)

- `pheanix@userv00:~$ sudo docker pull jenkins/jenkins:lts`
- `pheanix@userv00:~$ sudo docker images`
- `pheanix@userv00:~$ mkdir jenkins`
- `sudo docker run -p 9999:8080 -p 50000:50000 -v /home/pheanix/jenkins:/var/jenkins_home jenkins/jenkins:lts`

![jenk000.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk000.png)

### Task 4.2 Installing requirement plugins.

Installing default plugins. Install plugin Green Balls.

### Task 4.3 Create build agent.

Create agent

![jenk001.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk001.png)

![jenk002.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk002.png)

![jenk002a.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk002a.png)

![jenk002b.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk002b.png)

![jenk002c.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk002c.png)


### Task 4.4 Create Freestyle project.

![jenk003.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk003.png)

### Task 4.5 Create pipeline which the execute on host commnad docker ps -a.

Dockerfile in (task4/Jenkins/Dockerfile)
Docker-compose file in (task4/docker-compose.yml)

![jenk004.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk004.png)

![jenk005.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk005.png)

### Task 4.6 Create pipeline which download from repository image.

![jenk006.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk006.png)

![jenk007.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk007.png)

Log from jenkins in file (task4/t4.6_jenkins.log)

### Task 4.7 .

![jenk008.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk008.png)

![jenk008.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task4/images/jenk009.png)


Log from jenkins in file (task4/t4.7_jenkins.log)


