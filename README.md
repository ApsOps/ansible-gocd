ansible-gocd
============

Ansible Playbook to install [GoCD](http://www.go.cd/) server and agents. Derived from another [repo](https://github.com/Tpbrown/ansible-gocd).

Steps to run
------------

1. Add hosts in inventory file
2. Edit variables in `vars/main.yml` and `vars/plugins.yml`
3. Run cmd `ansible-playbook -i hosts gocd.yml`
4. If you want to run specific tasks, use tags:
```
ansible-playbook -i hosts gocd.yml --tags="agent"
```