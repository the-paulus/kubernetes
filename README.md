# kubernets
A collection of Ansible playbooks and Vagrant files to create a virtual Kubernetes cluster.

## Pre-requisits

## Clusters

Each directory is a different type of cluster that use Vagrant and Ansible. The ansible.cfg file located in the root of this project is linked to one in each of the directory that define common settings.

For each cluster simply run the following commands to spin up the cluster:

```
vagrant up
ansible-playbook setup.yml
```

- basic-cluster -- A simple cluster of one control plane node and three workers.
- basic-cluster-storage -- Just like the basic-cluster but each worker has an additional disk drive attached for storage.
- ha-cluster - A high available kubernetes cluster, containing only
