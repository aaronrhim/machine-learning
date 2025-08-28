# Installation Process

# Docker installation

Dictionary:
- Image: blueprint (reproducible environment)
- Container: one running instance of an image (state)

In team workflows, you don't normally pass around containers, because containers are meant to be disposable. Instead, you just edit and share the dockerfile (so anyone can build the image on their own machine) or you can save images (pushed to Docker Hub). 

Best practice in teams: check in the Dockerfile to git and then push built images to a registry for reusability.

### Archlinux setup
```bash
sudo pacman -S docker
sudo systemctl enable --now docker.service
sudo systemctl start --now docker.service

sudo usermod -a -G docker <username>  # allow user to run without sudo
```
Replace `<username>` with your actual Linux user.

### Build current docker image
```bash
docker build -t <image_name> .
```
Replace <image_name> with whatever name you want the image to be called.

### View existing containers
```bash
docker ps # lists running containers
docker ps -a # lists all containers, including stopped ones (preferred method)
```

### View existing images
```bash
docker image ls # lists template images
```

## Docker Navigation

### Run a new container from image
```bash
docker run -it --name <container_name> <image_name> bash
```
Replace <container> with the name of the container you are trying to access.

### Run an existing container from iamge
```bash
# If it is stopped
docker start -ai <container_name>
```
```bash
# If it is running and you want a new shell
docker exec -it <container_name> bash
```