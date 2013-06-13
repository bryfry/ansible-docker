#ansible-docker

ansible playbook for provisioning docker lxc containers

##hosting.yml
setup a lxc host with the required dependencies

**tags**

* **dev** - setup for development environment, compile docker, etc.
* **ppa** - install docker from the ubuntu ppa
* **bin** - install docker from the docker-latest binary [not yet implemented]
