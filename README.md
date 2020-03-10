# Set up 🔧 Pop!_OS 💻 environment

Ansible playbook for install my development environment, based on Pop!\_OS 19.10!

## Before

Before play the playbook take a look at those variables.

```
mysql_root_password: root
workstation_license: XXX-XXX-XX
```

Set your new machine ip (could be localhost) in `hosts` file and your sudo password.

```
[popenv]
pop                                             # machine address (hostname or ip)

[popenv:vars]
ansible_python_interpreter=/usr/bin/python3
ansible_sudo_pass=123qwe                        # sudo password
```

Install ansible on the machine where you play.

[Ansible Installation Guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

Install requirements from Ansible Galazy.

```
ansible-galaxy install -r requirements.yml
```

## Install

For play the playbook execute the following command.

```
ansible-playbook -i hosts install.yml
```

## what does install

- configure apt proxy [set_apt_proxy] (todo templates)
- unconfigure apt proxy (do not leave credentials on the machine) [unset_apt_proxy]
- upload apt cache, upgrade package and os [update]
- Install base software and configure [base_software] 
    - git
    - curl
    - vim
    - ntp
    - bind-utils
    - vim-athena
- Install zsh shell [gantsign.oh-my-zsh]
- Install frequent used browsers [browsers]
- Install basic tools [basic_tools]
    - tilix
    - vs code
    - wps
- Install development software [dev_software]
    - mysql
    - sqlite3
    - java
    - gradle
    - php
    - composer
    - pip
    - nginx
    - node
    - npm
    - go
    - docker
    - docker-compose
    - vmware
    - virtual box
- Install most used IDEs [ide]
    - intellij
    - phpstorm
    - android studio
- Setup ZSH theme powerlevel10k (with fonts) [powerlevel10k]

# TODO List

- Setup graphics gnome tweaks
    - (https://github.com/jaredhocutt/ansible-gnome-extensions cloning in roles folder)
    - dash to dock
    - desktop icons
    - load conf
- Reboot at end
- Proxy for each download
