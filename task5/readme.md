# Task 5

## Task 5. Databases. Remember everything.

### Task 5.1 Read about database

### Task 5.2 Install database MySQL

Docker-compose file in (task5/t5.2/docker-compose.yml)

### Task 5.3 Filling databse DevOps

Files with data (task5/students.csv and task5/results.csv)



- `SET GLOBAL local_infile=1;`

Connect to Database

- `sudo mysql -upheanix -pqwerty -h192.168.77.106 -P3308`

Select database

- `use DevOps`

Create tables

- `source students.sql`
- `source result.sql`

Past data into tables
- `LOAD DATA LOCAL INFILE '/home/pheanix/task5/students.csv' INTO TABLE students FIELDS TERMINATED BY ';' ENCLOSED BY '"' LINES TERMINATED BY '\r\n' IGNORE 1 LINES (ID, Student, StudentID);`
- `LOAD DATA LOCAL INFILE '/home/pheanix/task5/result.csv' INTO TABLE result FIELDS TERMINATED BY ';' ENCLOSED BY '"' LINES TERMINATED BY '\r\n' IGNORE 1 LINES (ID, StudentID, Task1, Task2, Task3, Task4);`


### Task 5.4 Selecting data from database

Selected Data from database

- `SELECT students.ID, students.Student, result.Task1, result.Task2, result.Task3, result.Task4 FROM DevOps.students, DevOps.result WHERE students.StudentID=result.StudentID and students.Student='Никольский Валерий Александрович';`

![mysql_query.png](https://github.com/Pheanixs/DevOps_Feb2021/blob/master/task5/images/mysql_query.png)
