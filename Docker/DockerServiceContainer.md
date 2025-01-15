# Setup MariaDB container

![image](https://github.com/user-attachments/assets/d7eb1aeb-de0b-45cc-b2ff-29d5cb1b02ce)


## Command
docker container run -d -e MARIADB_USER=db_user -e MARIADB_PASSWORD=db_pass -e MARIADB_DATABASE=frontend_app -e MARIADB_ROOT_PASSWORD=mariadb_root_pass mariadb
<br><br><br>
### Output
![image](https://github.com/user-attachments/assets/3cad980e-50be-4628-84b7-a7ede8ab5b03)
<br>
![image](https://github.com/user-attachments/assets/a948fdc4-e569-4468-97dd-6ee0240c23c5)


<br>
# Setup Wordpress for Frontend
![image](https://github.com/user-attachments/assets/03ba64bf-59e4-4214-8c9f-322f90082e96)

## Command
root@Docker-Machine:~# docker container run -d -e WORDPRESS_DB_HOST=my_backend_db -e WORDPRESS_DB_USER=db_user -e WORDPRESS_DB_PASSWORD=db_pass -e WORDPRESS_DB_NAME=frontend_app --name my_fnt_app wordpress
<br><br><br>
### Output
![image](https://github.com/user-attachments/assets/8f6de755-c921-4a33-ba64-f513cf29d7df)
<br><br><br>

![image](https://github.com/user-attachments/assets/05ed1529-8a86-4b62-9556-6ec043c53910)

<p>Now I need to expose the workpress to port 8080 as well.</p>
<br>

![image](https://github.com/user-attachments/assets/dca4c736-56d5-4948-9010-3b5f141ccce2)
<br>
### create docker network
![image](https://github.com/user-attachments/assets/19a9837a-a4f6-41e9-8144-a5e47d6b75e9)

### Re-installing the docker containers
![image](https://github.com/user-attachments/assets/ffd19c8b-2a1b-40d6-a320-e47beacf7081)

## Application is Up (End to End)
![image](https://github.com/user-attachments/assets/0dec583e-901c-403f-b360-74736583a052)
