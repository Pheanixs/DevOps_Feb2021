# Task 2

## Task 2. Work with Docker

### Task 2.0

Start read documentation about docker from (https://doc.docker.com)

### Task 2.1

Install Docker use virtual machine (VM Virtual Box) on os Ubuntu 18.04.5 Server LTS
Listing commands on file (task2/cmd_inst_lin_docker.txt)

Install Docker on Windows 10 Pro x64. 
![win_docker_001.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task2/images/win_docker_001.png)


### Task 2.2

Find, download and run container "hello-world" (in site https://hub.docker.com/_/hello-world)
Listing commands on (task2/cmd_find_cont.txt)

Reading documentation how create commands and parametrs from (https://docs.docker.com/engine/reference/commandline/container_create/),
how run (https://docs.docker.com/engine/reference/commandline/container_run/) and how start (https://docs.docker.com/engine/reference/commandline/container_start/).


### Task 2.3
#### Task 2.3.1

Download image nginx. Create Docker file (task2/t2.2/Dockerfile). Create simple html page (task2/html/index.html).
Run command in bush. Command and result in file (task2/cmd_nginx.txt)

Run internet browser and check web-server (my local http://192.168.77.105:9998)

![task22_000.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task2/images/task22_000.png)

#### Task 2.3.2

Create Docker file (task2/t2.3/Dockerfile).
Command and result in file (task2/cmd_t23.txt)


### Task 2.4

Login to Docker Hub
- `sudo docker login`
- `sudo docker push pheanix/nginx-web:v2`

Results:
![task23_000.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task2/images/task23_000.png)
![task23_001.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task2/images/task23_001.png)

### Task 2.5

Create `docker-compose.yaml` file (task2/t2.5/docker-compose.yaml).

List outputs messages after running command `sudo doc up -d` in file (task2/cmd_t25.txt).

List created images `sudo docker-compose images` in file (task2/cmd_t25a.txt).

List status `sudo docker-compose ps` in file (task2/cmd_t25b).

Results:
![task25_000.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task2/images/task25_000.png)
![task25_001.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task2/images/task25_001.png)


