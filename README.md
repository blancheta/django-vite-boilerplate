# Django Vite Boilerplate

### Prerequisites

```
- Install docker
- Ensure docker is running
```

### Steps to build the project

```
- Install docker, docker-compose
- Run docker
- docker pull python
- Create Dockerfile containing logic to run a django dev server DEBUG=True
- docker run backend --tag app-backend -p 80:8000 
- Add docker-compose configuration file because I have realised that static files for django admin can only be served via nginx or apache
- Add nginx service in docker-compose.yml file
- Add nginx configuration file
- Create a volume to share static files from django with nginx container

```

### Deploy project

```
docker-compose up --build
```

### Access the project
http://127.0.0.1:1337