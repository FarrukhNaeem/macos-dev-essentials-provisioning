# macos-dev-essentials-provisioning

An ansible project to setup your local MacOS/Linux machine for development by quickly downloading and installing required softwares, clone your repositories in desired file hierarchy, create configuration files based on the Environment etc.

### Prerequisites

* Install ansible using the following commands:
  * `sudo easy_install pip`
  * `sudo pip install ansible`
  
### Action Time

* `cd` into the `macos-dev-essentials-provisioning` directory and run: `ansible-playbook initiate-setup.yml` *sudo pass would be asked*

## Open to contributions

Please feel to add more capabilities to this Project.

## Useful Docker Commands

### List available docker images
`docker image ls`

### Deleting an image
`docker rmi <image_id>` use -f after *rmi* to force delete

### List running containers
`docker ps`

### List all containers 
`docker ps -a`

### Deleting a container
`docker rm <container_id>` use -f after *rm* to delete a running container

### Getting shell access into a running container
`docker exec -it <container_id> bash`

### Building from docker-compose script
`docker-compose up --build`

### Starting a docker-compose execution 
`docekr-compose up` use service or group of services as parameter if needed e.g: `docker-compose up web`

### Stopping all the docker-compose services at once
`docker-compose down` use service or group of services as parameter if needed e.g: `docker-compose down web`

### See follow logs of a specific container
`docker container logs -f <container_id>`

### See the logs of complete docker-compose execution
`docker-compose logs -f`

### Run docker-compose up in deamon mode 
`docker-compose up -d`
