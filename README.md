# maas-ansible-playbook - maas region/cluster services set up with ansible playbook

This works on virtualbox.

## Overview

This is simply an example I used to come up to speed with Ansible and Maas.  There are
a few noteworthy things.

* I use a playbook to create a MaaS Region/Cluster service.  This playbook runs with a VirtualBox host.
** This is a bit backwards, because we will be using MaaS as the source for compute resources for future Ansible playbooks.
* There needs to be 3 interfaces set up.
** eth0 - this is (dhcp) the outside world.
** eth1 - this is (static) the host only network, for communicating between virtual instances on this host.
** eth2 - this is (static) the MaaS network.  A dhcp server will be running on this port for all of the MaaS cluster computers.

## Installation

## Notes

This has been used as a learning tool for me to better know MaaS and Ansible.

