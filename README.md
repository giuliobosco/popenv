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

## Variables:

Insert in this line of `install.yml` file:

```
workstation_license: XXX-XXX-XXX
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
- browsers (done)
    - google chrome
    - firefox
    - opera
- basic tools (done)
    - tilix
    - vs code
    - wps
- development software (done)
    - mysql (done)
    - sqlite3
    - java
    - gradle
    - php
    - composer
    - pip
    - nginx (php istance, empty istance)
    - node
    - npm
    - go
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

REQUIRED REBOOT

FIX PROXY FOR ALL DOWNLOAD
