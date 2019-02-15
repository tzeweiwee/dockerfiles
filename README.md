# dockerfiles
This repo contains Dockerfiles which are hosted on Dockerhub

# Creating a new Dockerfile

1. create a new folder
2. `touch Dockerfile`
3. create a new repo and configure auto build on Dockerhub - link it to this GitHub repo
4. build the Docker image you've created: `docker build -t reponame:tagname .`
5. push the Docker image to Dockerhub for universal usage `docker push reponame:tagname`
