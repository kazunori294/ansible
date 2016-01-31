# ansible

## how to run command

```
HOSTCLASS=xxxxxx
ansible-playbook -i /etc/ansible/hosts /etc/ansible/hostclass/${HOSTCLASS}/site.yml --check
ansible-playbook -i /etc/ansible/hosts /etc/ansible/hostclass/${HOSTCLASS}/site.yml
```
