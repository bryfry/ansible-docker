#ansible-docker

ansible playbook for setting up docker

##docker.yml
setup a lxc host with the required dependencies

example run:```ansible-playbook -i inventory docker.yml --tags repo```

**tags**

* **repo** - setup for development environment, compile docker, etc.
* **bin** - install docker from the docker-latest binary [not yet implemented]
* **vbox** - for use with vbox host, re-install VBox Guest Additions [not yet implemented]
