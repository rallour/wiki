<!-- TITLE: Openshift Ansible Cmds -->
<!-- SUBTITLE: A list of commong and useful Openshift Ansible Cmds -->


# Anatomy of an ansible command
* ansible `<target>` -m `<command>`




# Common Commands
## Ping
### Ensure that ansible is able to reach via network all hosts that are under it's control in the open shift inventory file.
#### Useage: `ansible all -m ping`


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
node2.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
loadbalancer1.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
infranode2.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
infranode1.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
support1.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
master2.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
node1.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}
master1.df2f.internal | SUCCESS => {
    "changed": false, 
    "failed": false, 
    "ping": "pong"
}

```

