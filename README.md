Role Name
========
NIS Slave

This role will configure NIS slave sever on CentOS 7,
following instructions from http://blog.zwiegnet.com/linux-server/configure-nis-slave-centos-6/

This is my first Ansible Galaxy role, so I am still figuring
out how the syntax for variables works.

Requirements
------------

An existing NIS Master server is required.

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here.

Role Variables
--------------
nisslave_masterip: The ip address of the nisdomain's master server
nisslave_nisdomain: The full name of the nisdomain.


A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: nisslave_servers
      roles:
         - role: jdelaporte.nisslave
	   nisslave_masterip: 192.168.1.2
	   nisslave_nisdomain:nis.domain

License
-------
MIT
BSD

Author Information
------------------
Joanna Delaporte

