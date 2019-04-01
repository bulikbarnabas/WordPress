#!/bin/bash

# Az Ubuntu 18.04 munkaállomás konfigurálása az Ansible programmal.

#### Az Ansible telepítése:

sudo apt-get -y install software-properties-common

sudo apt-add-repository ppa:ansible/ansible -y

sudo apt-get update -y

sudo apt-get install -y ansible git

#### script indítás:

sudo ansible-pull -U https://github.com/englert/ansible.git

## script tesztelés lokálisan:
## ansible-playbook  local.yml
