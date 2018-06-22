<!-- TITLE: Command Reference -->
<!-- SUBTITLE: Common Commands and Procedures -->

# Information Gathering
* oc get status
* oc get events
* oc describe
* oc get nodes [--show-labels]
* oc delete nodes [-l *selector*=*value*]
# Project Maintenance
# User Maintenance
# Pod Maintenance
* oc get pods
* oc rsh *pod_name*
* oc delete pods [-l *selector*=*value*]
# Node Maintenance
* oc get nodes
* ssh *node*
	* service atomic-openshift-node stop
	* rm /etc/master/config/.....
	* exit 
* oc delete nodes [-l *selector*=*value*]

# Resource Quotas and Limits
# Network Modification
# Object Security 
# Repository Maintenance
# Storage Maintenance

[Return Home](home)