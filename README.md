# ubuntu-ansible-docker

How to build Ubuntu on Vagrant on Mac and provision Docker on guest OS.

## Getting Started

- MacOS, Vagrant
- Ubuntu16.04

### Prerequisites

```
$ brew install ansible
```

### Installing

```
$ vagrant ssh

gesut(ubuntu)
$ sudo apt-get install python
$ exit

host(Mac)
$ git clone ubuntu-ansible-docker.git
$ cd ubuntu-ansible-docker
$ echo {guest hostname} > hosts
$ vagrant up
$ ansible-playbook -i hosts playbook.yml
```

- failed = 1 is output but there is no problem

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
