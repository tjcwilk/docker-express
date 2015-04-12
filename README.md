# docker-express
A Base nodejs Express application in a docker container.

# Install

General Docker instillation documentation can be found here - https://docs.docker.com/installation.  However, in summary:

* To install docker on windows, it needs to run inside a VM. Docker have a tool named Boot2Docker that wraps the use of using docker in a VM behind some sleek commands inside a terminal window. Follow this: https://docs.docker.com/installation/windows/

*  Linux: if your using a debian derivative, you could use apt-get install docker.. but the official pages recommend you wget it from them directly so you have an up to date version. Im assuming on others things like rpm will do the same.

* Mac, no idea. consult the official docs :)


# Using Docker

* Build: `docker built -t <image-name> <location>`
* Run: `docker run -name <container-name> -p 80:3000 <image-name> <command>`
* Run with mountpoint: `docker run -v <host-folder>:<container-mountpoint> --name <container-name> -d -p 80:3000 <image-name>`

* exec inside container: `docker exec <image_id> node ./bin/www`
* attatch to container: `docker exec -ti <image_id> /bin/bash`

* List images: `docker images`
* List containers: `docker ps` or `docker ps -a`



