#ansible-docker
ansible playbook for setting up docker

* updates kernel (linux-image-generic-lts-raring)
* adds docker repo key
* adds docker repo
* install lxc-docker
* adds user to docker group
* restarts target if needed

##docker.yml
setup a lxc-docker host with the required dependencies

example run: ```ansible-playbook docker.yml```

make sure to add a docker_host item to your inventory (hosts) file

###things not implemented
* install docker from the docker-latest binary instead of repos
* re-install VBox Guest Additions if on virtualbox and kernel updated
