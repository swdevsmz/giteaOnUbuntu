# giteaOnUbuntu
~~~
docker-compose.yml
version: '3'
services:
  web:
    image: gitea/gitea:1.7
    volumes:
      - ./gitea-data:/data
    ports:
      - "3000:3000"
      - "10022:10022"
    environment:
      - TZ=Japan
      - SSH_PORT=10022
    restart: always
~~~
