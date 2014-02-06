#ansible-docker
ansible playbook for setting up lxc-docker and required dependencies

* updates kernel (can be skipped)
* adds docker repo key
* adds docker repo
* install lxc-docker
* adds user to docker group
* restarts target if needed (kernel update)


**run**:  ```ansible-playbook docker.yml```

**non-AUFS run**: ```ansible-playbook docker.yml --extra-vars "docker_update_kernel=false"```

**note**: expects ```docker_host``` item to your inventory (hosts) file:


###things not implemented
* yum, including OS detection (please fork and add if you are interested)
* install docker from the docker-latest binary instead of repos
* re-install VBox Guest Additions if on virtualbox and kernel updated
