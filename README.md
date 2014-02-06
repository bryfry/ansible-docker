#ansible-docker
ansible playbook for setting up lxc-docker and required dependencies

* updates kernel (can be skipped)
* adds docker repo key
* adds docker repo
* install lxc-docker
* adds user to docker group
* restarts target if needed


**Run**:  ```ansible-playbook docker.yml```

**Non-AUFS run**: ```ansible-playbook docker.yml --extra-vars "docker_update_kernel=false"```

**Note**: expects ```docker_host``` item to your inventory (hosts) file:


###Things not implemented
Please fork and add if you are interested

* yum, including OS detection 
* install docker from the docker-latest binary instead of repos
* re-install VBox Guest Additions if on virtualbox and kernel updated
