# SSC-Docker-Compose
Self Signed Certificate on nginx proxy to nodejs using Docker-Compose


Create Self Signed Certificate
sudo openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -keyout selfsigned.key -out selfsigned.crt -config req.cnf -sha256

Create diffie-hellman parameter
sudo openssl dhparam -out dhparam.pem 4096

For Reference only
docker build -t app .

For Reference only
docker run -p 9000:80 app

Commands
docker-compose build
docker-compose up
docker-compose down

sh access
docker-compose exec node sh
docker-compose exec proxy sh