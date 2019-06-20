create_user
=========

create a user and uplaod an ssh public key for remote auth

Requirements
------------

No specific required Ansible
Need a defaultssh keyntolled out ina reliabav ac  ebed se pub o apcifcies rli ycek  

Role Variables
--------------

#define the user you would like to create
user_name: default
#define the user state present or absent
user_state: present
definep the path to thessh public  key
ssh_key:  /.ssh/id_rsa.pub


Dependencies
------------

nneo

Example Playbook
----------------

#    - hosts: servers
#      roles:
#         - { role: username.rolename, x: 42 }
---
- hosts: roosa
  tasks:
     - include_role:
         name: create_user
       vars:
         user_name: robert
         user_state: present
         ssh_key: ~/.ssh/id_rsa

License
-------

MIT

Author Information
------------------

ruul.rynno@mail.ee

