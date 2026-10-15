docker build -t tailred1223/fedora-httpd:1.0 .
docker images

docker run -d -p 8080:80 --name dmytro-web tailred1223/fedora-httpd:1.0
docker ps

curl.exe -i http://localhost:8080
http://localhost:8080
docker history tailred1223/fedora-httpd:1.0

docker login
docker push tailred1223/fedora-httpd:1.0

docker stop dmytro-web
docker rm dmytro-web
docker rmi tailred1223/fedora-httpd:1.0
docker images
docker pull tailred1223/fedora-httpd:1.0
docker images


1.1
docker build -t tailred1223/fedora-httpd:1.1 page/
docker run -d -p 8080:80 --name dmytro-page tailred1223/fedora-httpd:1.1
docker ps
curl.exe -i http://localhost:8080
http://localhost:8080
docker images