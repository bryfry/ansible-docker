#ansible-docker

ansible playbook for provisioning docker lxc containers

##hosting.yml
setup a lxc host with the required dependencies

* tag: dev - setup for development environment, compile docker, etc.
* tag: ppa - install docker from the ubuntu ppa
* tag: bin - install docker from the docker-latest binary [not yet implemented]
