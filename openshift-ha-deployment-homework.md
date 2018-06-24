<!-- TITLE: Openshift Ha Deployment Homework -->
<!-- SUBTITLE: Everything related to Open Shift HA Deployment Homework -->

# Infrastructure Information
* GUID - 8613
* SSH Command: `ssh jasosmit-redhat.com@ocplab-8613.oslab.opentlc.com`
* Project Directory: `cd /home/jasosmit/Documents/Training/openshift/openshift_advanced_deployment_homework`
# Homework General Notes
* [Homework Description Link](https://www.opentlc.com/labs/ocp_advanced_deployment/07_1_Assignment_Lab.html)
* OCP: Open Shift Community of Practice [github repo](https://github.com/redhat-cop)


# Basic and HA Requirements
* Ability to authenticate at the master console
* Registry has storage attached and working
* Router is configured on each infranode
* PVs of different types are available for users to consume
* Ability to deploy a simple app (nodejs-mongo-persistent)
* There are three masters working
* There are three etcd instances working
* There is a load balancer to access the masters called loadbalancer.$GUID.$DOMAIN
* There is a load balancer/DNS for both infranodes called \*.apps.$GUID.$DOMAIN
* There are at least two infranodes, labeled env=infra