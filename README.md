# ansible

## how to run command

```
HOSTCLASS=xxxxxx
ansible-playbook -i /etc/ansible/hosts/${HOSTCLASS} /etc/ansible/hostclass/${HOSTCLASS}/site.yml --check
ansible-playbook -i /etc/ansible/hosts/${HOSTCLASS} /etc/ansible/hostclass/${HOSTCLASS}/site.yml
```


### test deployment
```
HOSTCLASS=xxxxxx

cat << EOF   > /tmp/testhosts
[${HOSTCLASS}]
ip address
EOF

ansible-playbook -i /tmp/testhosts /etc/ansible/hostclass/${HOSTCLASS}/site.yml --check
ansible-playbook -i /tmp/testhosts /etc/ansible/hostclass/${HOSTCLASS}/site.yml
```
