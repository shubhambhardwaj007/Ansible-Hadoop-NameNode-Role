<a href="https://hadoop.apache.org/"><img src="images/Hadoop_logo.svg" width="100%" height="100%"></a>

# Ansible-Hadoop-NameNode-Role

An Ansible Role to Configure and setup [Hadoop](https://hadoop.apache.org/) Name Node.

Requirements
------------
This role is dependent upon `shubhambhardwaj007.hadoop_software_installation`.
For a full usage example with the `shubhambhardwaj007.hadoop_software_installation` role, see the Example Playbook later in this README.

Role Variables
--------------
Available variables are listed below, along with default values (see vars/main.yml):
```
Name_Node_Hdfs_Port: "9001"
Name_Node_Directory_Path: "/root/"
```
The `Name_Node_Hdfs_Port` is the port exposed for Data Node to connect.The `Data_Node_Directory_Path` is the directory path to store Hdfs metadata about data segments.

Dependencies
------------
None

Example Playbook
----------------
```
 - hosts: name_node
   roles:
     - shubhambhardwaj007.ansible_hadoop_software_installation_role
     - shubhambhardwaj007.hadoop_namenode
```
License
-------

GNU

Author Information
------------------
This role was created in 2021 by [Shubham Bhardwaj](https://galaxy.ansible.com/shubhambhardwaj007/hadoop_namenode)
