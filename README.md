# Ansible Playbooks Project

In this project, I created Ansible playbooks for installing apache and git on multiple ubuntu and amazon linux servers, using variables and handlers.

# Project Steps

## Step 1: Setting up our Ansible architecture

First, launch five EC2 instances in us-east-1. Using the free tier options, launch three ubuntu servers and two amazon linux 2 servers. 
Under advanced details, make sure to select an EC2 SSM role for the IAM instance profile to be able to connect to the instances via the Session Manager.
Once they have launched, update their names, designating one of the ubuntu servers as the controller, and the other two as clients. Rename the amazon linux 2 clients as well.


![image1](images/architecture.png)

## Step 2: Setting up the controller

To install Ansible on the ubuntu controller, use the official ansible documentation: https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html#installing-ansible-on-ubuntu 

![image2](images/ansibleinstall.png)