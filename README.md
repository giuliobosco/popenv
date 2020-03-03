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

- upload (done)
  - upload proxy file
  - cache
  - os dist
  - all packages
  - python3
  - remove proxy file
- basic software (done)
    - git
    - curl
    - vim
    - ntp
    - bind-utils
- shell (zsh)
    - https://github.com/gantsign/ansible-role-oh-my-zsh
- basic gsoftware
    - gnome tweaks
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

