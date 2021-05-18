<a href="https://hadoop.apache.org/"><img src="images/Hadoop_logo.svg" width="100%" height="100%"></a>

# Ansible-Hadoop-ClientNode-Role

An Ansible Role to Configure and setup [Hadoop](https://hadoop.apache.org/) Client Node.

Requirements
------------
This role is dependent upon `shubhambhardwaj007.ansible_hadoop_software_installation_role`.
For a full usage example with the `shubhambhardwaj007.ansible_hadoop_software_installation_role` role, see the Example Playbook later in this README.

Role Variables
--------------
Available variables are listed below, along with default values (see vars/main.yml):
```
 Name_Node_Hdfs_Port: "9001"
 Job_Tracker_Mapreduce_Port: "9002"
```
The `Name_Node_Hdfs_Port` should be similar to exposed port by Hadoop Master Node.The `Job_Tracker_Mapreduce_Port` should be similar to exposed port by Hadoop Job Tracker Node.

Dependencies
------------
None

Example Playbook
----------------
```
 - hosts: client_node
   roles:
     - shubhambhardwaj007.ansible_hadoop_software_installation_role
     - shubhambhardwaj007.ansible_hadoop_clientNode_role
```
License
-------

GNU

Author Information
------------------
This role was created in 2021 by [Shubham Bhardwaj](https://galaxy.ansible.com/shubhambhardwaj007/hadoop_clientnode)
