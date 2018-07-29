# Wordpress docker-compose

Wordpress `docker-compose` development image for local 
development experiments. To keep things simple only **HTTP** is supported.

## Quick start

Clone the repository:

```bash
git clone http://
``` 

Change to cloned directory and run `docker-compose`

```bash
cd wordpress-local-docker
docker-compose up
```

Finally navigate to page: <http://localhost:8080>

## Components used

Only official docker images are used. Below is list of used 
components.

* [Wordpress 4.9.7 with PHP 7.2 FPM Alpine](https://hub.docker.com/_/wordpress/)
* [Nginx Alpine](https://hub.docker.com/_/nginx/)
* [MySQL 8](https://hub.docker.com/_/mysql/)

Only modifications done are:

* Nginx FPM configuration added to `./nginx` directory
* Increased Nginx and PHP file upload size to 120 MB. These changes can be modified 
  in file `./php/uploads.ini`
  

