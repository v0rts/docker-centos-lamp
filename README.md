# centos-lamp
A CentOS 7 Docker LAMP suitable for local PHP development

# features
- Centos 7
- Apache 2.4
- MariaDB 10.1
- PHP 7.0
- Git
- Composer

# quickstart

```
cd project

# Start container
docker run -d -p 80:80 -v `pwd`:/var/www/html:Z -t centos-lamp

# Enter container
docker exec -it containername sh
```

# example usage

Create a project folder and database folder.

`mkdir -p project/database`

Move into the project folder.

`cd project`

Run the command to launch the docker and map project and database directory.

``docker run -d -p 8080:80 -v `pwd`:/var/www/html:Z -t centos-lamp``

# usage notes

Put a .sql dump into the database folder for import

