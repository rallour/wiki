<!-- TITLE: Openshift Ansible Cmds -->
<!-- SUBTITLE: A list of commong and useful Openshift Ansible Cmds -->


# Anatomy of an ansible command
* ansible `<target>` -m `<command>`




# Common Commands
## Ping
### Ensure that ansible is able to reach via network all hosts that are under it's control in the open shift inventory file.
Useage: `ansible all -m ping`

```text
[root@bastion ansible]# ansible all -m ping
master3.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
node3.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
...

```

## Shell
### This command allows you to run arbitrary shell commands against the specified group of servers. The command output, return code and server name are returned for each server that matches the selector.
Example: `ansible nodes -m shell -a 'systemctl status docker | grep Active '`


```text
ansible nodes -m shell -a 'systemctl status docker | grep Active '
master1.df2f.internal | SUCCESS | rc=0 >>
   Active: active (running) since Thu 2018-06-21 13:21:37 UTC; 3h 57min ago

node2.df2f.internal | SUCCESS | rc=0 >>
   Active: active (running) since Thu 2018-06-21 13:21:37 UTC; 3h 57min ago

node3.df2f.internal | SUCCESS | rc=0 >>
   Active: active (running) since Thu 2018-06-21 13:21:43 UTC; 3h 57min ago

...
```


