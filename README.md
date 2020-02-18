# Learn Ansible

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


