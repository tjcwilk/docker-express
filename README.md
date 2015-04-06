# docker-express
A Base nodejs Express application in a docker container.

# Install

General Docker instillation documentation can be found here - https://docs.docker.com/installation.  However, im summary:

* To install docker on windows, it needs to run inside a VM. Docker have a tool named Boot2Docker that wraps the use of using docker in a VM behind some sleek commands inside a terminal window. Follow this: https://docs.docker.com/installation/windows/

*  Linux: if your using a debian derivative, you could use apt-get install docker.. but the official pages recommend you wget it from them directly so you have an up to date version. Im assuming on others things like rpm will do the same.
*  
* Mac, no idea. consult the official docs :)


# Build

* change into the application directory
* To build, run `docker build -t docker-express . `. This pulls down the base docker image
* To launch the app inside the container, run `docker run -it --rm --name my-running-app docker-express`
