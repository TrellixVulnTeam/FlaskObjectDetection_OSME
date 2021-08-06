## Practical Web Development with: Docker, Django, Nginx, Redis and Gunicorn


### How to start MYSQL contianer 
****

docker run -d --name app-db --cpus 0.5 --memory 512m -e MYSQL_USER=hp -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=web_app_db --net app-net mysql:5.7

****
### how to start WebApp container 
****
docker run -itd --name web-app-1 -v $PWD:/code --cpus 0.5 --memory 512m -p 8080:8000 --workdir /code --net app-net -e DOCKER_CONTAINER_ID=1 python:3.8


****


