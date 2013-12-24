#ansible-docker
ansible playbook for setting up docker

##docker.yml
setup a lxc-docker host with the required dependencies

example run: ```ansible-playbook docker.yml```

make sure to add a docker_host item to your inventory (hosts) file

###things not implemented
* install docker from the docker-latest binary instead of repos
* re-install VBox Guest Additions if on virtualbox and kernel updated
