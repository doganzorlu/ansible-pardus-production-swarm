
Management Server:

```bash
$ sudo apt-get update & apt-get install ansible 
$ sudo update-alternatives --install /usr/bin/python python /usr/bin/python3 1
$ sudo upt-get install python3-pip
$ sudo update-alternatives --install /usr/bin/pip pip /usr/bin/pip3 1
$ sudo pip install docker-py
$ apt-get install sshpass
```

Docker Swarm Deployment Playbook

Edit the inventory file with your current configuration. Run the following command to deploy swarm:

$ ansible-playbook -i inventory.yml -u &lt;sudo username&gt; --ask-pass -kK  deploy.yml

TODO:

- prometheus + grafana installation role
- ingress controller role
