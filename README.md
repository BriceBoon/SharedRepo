# How to use 4-BooksWithRoles

## 1. What is 4-BooksWithRoles
4-BooksWithRoles is a playbook that will allow to deploy a Java Api on a specific folder as well as downloading 
Java 11 JRE for your Debian.

## 2. Organisation
4-BooksWithRoles contain 2 different folders :
-group_vars : containing the vars explaining to Ansible which computers should execute the playbook
-roles: containing the templates, tasks and vars that respectively contain hibernate configuration, the tasks
 that the playbook will execute and database and user configuration

4-BooksWithRoles also contain book.yml file that contain the different configuration possible for the book 
(which roles and hosts to use) and the hosts file that contain the IP adresses for the group_vars folder

## 3. How to run 4-BooksWithRoles
To run 4-BooksWithRoles you will have to launch the book.yml file that manage the other yml files and environment variables.
To do so, you should type "ansible-playbook book.yml" in your command line.
