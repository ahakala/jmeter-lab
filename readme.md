# jMeter with Vagrant and Ansible
This is a Vagrant/Ansible environment that can be used to quickly provision a number of hosts that can be used for load testing.

## Requirements
 - Vagrant
 - Virtual Box
 - Ansible 2.x

## use
1. Edit the servers.yaml file to reflect the correct IP and number of servers for the environment
2. Make any needed changes to the `Vagrantfile`
3. run `vagrant up` in the directory containing the vagrant file
4. once all of the servers are up run the Ansible playbook against them to configure the server nodes.
5. once these nodes are configured, set up the control machine to use all of the configured nodes. 
