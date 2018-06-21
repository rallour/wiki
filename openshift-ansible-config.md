<!-- TITLE: Openshift Ansible Config -->
<!-- SUBTITLE: A discussion / breakdown of the ansible.cfg for openshift. -->

# Location
# Contents
# Things to modify
# Example Config

```text
#task_includes_static = True
#handler_includes_static = True

# Controls if a missing handler for a notification event is an error or a warning
#error_on_missing_handler = True

# change this for alternative sudo implementations
#sudo_exe = sudo

# What flags to pass to sudo
# WARNING: leaving out the defaults might create unexpected behaviours
#sudo_flags = -H -S -n

# SSH timeout
#timeout = 10

# default user to use for playbooks if user is not specified
# (/usr/bin/ansible will use current user as default)
#remote_user = root

# logging is off by default unless this path is defined
# if so defined, consider logrotate
log_path = /var/log/ansible.log

```
