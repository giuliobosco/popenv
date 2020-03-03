# Set up 🔧 Pop!_OS 💻 environment

Command:

```
ansible -m shell -a 'shutdown -h now' all -i hosts -u root
```

ping:

```
ansible all -m ping -i hosts --user root
```

playbook:

```
ansible-playbook playbook.yml
```


# todos

- set_apt_proxy (todo templates)
- unset_apt_proxy
- upload (done)
  - cache
  - os dist
  - all packages
  - python3
- basic software (done)
    - git
    - curl
    - vim
    - ntp
    - bind-utils
- shell (zsh) (done)
    - https://github.com/gantsign/ansible-role-oh-my-zsh
    - `$ ansible-galaxy install gantsign.oh-my-zsh` 
- basic gsoftware
    - google chrome
    - firefox
    - opera
    - tilix
    - vs code
    - wps
- advanced software
    - php
    - nginx (php istance, empty istance)
    - mysql
    - node
    - npm
    - docker
    - docker-compose
    - vmware
    - virtual box
- ides
    - intellij
    - phpstorm
    - android studio
- basic software 2
    - brackets
    - sublime text
- vs code conf
- vim conf
- fonts 
- oh-my-shell 
- powerlevel10k

- gnome tweaks (https://github.com/jaredhocutt/ansible-gnome-extensions cloning in roles folder)
    - dash to dock
    - desktop icons
    - load conf

