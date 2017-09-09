# vertica-ansible

Ansible playbook to deploy vertica CE on a set of hosts (max 3) running CentOS. 

* Edit your inventory file (inventory/vertica_hosts)
* Add your hosts under the vertica_hosts group
* Copy your Vertica RPM to /playbooks/roles/vertica/files
* Run the following command to install your cluster

ansible-playbook -i inventory/vertica_hosts playbooks/deploy_vertica.yml

* SSH keys will be copied across your cluster (both root and dbadmin)
* Script will set most of the required vertica prereqs on the OS
