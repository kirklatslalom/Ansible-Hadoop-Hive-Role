<a href="https://hive.apache.org/"><img src="images/hive_logo_medium.jpg" width="200" height="200"></a>

# Ansible-Hadoop-Hive-Role

An Ansible Role to Configure and setup [Hive](https://hive.apache.org/) Data WareHouse on Client Node.

Requirements
------------
This role is dependent upon `shubhambhardwaj007.hadoop_software_installation`.
For a full usage example with the `shubhambhardwaj007.hadoop_software_installation` role, see the Example Playbook later in this README.

Role Variables
--------------
Available variables are listed below, along with default values (see vars/main.yml):
```
Hive_Software_Directory: "/root/hive_software/"
Hive_Software_Version: "apache-hive-0.13.1-bin"
Hive_Software_Download_Url: "https://archive.apache.org/dist/hive/hive-0.13.1/apache-hive-0.13.1-bin.tar.gz"
Hive_Workspace_Directory: "/root/hive_workspace"

```
Dependencies
------------
None

Example Playbook
----------------
```
 - hosts: client_node
   roles:
     - shubhambhardwaj007.ansible_hadoop_software_installation_role
     - shubhambhardwaj007.hive
```
License
-------

GNU

Author Information
------------------
This role was created in 2021 by [Shubham Bhardwaj](https://galaxy.ansible.com/shubhambhardwaj007/hive)
